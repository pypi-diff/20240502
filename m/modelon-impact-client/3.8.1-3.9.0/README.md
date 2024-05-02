# Comparing `tmp/modelon_impact_client-3.8.1.tar.gz` & `tmp/modelon_impact_client-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelon_impact_client-3.8.1.tar", max compression
+gzip compressed data, was "modelon_impact_client-3.9.0.tar", max compression
```

## Comparing `modelon_impact_client-3.8.1.tar` & `modelon_impact_client-3.9.0.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0     1479 2024-02-12 04:57:49.071783 modelon_impact_client-3.8.1/LICENSE.md
--rw-r--r--   0        0        0     2748 2024-02-12 04:57:49.078783 modelon_impact_client-3.8.1/README.md
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.039782 modelon_impact_client-3.8.1/modelon/__init__.py
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.069783 modelon_impact_client-3.8.1/modelon/impact/__init__.py
--rw-r--r--   0        0        0      978 2024-02-12 04:57:49.065783 modelon_impact_client-3.8.1/modelon/impact/client/__init__.py
--rw-r--r--   0        0        0    26054 2024-02-12 04:57:49.045782 modelon_impact_client-3.8.1/modelon/impact/client/client.py
--rw-r--r--   0        0        0     1577 2024-02-12 04:57:49.079783 modelon_impact_client-3.8.1/modelon/impact/client/configuration.py
--rw-r--r--   0        0        0     1937 2024-02-12 04:57:49.047783 modelon_impact_client-3.8.1/modelon/impact/client/credential_manager.py
--rw-r--r--   0        0        0      119 2024-02-12 04:57:49.058783 modelon_impact_client-3.8.1/modelon/impact/client/entities/__init__.py
--rw-r--r--   0        0        0      640 2024-02-12 04:57:49.035782 modelon_impact_client-3.8.1/modelon/impact/client/entities/asserts.py
--rw-r--r--   0        0        0    24785 2024-02-12 04:57:49.078783 modelon_impact_client-3.8.1/modelon/impact/client/entities/case.py
--rw-r--r--   0        0        0     2260 2024-02-12 04:57:49.092783 modelon_impact_client-3.8.1/modelon/impact/client/entities/content.py
--rw-r--r--   0        0        0     6622 2024-02-12 04:57:49.048782 modelon_impact_client-3.8.1/modelon/impact/client/entities/custom_function.py
--rw-r--r--   0        0        0    18420 2024-02-12 04:57:49.052783 modelon_impact_client-3.8.1/modelon/impact/client/entities/experiment.py
--rw-r--r--   0        0        0     2512 2024-02-12 04:57:49.034782 modelon_impact_client-3.8.1/modelon/impact/client/entities/external_result.py
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.090783 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/__init__.py
--rw-r--r--   0        0        0      180 2024-02-12 04:57:49.026782 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/case.py
--rw-r--r--   0        0        0      200 2024-02-12 04:57:49.069783 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/custom_function.py
--rw-r--r--   0        0        0      366 2024-02-12 04:57:49.063783 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/experiment.py
--rw-r--r--   0        0        0      192 2024-02-12 04:57:49.066783 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/external_result.py
--rw-r--r--   0        0        0      186 2024-02-12 04:57:49.064783 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/model.py
--rw-r--r--   0        0        0      190 2024-02-12 04:57:49.059783 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/model_executable.py
--rw-r--r--   0        0        0      190 2024-02-12 04:57:49.038782 modelon_impact_client-3.8.1/modelon/impact/client/entities/interfaces/workspace.py
--rw-r--r--   0        0        0      156 2024-02-12 04:57:49.060783 modelon_impact_client-3.8.1/modelon/impact/client/entities/log.py
--rw-r--r--   0        0        0    16772 2024-02-12 04:57:49.053783 modelon_impact_client-3.8.1/modelon/impact/client/entities/model.py
--rw-r--r--   0        0        0    12111 2024-02-12 04:57:49.043783 modelon_impact_client-3.8.1/modelon/impact/client/entities/model_executable.py
--rw-r--r--   0        0        0    12804 2024-02-12 04:57:49.087783 modelon_impact_client-3.8.1/modelon/impact/client/entities/project.py
--rw-r--r--   0        0        0     1988 2024-02-12 04:57:49.063783 modelon_impact_client-3.8.1/modelon/impact/client/entities/result.py
--rw-r--r--   0        0        0     1479 2024-02-12 04:57:49.027782 modelon_impact_client-3.8.1/modelon/impact/client/entities/status.py
--rw-r--r--   0        0        0    33288 2024-02-12 04:57:49.083783 modelon_impact_client-3.8.1/modelon/impact/client/entities/workspace.py
--rw-r--r--   0        0        0     1366 2024-02-12 04:57:49.050783 modelon_impact_client-3.8.1/modelon/impact/client/exceptions.py
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.036782 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/__init__.py
--rw-r--r--   0        0        0     5284 2024-02-12 04:57:49.098783 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/asserts.py
--rw-r--r--   0        0        0     4039 2024-02-12 04:57:49.046783 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/expansion.py
--rw-r--r--   0        0        0    10243 2024-02-12 04:57:49.029782 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/extension.py
--rw-r--r--   0        0        0    12627 2024-02-12 04:57:49.074783 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/fmu_based.py
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.070783 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/interfaces/__init__.py
--rw-r--r--   0        0        0      507 2024-02-12 04:57:49.047783 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/interfaces/definition.py
--rw-r--r--   0        0        0      409 2024-02-12 04:57:49.049783 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/interfaces/expansion.py
--rw-r--r--   0        0        0      188 2024-02-12 04:57:49.021782 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/interfaces/extension.py
--rw-r--r--   0        0        0    18531 2024-02-12 04:57:49.054782 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/model_based.py
--rw-r--r--   0        0        0     4699 2024-02-12 04:57:49.032782 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/operators.py
--rw-r--r--   0        0        0      643 2024-02-12 04:57:49.036782 modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/util.py
--rw-r--r--   0        0        0       65 2024-02-12 04:57:49.096783 modelon_impact_client-3.8.1/modelon/impact/client/jupyterhub/__init__.py
--rw-r--r--   0        0        0     2976 2024-02-12 04:57:49.073783 modelon_impact_client-3.8.1/modelon/impact/client/jupyterhub/authorize.py
--rw-r--r--   0        0        0      281 2024-02-12 04:57:49.102783 modelon_impact_client-3.8.1/modelon/impact/client/jupyterhub/exceptions.py
--rw-r--r--   0        0        0     2895 2024-02-12 04:57:49.051782 modelon_impact_client-3.8.1/modelon/impact/client/jupyterhub/sal.py
--rw-r--r--   0        0        0       79 2024-02-12 04:57:49.038782 modelon_impact_client-3.8.1/modelon/impact/client/operations/__init__.py
--rw-r--r--   0        0        0     5814 2024-02-12 04:57:49.055783 modelon_impact_client-3.8.1/modelon/impact/client/operations/base.py
--rw-r--r--   0        0        0     2440 2024-02-12 04:57:49.064783 modelon_impact_client-3.8.1/modelon/impact/client/operations/case.py
--rw-r--r--   0        0        0     2503 2024-02-12 04:57:49.065783 modelon_impact_client-3.8.1/modelon/impact/client/operations/content_import.py
--rw-r--r--   0        0        0     2245 2024-02-12 04:57:49.036782 modelon_impact_client-3.8.1/modelon/impact/client/operations/experiment.py
--rw-r--r--   0        0        0     2409 2024-02-12 04:57:49.066783 modelon_impact_client-3.8.1/modelon/impact/client/operations/external_result_import.py
--rw-r--r--   0        0        0     2720 2024-02-12 04:57:49.060783 modelon_impact_client-3.8.1/modelon/impact/client/operations/fmu_import.py
--rw-r--r--   0        0        0     5846 2024-02-12 04:57:49.096783 modelon_impact_client-3.8.1/modelon/impact/client/operations/model_executable.py
--rw-r--r--   0        0        0     2685 2024-02-12 04:57:49.114783 modelon_impact_client-3.8.1/modelon/impact/client/operations/project_import.py
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.041782 modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/__init__.py
--rw-r--r--   0        0        0     2600 2024-02-12 04:57:49.096783 modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/conversion.py
--rw-r--r--   0        0        0     3627 2024-02-12 04:57:49.099783 modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/exports.py
--rw-r--r--   0        0        0     2470 2024-02-12 04:57:49.074783 modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/imports.py
--rw-r--r--   0        0        0     3770 2024-02-12 04:57:49.080783 modelon_impact_client-3.8.1/modelon/impact/client/options.py
--rw-r--r--   0        0        0     5247 2024-02-12 04:57:49.067783 modelon_impact_client-3.8.1/modelon/impact/client/published_workspace_client.py
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.028782 modelon_impact_client-3.8.1/modelon/impact/client/py.typed
--rw-r--r--   0        0        0        0 2024-02-12 04:57:49.072783 modelon_impact_client-3.8.1/modelon/impact/client/sal/__init__.py
--rw-r--r--   0        0        0      132 2024-02-12 04:57:49.069783 modelon_impact_client-3.8.1/modelon/impact/client/sal/context.py
--rw-r--r--   0        0        0     1544 2024-02-12 04:57:49.056783 modelon_impact_client-3.8.1/modelon/impact/client/sal/custom_function.py
--rw-r--r--   0        0        0      671 2024-02-12 04:57:49.024782 modelon_impact_client-3.8.1/modelon/impact/client/sal/exceptions.py
--rw-r--r--   0        0        0     6787 2024-02-12 04:57:49.074783 modelon_impact_client-3.8.1/modelon/impact/client/sal/experiment.py
--rw-r--r--   0        0        0      630 2024-02-12 04:57:49.045782 modelon_impact_client-3.8.1/modelon/impact/client/sal/exports.py
--rw-r--r--   0        0        0     1476 2024-02-12 04:57:49.103783 modelon_impact_client-3.8.1/modelon/impact/client/sal/external_result.py
--rw-r--r--   0        0        0     3305 2024-02-12 04:57:49.067783 modelon_impact_client-3.8.1/modelon/impact/client/sal/http.py
--rw-r--r--   0        0        0      476 2024-02-12 04:57:49.106783 modelon_impact_client-3.8.1/modelon/impact/client/sal/imports.py
--rw-r--r--   0        0        0     3084 2024-02-12 04:57:49.080783 modelon_impact_client-3.8.1/modelon/impact/client/sal/model_executable.py
--rw-r--r--   0        0        0     4883 2024-02-12 04:57:49.075783 modelon_impact_client-3.8.1/modelon/impact/client/sal/project.py
--rw-r--r--   0        0        0     5097 2024-02-12 04:57:49.048782 modelon_impact_client-3.8.1/modelon/impact/client/sal/request.py
--rw-r--r--   0        0        0     5114 2024-02-12 04:57:49.064783 modelon_impact_client-3.8.1/modelon/impact/client/sal/response.py
--rw-r--r--   0        0        0     5082 2024-02-12 04:57:49.037782 modelon_impact_client-3.8.1/modelon/impact/client/sal/service.py
--rw-r--r--   0        0        0      885 2024-02-12 04:57:49.030782 modelon_impact_client-3.8.1/modelon/impact/client/sal/uri.py
--rw-r--r--   0        0        0      454 2024-02-12 04:57:49.057783 modelon_impact_client-3.8.1/modelon/impact/client/sal/users.py
--rw-r--r--   0        0        0    12399 2024-02-12 04:57:49.056783 modelon_impact_client-3.8.1/modelon/impact/client/sal/workspace.py
--rw-r--r--   0        0        0     1440 2024-02-12 04:59:19.745681 modelon_impact_client-3.8.1/pyproject.toml
--rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1479 2024-02-15 04:09:47.458728 modelon_impact_client-3.9.0/LICENSE.md
+-rw-r--r--   0        0        0     2748 2024-02-15 04:09:47.470728 modelon_impact_client-3.9.0/README.md
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.413728 modelon_impact_client-3.9.0/modelon/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.454728 modelon_impact_client-3.9.0/modelon/impact/__init__.py
+-rw-r--r--   0        0        0     1035 2024-02-15 04:09:47.448728 modelon_impact_client-3.9.0/modelon/impact/client/__init__.py
+-rw-r--r--   0        0        0    26054 2024-02-15 04:09:47.418727 modelon_impact_client-3.9.0/modelon/impact/client/client.py
+-rw-r--r--   0        0        0     1577 2024-02-15 04:09:47.470728 modelon_impact_client-3.9.0/modelon/impact/client/configuration.py
+-rw-r--r--   0        0        0     1937 2024-02-15 04:09:47.419728 modelon_impact_client-3.9.0/modelon/impact/client/credential_manager.py
+-rw-r--r--   0        0        0      119 2024-02-15 04:09:47.435728 modelon_impact_client-3.9.0/modelon/impact/client/entities/__init__.py
+-rw-r--r--   0        0        0      640 2024-02-15 04:09:47.408728 modelon_impact_client-3.9.0/modelon/impact/client/entities/asserts.py
+-rw-r--r--   0        0        0    24785 2024-02-15 04:09:47.468728 modelon_impact_client-3.9.0/modelon/impact/client/entities/case.py
+-rw-r--r--   0        0        0     2260 2024-02-15 04:09:47.486728 modelon_impact_client-3.9.0/modelon/impact/client/entities/content.py
+-rw-r--r--   0        0        0     6622 2024-02-15 04:09:47.420728 modelon_impact_client-3.9.0/modelon/impact/client/entities/custom_function.py
+-rw-r--r--   0        0        0    18420 2024-02-15 04:09:47.425728 modelon_impact_client-3.9.0/modelon/impact/client/entities/experiment.py
+-rw-r--r--   0        0        0     2512 2024-02-15 04:09:47.408728 modelon_impact_client-3.9.0/modelon/impact/client/entities/external_result.py
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.485728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/__init__.py
+-rw-r--r--   0        0        0      180 2024-02-15 04:09:47.399727 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/case.py
+-rw-r--r--   0        0        0      200 2024-02-15 04:09:47.454728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/custom_function.py
+-rw-r--r--   0        0        0      366 2024-02-15 04:09:47.445728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/experiment.py
+-rw-r--r--   0        0        0      192 2024-02-15 04:09:47.449728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/external_result.py
+-rw-r--r--   0        0        0      186 2024-02-15 04:09:47.446728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/model.py
+-rw-r--r--   0        0        0      190 2024-02-15 04:09:47.436728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/model_executable.py
+-rw-r--r--   0        0        0      190 2024-02-15 04:09:47.411728 modelon_impact_client-3.9.0/modelon/impact/client/entities/interfaces/workspace.py
+-rw-r--r--   0        0        0      156 2024-02-15 04:09:47.440728 modelon_impact_client-3.9.0/modelon/impact/client/entities/log.py
+-rw-r--r--   0        0        0    16772 2024-02-15 04:09:47.426728 modelon_impact_client-3.9.0/modelon/impact/client/entities/model.py
+-rw-r--r--   0        0        0    12111 2024-02-15 04:09:47.417728 modelon_impact_client-3.9.0/modelon/impact/client/entities/model_executable.py
+-rw-r--r--   0        0        0    12804 2024-02-15 04:09:47.483728 modelon_impact_client-3.9.0/modelon/impact/client/entities/project.py
+-rw-r--r--   0        0        0     1988 2024-02-15 04:09:47.445728 modelon_impact_client-3.9.0/modelon/impact/client/entities/result.py
+-rw-r--r--   0        0        0     1479 2024-02-15 04:09:47.400727 modelon_impact_client-3.9.0/modelon/impact/client/entities/status.py
+-rw-r--r--   0        0        0    34034 2024-02-15 04:09:47.475728 modelon_impact_client-3.9.0/modelon/impact/client/entities/workspace.py
+-rw-r--r--   0        0        0     1366 2024-02-15 04:09:47.422728 modelon_impact_client-3.9.0/modelon/impact/client/exceptions.py
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.409727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/__init__.py
+-rw-r--r--   0        0        0     5284 2024-02-15 04:09:47.494728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/asserts.py
+-rw-r--r--   0        0        0     4039 2024-02-15 04:09:47.419728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/expansion.py
+-rw-r--r--   0        0        0    10243 2024-02-15 04:09:47.401727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/extension.py
+-rw-r--r--   0        0        0    12627 2024-02-15 04:09:47.463728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/fmu_based.py
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.455728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/__init__.py
+-rw-r--r--   0        0        0      507 2024-02-15 04:09:47.420728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/definition.py
+-rw-r--r--   0        0        0      409 2024-02-15 04:09:47.421728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/expansion.py
+-rw-r--r--   0        0        0      188 2024-02-15 04:09:47.390727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/interfaces/extension.py
+-rw-r--r--   0        0        0    18531 2024-02-15 04:09:47.426728 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/model_based.py
+-rw-r--r--   0        0        0     4699 2024-02-15 04:09:47.405727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/operators.py
+-rw-r--r--   0        0        0      643 2024-02-15 04:09:47.409727 modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/util.py
+-rw-r--r--   0        0        0       65 2024-02-15 04:09:47.492728 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/__init__.py
+-rw-r--r--   0        0        0     2976 2024-02-15 04:09:47.461728 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/authorize.py
+-rw-r--r--   0        0        0      281 2024-02-15 04:09:47.499729 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/exceptions.py
+-rw-r--r--   0        0        0     2895 2024-02-15 04:09:47.422728 modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/sal.py
+-rw-r--r--   0        0        0       79 2024-02-15 04:09:47.411728 modelon_impact_client-3.9.0/modelon/impact/client/operations/__init__.py
+-rw-r--r--   0        0        0     5814 2024-02-15 04:09:47.428728 modelon_impact_client-3.9.0/modelon/impact/client/operations/base.py
+-rw-r--r--   0        0        0     2440 2024-02-15 04:09:47.447728 modelon_impact_client-3.9.0/modelon/impact/client/operations/case.py
+-rw-r--r--   0        0        0     2503 2024-02-15 04:09:47.448728 modelon_impact_client-3.9.0/modelon/impact/client/operations/content_import.py
+-rw-r--r--   0        0        0     2245 2024-02-15 04:09:47.410728 modelon_impact_client-3.9.0/modelon/impact/client/operations/experiment.py
+-rw-r--r--   0        0        0     2409 2024-02-15 04:09:47.450728 modelon_impact_client-3.9.0/modelon/impact/client/operations/external_result_import.py
+-rw-r--r--   0        0        0     2720 2024-02-15 04:09:47.440728 modelon_impact_client-3.9.0/modelon/impact/client/operations/fmu_import.py
+-rw-r--r--   0        0        0     5846 2024-02-15 04:09:47.492728 modelon_impact_client-3.9.0/modelon/impact/client/operations/model_executable.py
+-rw-r--r--   0        0        0     2685 2024-02-15 04:09:47.504729 modelon_impact_client-3.9.0/modelon/impact/client/operations/project_import.py
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.415727 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/__init__.py
+-rw-r--r--   0        0        0     2600 2024-02-15 04:09:47.493728 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/conversion.py
+-rw-r--r--   0        0        0     3627 2024-02-15 04:09:47.494728 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/exports.py
+-rw-r--r--   0        0        0     2470 2024-02-15 04:09:47.463728 modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/imports.py
+-rw-r--r--   0        0        0     3770 2024-02-15 04:09:47.472728 modelon_impact_client-3.9.0/modelon/impact/client/options.py
+-rw-r--r--   0        0        0     5373 2024-02-15 04:09:47.452728 modelon_impact_client-3.9.0/modelon/impact/client/published_workspace_client.py
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.400727 modelon_impact_client-3.9.0/modelon/impact/client/py.typed
+-rw-r--r--   0        0        0        0 2024-02-15 04:09:47.459728 modelon_impact_client-3.9.0/modelon/impact/client/sal/__init__.py
+-rw-r--r--   0        0        0      132 2024-02-15 04:09:47.455728 modelon_impact_client-3.9.0/modelon/impact/client/sal/context.py
+-rw-r--r--   0        0        0     1544 2024-02-15 04:09:47.430728 modelon_impact_client-3.9.0/modelon/impact/client/sal/custom_function.py
+-rw-r--r--   0        0        0      671 2024-02-15 04:09:47.395727 modelon_impact_client-3.9.0/modelon/impact/client/sal/exceptions.py
+-rw-r--r--   0        0        0     6787 2024-02-15 04:09:47.463728 modelon_impact_client-3.9.0/modelon/impact/client/sal/experiment.py
+-rw-r--r--   0        0        0      630 2024-02-15 04:09:47.418727 modelon_impact_client-3.9.0/modelon/impact/client/sal/exports.py
+-rw-r--r--   0        0        0     1476 2024-02-15 04:09:47.500728 modelon_impact_client-3.9.0/modelon/impact/client/sal/external_result.py
+-rw-r--r--   0        0        0     3305 2024-02-15 04:09:47.452728 modelon_impact_client-3.9.0/modelon/impact/client/sal/http.py
+-rw-r--r--   0        0        0      476 2024-02-15 04:09:47.503728 modelon_impact_client-3.9.0/modelon/impact/client/sal/imports.py
+-rw-r--r--   0        0        0     3084 2024-02-15 04:09:47.472728 modelon_impact_client-3.9.0/modelon/impact/client/sal/model_executable.py
+-rw-r--r--   0        0        0     4883 2024-02-15 04:09:47.464728 modelon_impact_client-3.9.0/modelon/impact/client/sal/project.py
+-rw-r--r--   0        0        0     5097 2024-02-15 04:09:47.420728 modelon_impact_client-3.9.0/modelon/impact/client/sal/request.py
+-rw-r--r--   0        0        0     5114 2024-02-15 04:09:47.446728 modelon_impact_client-3.9.0/modelon/impact/client/sal/response.py
+-rw-r--r--   0        0        0     5082 2024-02-15 04:09:47.411728 modelon_impact_client-3.9.0/modelon/impact/client/sal/service.py
+-rw-r--r--   0        0        0      885 2024-02-15 04:09:47.402727 modelon_impact_client-3.9.0/modelon/impact/client/sal/uri.py
+-rw-r--r--   0        0        0      454 2024-02-15 04:09:47.435728 modelon_impact_client-3.9.0/modelon/impact/client/sal/users.py
+-rw-r--r--   0        0        0    12555 2024-02-15 04:09:47.431728 modelon_impact_client-3.9.0/modelon/impact/client/sal/workspace.py
+-rw-r--r--   0        0        0     1440 2024-02-15 04:13:33.738229 modelon_impact_client-3.9.0/pyproject.toml
+-rw-r--r--   0        0        0     3722 1970-01-01 00:00:00.000000 modelon_impact_client-3.9.0/PKG-INFO
```

### Comparing `modelon_impact_client-3.8.1/LICENSE.md` & `modelon_impact_client-3.9.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/README.md` & `modelon_impact_client-3.9.0/README.md`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/__init__.py` & `modelon_impact_client-3.9.0/modelon/impact/client/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from modelon.impact.client.client import Client
 from modelon.impact.client.entities.project import (
     ContentType,
     ProjectType,
     StorageLocation,
 )
-from modelon.impact.client.entities.workspace import WorkspaceDefinition
+from modelon.impact.client.entities.workspace import (
+    AccessSettings,
+    PublishedWorkspaceType,
+    WorkspaceDefinition,
+)
 from modelon.impact.client.experiment_definition.expansion import (
     FullFactorial,
     LatinHypercube,
     Sobol,
 )
 from modelon.impact.client.experiment_definition.extension import (
     SimpleExperimentExtension,
```

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/client.py` & `modelon_impact_client-3.9.0/modelon/impact/client/client.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/configuration.py` & `modelon_impact_client-3.9.0/modelon/impact/client/configuration.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/credential_manager.py` & `modelon_impact_client-3.9.0/modelon/impact/client/credential_manager.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/asserts.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/case.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/content.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/content.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/custom_function.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/experiment.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/external_result.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/model.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/model.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/model_executable.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/project.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/result.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/status.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/status.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/entities/workspace.py` & `modelon_impact_client-3.9.0/modelon/impact/client/entities/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 ExperimentDefinition = Union[
     Type[BaseExperimentDefinition],
     Dict[str, Any],
 ]
 
 
 @dataclass
+class AccessSettings:
+    group_names: Optional[List[str]] = None
+
+
+@dataclass
 class Reference:
     id: str
 
 
 @dataclass
 class ReleasedProjectReference:
     id: str
@@ -663,40 +668,61 @@
             self._workspace_id, path_to_result, label=label, description=description
         )
         return ExternalResultImportOperation[ExternalResult](
             resp["data"]["location"], self._sal, ExternalResult.from_operation
         )
 
     def export(
-        self, publish: bool = False, class_path: Optional[str] = None
+        self,
+        publish: bool = False,
+        class_path: Optional[str] = None,
+        access: Optional[AccessSettings] = None,
     ) -> WorkspaceExportOperation:
         """Exports the workspace as a binary compressed archive. Similar to
         :obj:`~modelon.impact.client.entities.workspace.Workspace.download`, but gives
         more control for getting the workspace async. Returns an
         modelon.impact.client.operations.workspace.exports .WorkspaceExportOperation
         class object. The binary archive is stored to cloud storage if the publish
         argument is set to True.
 
         Args:
             publish: To export the workspace and save it to cloud storage.
             class_path: The Modelica class path of the model. If specified,
                 the workspace is exported in app mode.
+            access: The access control settings for the workspace.
 
         Returns:
             An WorkspaceExportOperation class object.
 
         Example::
 
             path = workspace.export().wait().download_as('/home/workspace.zip')
+
+            # Publish a workspace
             path = workspace.export(publish=True,
                 class_path='Modelica.Blocks.Examples.PID_Controller')
 
+            # Publish a workspace without sharing with group
+            from modelon.impact.client import AccessSettings
+
+            path = workspace.export(publish=True,
+                class_path='Modelica.Blocks.Examples.PID_Controller',
+                access=AccessSettings(group_names=[])
+            )
+
         """
+        if access:
+            access_settings = {"groupNames": access.group_names}
+        else:
+            access_settings = None
         resp = self._sal.workspace.workspace_export_setup(
-            self._workspace_id, publish, class_path
+            self._workspace_id,
+            publish,
+            class_path,
+            access_settings,
         )
         return WorkspaceExportOperation[Workspace](
             resp["data"]["location"], self._sal, Export.from_operation
         )
 
     def download(self, path: str) -> str:
         """Downloads the workspace as a binary compressed archive. Returns the local
```

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/exceptions.py` & `modelon_impact_client-3.9.0/modelon/impact/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/asserts.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/asserts.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/expansion.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/expansion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/extension.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/extension.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/fmu_based.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/fmu_based.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/model_based.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/model_based.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/operators.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/operators.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/experiment_definition/util.py` & `modelon_impact_client-3.9.0/modelon/impact/client/experiment_definition/util.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/jupyterhub/authorize.py` & `modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/authorize.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/jupyterhub/sal.py` & `modelon_impact_client-3.9.0/modelon/impact/client/jupyterhub/sal.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/base.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/base.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/case.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/case.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/content_import.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/content_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/experiment.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/external_result_import.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/external_result_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/fmu_import.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/fmu_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/model_executable.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/project_import.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/project_import.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/conversion.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/conversion.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/exports.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/operations/workspace/imports.py` & `modelon_impact_client-3.9.0/modelon/impact/client/operations/workspace/imports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/options.py` & `modelon_impact_client-3.9.0/modelon/impact/client/options.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/published_workspace_client.py` & `modelon_impact_client-3.9.0/modelon/impact/client/published_workspace_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,16 +129,19 @@
             maximum: Maximum number of published workspaces to return.
 
         Returns:
             A list of PublishedWorkspaceAccess class objects.
 
         Example::
 
+            from modelon.impact.client.published_workspace_client import
+                PublishedWorkspaceAccessKind
+
             pw_client = client.get_published_workspaces_client()
-            pw_client.get_by_kind(PublishedWorkspaceAccessKind.REQUESTED_BY_ME)
+            pw_client.get_by_access_kind(PublishedWorkspaceAccessKind.REQUESTED_BY_ME)
 
         """
         data = self._sal.workspace.get_published_workspaces_by_kind(
             access_kind.value, first, maximum
         )["data"]["items"]
         return [
             PublishedWorkspaceAccess(
```

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/custom_function.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/custom_function.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/exceptions.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/exceptions.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/experiment.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/experiment.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/exports.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/exports.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/external_result.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/external_result.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/http.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/http.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/model_executable.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/model_executable.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/project.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/project.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/request.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/request.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/response.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/response.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/service.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/service.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/uri.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/uri.py`

 * *Files identical despite different names*

### Comparing `modelon_impact_client-3.8.1/modelon/impact/client/sal/workspace.py` & `modelon_impact_client-3.9.0/modelon/impact/client/sal/workspace.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,18 +62,24 @@
             self._base_uri
             / f"api/workspaces/{workspace_id}/dependencies?vcsInfo={vcs_info}"
             f"&includeDisabled={include_disabled}"
         ).resolve()
         return self._http_client.get_json(url)
 
     def workspace_export_setup(
-        self, workspace_id: str, publish: bool, class_path: Optional[str] = None
+        self,
+        workspace_id: str,
+        publish: bool,
+        class_path: Optional[str] = None,
+        access_settings: Optional[Dict[str, Any]] = None,
     ) -> Dict[str, Any]:
         url = (self._base_uri / "api/workspace-exports").resolve()
-        body = {"workspaceId": workspace_id, 'publish': publish}
+        body = {"workspaceId": workspace_id, "publish": publish}
+        if access_settings:
+            body["access"] = access_settings
         if class_path:
             body['appMode'] = {'model': class_path}
         return self._http_client.post_json(url, body=body)
 
     def workspace_conversion_setup(
         self, workspace_id: str, backup_name: Optional[str]
     ) -> Dict[str, Any]:
```

### Comparing `modelon_impact_client-3.8.1/pyproject.toml` & `modelon_impact_client-3.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "modelon-impact-client"
 packages = [
     { include = "modelon" },
 ]
-version = "3.8.1"
+version = "3.9.0"
 description = "Client library for easy scripting against Modelon Impact"
 readme = "README.md"
 homepage = "https://www.modelon.com/modelon-impact"
 repository = "https://github.com/modelon-community/impact-client-python"
 documentation = "https://modelon-impact-client.readthedocs.io"
 license = "BSD"
 authors = [
```

### Comparing `modelon_impact_client-3.8.1/PKG-INFO` & `modelon_impact_client-3.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelon-impact-client
-Version: 3.8.1
+Version: 3.9.0
 Summary: Client library for easy scripting against Modelon Impact
 Home-page: https://www.modelon.com/modelon-impact
 License: BSD
 Keywords: impact,client,API
 Author: WEP
 Author-email: impact@modelon.com
 Requires-Python: >=3.8.0,<4.0.0
```

