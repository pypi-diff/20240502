# Comparing `tmp/lsst-pipe-base-26.2024.900.tar.gz` & `tmp/lsst_pipe_base-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-pipe-base-26.2024.900.tar", last modified: Thu Feb 29 10:21:38 2024, max compression
+gzip compressed data, was "lsst_pipe_base-27.0.0rc1.tar", last modified: Wed May  1 21:16:43 2024, max compression
```

## Comparing `lsst-pipe-base-26.2024.900.tar` & `lsst_pipe_base-27.0.0rc1.tar`

### file list

```diff
@@ -1,143 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      362 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.628640 lsst-pipe-base-26.2024.900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.632640 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/
--rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipeline.rst
--rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipelinetask.rst
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-framework-overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-retargeting-howto.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-a-pipeline-task.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.628640 lsst-pipe-base-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.632640 lsst-pipe-base-26.2024.900/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.632640 lsst-pipe-base-26.2024.900/python/lsst/pipe/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.636640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6227 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_datasetQueryConstraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    11217 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    30005 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_observation_dimension_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17418 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_quantumContext.py
--rw-r--r--   0 runner    (1001) docker     (127)     4122 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    24073 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_task_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    27499 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/automatic_connection_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/resources.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    18440 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connectionTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    53003 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connections.py
--rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/executionButlerBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    16535 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/execution_reports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/pexConfig.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.640640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_implDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_loadHelpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    27947 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_versionDeserializers.py
--rw-r--r--   0 runner    (1001) docker     (127)    53094 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/quantumNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     7463 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeTools.py
--rw-r--r--   0 runner    (1001) docker     (127)    62364 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineTask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10316 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31317 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_edges.py
--rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7380 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    72184 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    36635 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/io.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
--rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
--rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
--rw-r--r--   0 runner    (1001) docker     (127)    28593 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/prerequisite_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    53756 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_skeleton.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/register_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/transfer_from_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    15113 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/taskFactory.py
--rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/testUtils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.644640 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_data_id_match.py
--rw-r--r--   0 runner    (1001) docker     (127)    28357 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    22388 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/no_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/pipelineStepTester.py
--rw-r--r--   0 runner    (1001) docker     (127)    18714 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/simpleQGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst/pipe/base/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2077 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:21:38.000000 lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:21:38.652640 lsst-pipe-base-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_cliCmdRegisterInstrument.py
--rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_configOverrides.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_config_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_dataid_match.py
--rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_dataset_handle.py
--rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_dynamic_connections.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_executionButler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2621 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_execution_reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_graphBuilder.py
--rw-r--r--   0 runner    (1001) docker     (127)    14583 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_instrument.py
--rw-r--r--   0 runner    (1001) docker     (127)     8528 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipeTools.py
--rw-r--r--   0 runner    (1001) docker     (127)     7931 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)    26675 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipelineIR.py
--rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipelineLoadSubset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15012 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipelineTask.py
--rw-r--r--   0 runner    (1001) docker     (127)    66381 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_pipeline_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    25662 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_quantumGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_struct.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_task.py
--rw-r--r--   0 runner    (1001) docker     (127)    10161 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_taskmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-02-29 10:21:25.000000 lsst-pipe-base-26.2024.900/tests/test_testUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.923969 lsst_pipe_base-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      362 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-01 21:16:43.923969 lsst_pipe_base-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.899969 lsst_pipe_base-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.903969 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/
+-rw-r--r--   0 runner    (1001) docker     (127)    20761 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    25134 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/creating-a-pipeline.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    50486 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/creating-a-pipelinetask.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/creating-a-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2808 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/task-framework-overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/task-retargeting-howto.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11157 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/testing-a-pipeline-task.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7191 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/working-with-pipeline-graphs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.899969 lsst_pipe_base-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.903969 lsst_pipe_base-27.0.0rc1/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.903969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.911969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_datasetQueryConstraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11352 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30075 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8027 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_observation_dimension_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17530 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_quantumContext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8947 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24451 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_task_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27546 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3298 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/automatic_connection_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7214 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/caching_limited_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.911969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.911969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.911969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1484 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/resources.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11983 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14661 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19386 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/connectionTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52230 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21283 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/executionButlerBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16969 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/execution_reports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.911969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/formatters/pexConfig.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.915969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6784 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/_implDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11857 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/_loadHelpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27987 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/_versionDeserializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56203 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/graphSummary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/quantumNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeTools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63422 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43674 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8381 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipelineTask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.915969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20859 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10392 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_dataset_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32831 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_edges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3621 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9194 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_mapping_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75520 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4395 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_task_subsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39356 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29594 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/io.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.915969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17157 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15036 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16537 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8992 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_show.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28590 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/prerequisite_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    54285 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/quantum_graph_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18544 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/quantum_graph_skeleton.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.919969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/register_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6433 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/transfer_from_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5048 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15145 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/taskFactory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18456 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/testUtils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.919969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.919969 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6331 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/_data_id_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27231 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/_pipeline_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22758 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4710 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/no_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4882 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/pipelineStepTester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/simpleQGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.923969 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:43.000000 lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-01 21:16:43.923969 lsst_pipe_base-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:43.923969 lsst_pipe_base-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_caching_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_cliCmdRegisterInstrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12290 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_configOverrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_config_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10061 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6144 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_dataid_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8118 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_dataset_handle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15553 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_dynamic_connections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_executionButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3296 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_execution_reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_graphBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16055 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_instrument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26529 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_pipelineIR.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7817 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_pipelineLoadSubset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15972 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_pipelineTask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67752 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_pipeline_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26949 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_quantumGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_struct.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13796 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10424 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_taskmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24994 2024-05-01 21:16:37.000000 lsst_pipe_base-27.0.0rc1/tests/test_testUtils.py
```

### Comparing `lsst-pipe-base-26.2024.900/PKG-INFO` & `lsst_pipe_base-27.0.0rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pipe-base-26.2024.900/README.md` & `lsst_pipe_base-27.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/bsd_license.txt` & `lsst_pipe_base-27.0.0rc1/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/CHANGES.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipeline.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/creating-a-pipeline.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-pipelinetask.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/creating-a-pipelinetask.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/creating-a-task.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/creating-a-task.rst`

 * *Files 1% similar despite different names*

```diff
@@ -303,8 +303,8 @@
 Variant tasks
 =============
 
 When there are (or are expected to be) different versions of a given task, those tasks should inherit from an abstract base class that defines the interface and is itself a subclass of `lsst.pipe.base.Task`.
 Star selectors (`lsst.meas.algorithms.BaseStarSelectorTask`) and PSF determiners (`lsst.meas.algorithms.BasePsfDeterminerTask`) are two examples of tasks with multiple variants.
 The abstract base class should be written using `abc.ABC` or `abc.ABCMeta`.
 The same module that defines the abstract base class should also define a registry, using `lsst.pex.config.RegistryField`, and all implementations should register themselves with that registry.
-Examples include `lsst.meas.algorithms.starSelectorRegistry` and `lsst.meas.algorithms.psfDeterminerRegistry`.
+Examples include :py:mod:`lsst.meas.algorithms.starSelectorRegistry` and :py:mod:`lsst.meas.algorithms.psfDeterminerRegistry`.
```

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/index.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,14 @@
 .. automodapi:: lsst.pipe.base.pipeline_graph
    :no-main-docstr:
 
 .. automodapi:: lsst.pipe.base.testUtils
    :no-main-docstr:
 
 .. automodapi:: lsst.pipe.base.connectionTypes
-  :no-main-docstr:
 
 .. automodapi:: lsst.pipe.base.pipelineIR
   :no-main-docstr:
 
 .. automodapi:: lsst.pipe.base.tests.mocks
 
 .. automodapi:: lsst.pipe.base.execution_reports
@@ -100,7 +99,9 @@
 QuantumGraph generation API reference
 -------------------------------------
 
 .. automodapi:: lsst.pipe.base.quantum_graph_builder
 .. automodapi:: lsst.pipe.base.quantum_graph_skeleton
 .. automodapi:: lsst.pipe.base.prerequisite_helpers
 .. automodapi:: lsst.pipe.base.all_dimensions_quantum_graph_builder
+   :skip: DatasetQueryConstraintVariant
+.. automodapi:: lsst.pipe.base._datasetQueryConstraints
```

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-framework-overview.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/task-framework-overview.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/task-retargeting-howto.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/task-retargeting-howto.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-a-pipeline-task.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/testing-a-pipeline-task.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/testing-pipelines-with-mocks.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/doc/lsst.pipe.base/working-with-pipeline-graphs.rst` & `lsst_pipe_base-27.0.0rc1/doc/lsst.pipe.base/working-with-pipeline-graphs.rst`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/gpl-v3.0.txt` & `lsst_pipe_base-27.0.0rc1/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/pyproject.toml` & `lsst_pipe_base-27.0.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -131,17 +131,21 @@
 # Docstring at the very first line is not required
 # D200, D205 and D400 all complain if the first sentence of the docstring does
 # not fit on one line.
 # Do not require docstrings in __init__.py files (D104)
 add-ignore = ["D107", "D105", "D102", "D100", "D200", "D205", "D400", "D104"]
 
 [tool.ruff]
+line-length = 110
+target-version = "py311"
 exclude = [
     "__init__.py",
 ]
+
+[tool.ruff.lint]
 ignore = [
     "N802",
     "N803",
     "N806",
     "N812",
     "N815",
     "N816",
@@ -151,34 +155,32 @@
     "D102",
     "D104",
     "D100",
     "D200",
     "D205",
     "D400",
 ]
-line-length = 110
 select = [
     "E",  # pycodestyle
     "F",  # pyflakes
     "N",  # pep8-naming
     "W",  # pycodestyle
     "D",  # pydocstyle
 ]
-target-version = "py311"
 extend-select = [
     "RUF100", # Warn about unused noqa
 ]
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 79
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # Do not need to add class docs to the example classes.
 "doc/_static/pipe_base/PipelineTask_Examples/*.py" = ["D101"]
 
 [tool.numpydoc_validation]
 checks = [
     "all",  # All except the rules listed below.
     "SA01",  # See Also section.
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_datasetQueryConstraints.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_datasetQueryConstraints.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,16 +21,17 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Module Defining variants for valid values used to constrain datasets in a
-graph building query.
+"""Symbols defined in this package should be imported from
+`all_dimensions_quantum_graph_builder` instead; it only appears in the docs
+due to limitations in Sphinx.
 """
 
 from __future__ import annotations
 
 __all__ = ("DatasetQueryConstraintVariant",)
 
 import sys
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_dataset_handle.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_dataset_handle.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
     _empty = DataCoordinate.make_empty(DimensionUniverse())
 
     def __init__(
         self,
         inMemoryDataset: Any,
         *,
-        storageClass: StorageClass | None = None,
+        storageClass: StorageClass | str | None = None,
         parameters: dict[str, Any] | None = None,
         dataId: DataId | None = None,
         copy: bool = False,
         **kwargs: Any,
     ):
         object.__setattr__(self, "inMemoryDataset", inMemoryDataset)
         object.__setattr__(self, "storageClass", storageClass)
@@ -248,30 +248,33 @@
         Raises
         ------
         KeyError
             Raised if the storage class could not be found.
         """
         factory = StorageClassFactory()
         if self.storageClass:
-            return factory.getStorageClass(self.storageClass)
+            if isinstance(self.storageClass, str):
+                return factory.getStorageClass(self.storageClass)
+            else:
+                return self.storageClass
 
         # Need to match python type.
         pytype = type(self.inMemoryDataset)
         return factory.findStorageClass(pytype)
 
     inMemoryDataset: Any
     """The object to store in this dataset handle for later retrieval.
     """
 
     dataId: DataCoordinate | frozendict
     """The `~lsst.daf.butler.DataCoordinate` associated with this dataset
     handle.
     """
 
-    storageClass: str | None = None
+    storageClass: StorageClass | str | None = None
     """The name of the `~lsst.daf.butler.StorageClass` associated with this
     dataset.
 
     If `None`, the storage class will be looked up from the factory.
     """
 
     parameters: dict | None = None
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_instrument.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_instrument.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,20 +30,21 @@
 __all__ = ("Instrument",)
 
 import contextlib
 import datetime
 import os.path
 from abc import ABCMeta, abstractmethod
 from collections.abc import Sequence
-from typing import TYPE_CHECKING, Any, cast, final
+from typing import TYPE_CHECKING, Any, Self, cast, final
 
 from lsst.daf.butler import DataCoordinate, DataId, DimensionPacker, DimensionRecord, Formatter
 from lsst.daf.butler.registry import DataIdError
 from lsst.pex.config import Config, RegistryField
 from lsst.utils import doImportType
+from lsst.utils.introspection import get_full_type_name
 
 from ._observation_dimension_packer import observation_packer_registry
 
 if TYPE_CHECKING:
     from lsst.daf.butler import Registry
 
 
@@ -132,16 +133,16 @@
             with registry.transaction():
                 registry.syncDimensionData("instrument", ...)
                 registry.syncDimensionData("detector", ...)
                 self.registerFilters(registry)
         """
         raise NotImplementedError()
 
-    @staticmethod
-    def fromName(name: str, registry: Registry, collection_prefix: str | None = None) -> Instrument:
+    @classmethod
+    def fromName(cls, name: str, registry: Registry, collection_prefix: str | None = None) -> Self:
         """Given an instrument name and a butler registry, retrieve a
         corresponding instantiated instrument object.
 
         Parameters
         ----------
         name : `str`
             Name of the instrument (must match the return value of `getName`).
@@ -180,20 +181,20 @@
         if not records:
             raise LookupError(f"No registered instrument with name '{name}'.")
         cls_name = records[0].class_name
         if not isinstance(cls_name, str):
             raise TypeError(
                 f"Unexpected class name retrieved from {name} instrument dimension (got {cls_name})"
             )
-        return Instrument._from_cls_name(cls_name, collection_prefix)
+        return cls._from_cls_name(cls_name, collection_prefix)
 
-    @staticmethod
+    @classmethod
     def from_string(
-        name: str, registry: Registry | None = None, collection_prefix: str | None = None
-    ) -> Instrument:
+        cls, name: str, registry: Registry | None = None, collection_prefix: str | None = None
+    ) -> Self:
         """Return an instance from the short name or class name.
 
         If the instrument name is not qualified (does not contain a '.') and a
         butler registry is provided, this will attempt to load the instrument
         using `Instrument.fromName()`. Otherwise the instrument will be
         imported and instantiated.
 
@@ -226,33 +227,33 @@
 
         See Also
         --------
         Instrument.fromName : Constructing Instrument from a name.
         """
         if "." not in name and registry is not None:
             try:
-                instr = Instrument.fromName(name, registry, collection_prefix=collection_prefix)
+                instr = cls.fromName(name, registry, collection_prefix=collection_prefix)
             except Exception as err:
                 raise RuntimeError(
                     f"Could not get instrument from name: {name}. Failed with exception: {err}"
                 ) from err
         else:
             try:
                 instr_class = doImportType(name)
             except Exception as err:
                 raise RuntimeError(
                     f"Could not import instrument: {name}. Failed with exception: {err}"
                 ) from err
             instr = instr_class(collection_prefix=collection_prefix)
-        if not isinstance(instr, Instrument):
-            raise TypeError(f"{name} is not an Instrument subclass.")
+        if not isinstance(instr, cls):
+            raise TypeError(f"{name} is not a {get_full_type_name(cls)} subclass.")
         return instr
 
-    @staticmethod
-    def from_data_id(data_id: DataCoordinate, collection_prefix: str | None = None) -> Instrument:
+    @classmethod
+    def from_data_id(cls, data_id: DataCoordinate, collection_prefix: str | None = None) -> Self:
         """Instantiate an `Instrument` object from a fully-expanded data ID.
 
         Parameters
         ----------
         data_id : `~lsst.daf.butler.DataCoordinate`
             Expanded data ID that includes the instrument dimension.
         collection_prefix : `str`, optional
@@ -268,20 +269,20 @@
 
         Raises
         ------
         TypeError
             Raised if the class name retrieved is not a string or the imported
             symbol is not an `Instrument` subclass.
         """
-        return Instrument._from_cls_name(
+        return cls._from_cls_name(
             cast(DimensionRecord, data_id.records["instrument"]).class_name, collection_prefix
         )
 
-    @staticmethod
-    def _from_cls_name(cls_name: str, collection_prefix: str | None = None) -> Instrument:
+    @classmethod
+    def _from_cls_name(cls, cls_name: str, collection_prefix: str | None = None) -> Self:
         """Instantiate an `Instrument` object type name.
 
         This just provides common error-handling for `fromName` and
         `from_data_id`
 
         Parameters
         ----------
@@ -301,17 +302,18 @@
         Raises
         ------
         TypeError
             Raised if the class name retrieved is not a string or the imported
             symbol is not an `Instrument` subclass.
         """
         instrument_cls: type = doImportType(cls_name)
-        if not issubclass(instrument_cls, Instrument):
+        if not issubclass(instrument_cls, cls):
             raise TypeError(
-                f"{instrument_cls!r}, obtained from importing {cls_name}, is not an Instrument subclass."
+                f"{instrument_cls!r}, obtained from importing {cls_name}, is not a subclass "
+                f"of {get_full_type_name(cls)}."
             )
         return instrument_cls(collection_prefix=collection_prefix)
 
     @staticmethod
     def importAll(registry: Registry) -> None:
         """Import all the instruments known to this registry.
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_observation_dimension_packer.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_observation_dimension_packer.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_quantumContext.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_quantumContext.py`

 * *Files 1% similar despite different names*

```diff
@@ -344,15 +344,16 @@
             should then correspond to either a list of object or a single
             object depending of the type of the corresponding attribute on
             dataset. I.e. if ``dataset.calexp`` is
             ``[datasetRef1, datasetRef2]`` then ``values.calexp`` should be
             ``[calexp1, calexp2]``. Like wise if there is a single ref, then
             only a single object need be passed. The same restriction applies
             if dataset is directly a `list` of `~lsst.daf.butler.DatasetRef`
-            or a single `~lsst.daf.butler.DatasetRef`.
+            or a single `~lsst.daf.butler.DatasetRef`. If ``values.NAME`` is
+            None, no output is written.
         dataset : `OutputQuantizedConnection` or `list`[`DatasetRef`] \
                 or `DatasetRef`
             This argument may either be an `InputQuantizedConnection` which
             describes all the inputs of a quantum, a list of
             `lsst.daf.butler.DatasetRef`, or a single
             `lsst.daf.butler.DatasetRef`. The function will get and return
             the corresponding datasets from the butler.
@@ -367,15 +368,16 @@
         if isinstance(dataset, OutputQuantizedConnection):
             if not isinstance(values, Struct):
                 raise ValueError(
                     "dataset is a OutputQuantizedConnection, a Struct with corresponding"
                     " attributes must be passed as the values to put"
                 )
             for name, refs in dataset:
-                valuesAttribute = getattr(values, name)
+                if (valuesAttribute := getattr(values, name, None)) is None:
+                    continue
                 if isinstance(refs, list | tuple):
                     if len(refs) != len(valuesAttribute):
                         raise ValueError(f"There must be a object to put for every Dataset ref in {name}")
                     for i, ref in enumerate(refs):
                         self._put(valuesAttribute[i], ref)
                 else:
                     self._put(valuesAttribute, refs)
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/_task_metadata.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/_task_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 import itertools
 import numbers
 import sys
 from collections.abc import Collection, Iterator, Mapping, Sequence
 from typing import Any, Protocol, TypeAlias, Union
 
-from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr
+from pydantic import BaseModel, ConfigDict, Field, StrictBool, StrictFloat, StrictInt, StrictStr
 
 # The types allowed in a Task metadata field are restricted
 # to allow predictable serialization.
 _ALLOWED_PRIMITIVE_TYPES = (str, float, int, bool)
 
 # Note that '|' syntax for unions doesn't work when we have to use a string
 # literal (and we do since it's recursive and not an annotation).
@@ -119,14 +119,18 @@
         topLevelTaskName:subtaskName:subsubtaskName.itemName
 
     Metadata item key of a task (`itemName` above) must not contain `.`,
     which serves as a separator in full metadata keys and turns
     the value into sub-dictionary. Arbitrary hierarchies are supported.
     """
 
+    # Pipelines regularly generate NaN and Inf so these need to be
+    # supported even though that's a JSON extension.
+    model_config = ConfigDict(ser_json_inf_nan="constants")
+
     scalars: dict[str, StrictFloat | StrictInt | StrictBool | StrictStr] = Field(default_factory=dict)
     arrays: dict[str, list[StrictFloat] | list[StrictInt] | list[StrictBool] | list[StrictStr]] = Field(
         default_factory=dict
     )
     metadata: dict[str, "TaskMetadata"] = Field(default_factory=dict)
 
     @classmethod
@@ -653,14 +657,18 @@
             """See `pydantic.BaseModel.copy`."""
             return super().copy(*args, **kwargs)
 
         def model_dump(self, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_dump`."""
             return super().model_dump(*args, **kwargs)
 
+        def model_dump_json(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_dump_json`."""
+            return super().model_dump(*args, **kwargs)
+
         def model_copy(self, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_copy`."""
             return super().model_copy(*args, **kwargs)
 
         @classmethod
         def model_json_schema(cls, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_json_schema`."""
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 """The standard, general-purpose implementation of the QuantumGraph-generation
 algorithm.
 """
 
 from __future__ import annotations
 
-__all__ = ("AllDimensionsQuantumGraphBuilder",)
+__all__ = ("AllDimensionsQuantumGraphBuilder", "DatasetQueryConstraintVariant")
 
 import dataclasses
 from collections.abc import Iterator, Mapping
 from contextlib import contextmanager
 from typing import TYPE_CHECKING, Any, final
 
 from lsst.daf.butler.registry import MissingDatasetTypeError
@@ -67,15 +67,15 @@
     Parameters
     ----------
     pipeline_graph : `.pipeline_graph.PipelineGraph`
         Pipeline to build a `QuantumGraph` from, as a graph.  Will be resolved
         in-place with the given butler (any existing resolution is ignored).
     butler : `lsst.daf.butler.Butler`
         Client for the data repository.  Should be read-only.
-    where : `str`
+    where : `str`, optional
         Butler expression language constraint to apply to all data IDs.
     dataset_query_constraint : `DatasetQueryConstraintVariant`, optional
         Specification of which overall-input datasets should be used to
         constrain the initial data ID queries.  Not including an important
         constraint can result in catastrophically large query results that take
         too long to process, while including too many makes the query much more
         complex, increasing the chances that the database will choose a bad
@@ -103,15 +103,15 @@
     """
 
     def __init__(
         self,
         pipeline_graph: PipelineGraph,
         butler: Butler,
         *,
-        where: str,
+        where: str = "",
         dataset_query_constraint: DatasetQueryConstraintVariant = DatasetQueryConstraintVariant.ALL,
         bind: Mapping[str, Any] | None = None,
         **kwargs: Any,
     ):
         super().__init__(pipeline_graph, butler, **kwargs)
         self.where = where
         self.dataset_query_constraint = dataset_query_constraint
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/automatic_connection_constants.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/automatic_connection_constants.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/__init__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/cmd/commands.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/__init__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/arguments.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/cli/opt/options.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/config.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/config.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/configOverrides.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connectionTypes.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/connectionTypes.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 
 __all__ = ["InitInput", "InitOutput", "Input", "PrerequisiteInput", "Output", "BaseConnection"]
 
 import dataclasses
 from collections.abc import Callable, Iterable, Sequence
 from typing import ClassVar
 
+from deprecated.sphinx import deprecated as deprecated_sphinx  # avoid clash with BaseConnection.deprecated
 from lsst.daf.butler import DataCoordinate, DatasetRef, DatasetType, DimensionUniverse, Registry, StorageClass
 from lsst.utils.introspection import find_outside_stacklevel
 
 
 @dataclasses.dataclass(frozen=True)
 class BaseConnection:
     """Base class used for declaring `PipelineTask` connections.
@@ -101,14 +102,20 @@
         try:
             return inst.allConnections[self.varName]
         except KeyError:
             raise AttributeError(
                 f"Connection {self.varName!r} of {klass.__name__} has been removed."
             ) from None
 
+    # TODO: remove on DM-40443.
+    @deprecated_sphinx(
+        reason="Deprecated in favor of PipelineGraph, and will be removed after v27.",
+        version="27.0",
+        category=FutureWarning,
+    )
     def makeDatasetType(
         self, universe: DimensionUniverse, parentStorageClass: StorageClass | str | None = None
     ) -> DatasetType:
         """Construct a true `~lsst.daf.butler.DatasetType` instance with
         normalized dimensions.
 
         Parameters
@@ -165,14 +172,20 @@
         if isinstance(self.dimensions, str):
             raise TypeError(
                 "Dimensions must be iterable of dimensions, got str, possibly omitted trailing comma"
             )
         if not isinstance(self.dimensions, Iterable):
             raise TypeError("Dimensions must be iterable of dimensions")
 
+    # TODO: remove on DM-40443.
+    @deprecated_sphinx(
+        reason="Deprecated in favor of PipelineGraph, and will be removed after v27.",
+        version="27.0",
+        category=FutureWarning,
+    )
     def makeDatasetType(
         self, universe: DimensionUniverse, parentStorageClass: StorageClass | str | None = None
     ) -> DatasetType:
         """Construct a true `~lsst.daf.butler.DatasetType` instance with
         normalized dimensions.
 
         Parameters
@@ -294,26 +307,35 @@
         used to make QuantumGraph generation faster by avoiding redundant
         datasets, and in certain cases it can (along with careful attention to
         which tasks are included in the same QuantumGraph) be used to work
         around the QuantumGraph generation algorithm's inflexible handling of
         spatial overlaps.  This option has no effect when the connection is not
         an overall input of the pipeline (or subset thereof) for which a graph
         is being created, and it never affects the ordering of quanta.
+    deferBinding : `bool`, optional
+        If `True`, the dataset will not be automatically included in
+        the pipeline graph, ``deferGraphConstraint`` is implied.
+        The custom QuantumGraphBuilder is required to bind it and add a
+        corresponding edge to the pipeline graph.
+        This option allows to have the same dataset type as both
+        input and output of a quantum.
 
     Raises
     ------
     TypeError
         Raised if ``minimum`` is greater than one but ``multiple=False``.
     NotImplementedError
         Raised if ``minimum`` is zero for a regular `Input` connection; this
         is not currently supported by our QuantumGraph generation algorithm.
     """
 
     deferGraphConstraint: bool = False
 
+    deferBinding: bool = False
+
     _connection_type_set: ClassVar[str] = "inputs"
 
     def __post_init__(self) -> None:
         super().__post_init__()
         if self.minimum == 0:
             raise TypeError(f"Cannot set minimum={self.minimum} for regular input.")
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/connections.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,14 +35,15 @@
     "DeferredDatasetRef",
     "InputQuantizedConnection",
     "OutputQuantizedConnection",
     "PipelineTaskConnections",
     "ScalarError",
     "iterConnections",
     "ScalarError",
+    "QuantizedConnection",
 ]
 
 import dataclasses
 import itertools
 import string
 import warnings
 from collections import UserDict
@@ -748,75 +749,66 @@
         ----------
         quantum : `lsst.daf.butler.Quantum`
             Quantum object which defines the inputs and outputs for a given
             unit of processing.
 
         Returns
         -------
-        retVal : `tuple` of (`InputQuantizedConnection`,
-            `OutputQuantizedConnection`) Namespaces mapping attribute names
+        retVal : `tuple` of (`InputQuantizedConnection`, \
+                `OutputQuantizedConnection`)
+            Namespaces mapping attribute names
             (identifiers of connections) to butler references defined in the
-            input `lsst.daf.butler.Quantum`.
+            input `~lsst.daf.butler.Quantum`.
         """
         inputDatasetRefs = InputQuantizedConnection()
         outputDatasetRefs = OutputQuantizedConnection()
-        # operate on a reference object and an iterable of names of class
-        # connection attributes
-        for refs, names in zip(
-            (inputDatasetRefs, outputDatasetRefs),
-            (itertools.chain(self.inputs, self.prerequisiteInputs), self.outputs),
-            strict=True,
-        ):
-            # get a name of a class connection attribute
-            for attributeName in names:
-                # get the attribute identified by name
-                attribute = getattr(self, attributeName)
-                # Branch if the attribute dataset type is an input
-                if attribute.name in quantum.inputs:
-                    # if the dataset is marked to load deferred, wrap it in a
-                    # DeferredDatasetRef
-                    quantumInputRefs: list[DatasetRef] | list[DeferredDatasetRef]
-                    if attribute.deferLoad:
-                        quantumInputRefs = [
-                            DeferredDatasetRef(datasetRef=ref) for ref in quantum.inputs[attribute.name]
-                        ]
-                    else:
-                        quantumInputRefs = list(quantum.inputs[attribute.name])
-                    # Unpack arguments that are not marked multiples (list of
-                    # length one)
-                    if not attribute.multiple:
-                        if len(quantumInputRefs) > 1:
-                            raise ScalarError(
-                                "Received multiple datasets "
-                                f"{', '.join(str(r.dataId) for r in quantumInputRefs)} "
-                                f"for scalar connection {attributeName} "
-                                f"({quantumInputRefs[0].datasetType.name}) "
-                                f"of quantum for {quantum.taskName} with data ID {quantum.dataId}."
-                            )
-                        if len(quantumInputRefs) == 0:
-                            continue
-                        setattr(refs, attributeName, quantumInputRefs[0])
-                    else:
-                        # Add to the QuantizedConnection identifier
-                        setattr(refs, attributeName, quantumInputRefs)
-                # Branch if the attribute dataset type is an output
-                elif attribute.name in quantum.outputs:
-                    value = quantum.outputs[attribute.name]
-                    # Unpack arguments that are not marked multiples (list of
-                    # length one)
-                    if not attribute.multiple:
-                        setattr(refs, attributeName, value[0])
-                    else:
-                        setattr(refs, attributeName, value)
-                # Specified attribute is not in inputs or outputs dont know how
-                # to handle, throw
-                else:
-                    raise ValueError(
-                        f"Attribute with name {attributeName} has no counterpart in input quantum"
+
+        # populate inputDatasetRefs from quantum inputs
+        for attributeName in itertools.chain(self.inputs, self.prerequisiteInputs):
+            # get the attribute identified by name
+            attribute = getattr(self, attributeName)
+            # if the dataset is marked to load deferred, wrap it in a
+            # DeferredDatasetRef
+            quantumInputRefs: list[DatasetRef] | list[DeferredDatasetRef]
+            if attribute.deferLoad:
+                quantumInputRefs = [
+                    DeferredDatasetRef(datasetRef=ref) for ref in quantum.inputs[attribute.name]
+                ]
+            else:
+                quantumInputRefs = list(quantum.inputs[attribute.name])
+            # Unpack arguments that are not marked multiples (list of
+            # length one)
+            if not attribute.multiple:
+                if len(quantumInputRefs) > 1:
+                    raise ScalarError(
+                        "Received multiple datasets "
+                        f"{', '.join(str(r.dataId) for r in quantumInputRefs)} "
+                        f"for scalar connection {attributeName} "
+                        f"({quantumInputRefs[0].datasetType.name}) "
+                        f"of quantum for {quantum.taskName} with data ID {quantum.dataId}."
                     )
+                if len(quantumInputRefs) == 0:
+                    continue
+                setattr(inputDatasetRefs, attributeName, quantumInputRefs[0])
+            else:
+                # Add to the QuantizedConnection identifier
+                setattr(inputDatasetRefs, attributeName, quantumInputRefs)
+
+        # populate outputDatasetRefs from quantum outputs
+        for attributeName in self.outputs:
+            # get the attribute identified by name
+            attribute = getattr(self, attributeName)
+            value = quantum.outputs[attribute.name]
+            # Unpack arguments that are not marked multiples (list of
+            # length one)
+            if not attribute.multiple:
+                setattr(outputDatasetRefs, attributeName, value[0])
+            else:
+                setattr(outputDatasetRefs, attributeName, value)
+
         return inputDatasetRefs, outputDatasetRefs
 
     def adjustQuantum(
         self,
         inputs: dict[str, tuple[BaseInput, Collection[DatasetRef]]],
         outputs: dict[str, tuple[Output, Collection[DatasetRef]]],
         label: str,
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/executionButlerBuilder.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/executionButlerBuilder.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/execution_reports.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/execution_reports.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,19 +32,18 @@
 import logging
 import uuid
 from collections.abc import Iterable, Mapping
 from typing import Any
 
 import networkx
 import yaml
-from lsst.daf.butler import Butler, DataCoordinate, DatasetRef
+from lsst.daf.butler import Butler, DataCoordinate, DatasetRef, Quantum
 from lsst.resources import ResourcePathExpression
 
-from .graph import QuantumGraph, QuantumNode
-from .pipeline import PipelineDatasetTypes
+from .graph import QuantumGraph
 
 
 @dataclasses.dataclass
 class DatasetTypeExecutionReport:
     """A report on the number of produced datasets as well as the status of
     missing datasets based on metadata.
 
@@ -122,26 +121,29 @@
     output_datasets: dict[str, DatasetTypeExecutionReport] = dataclasses.field(default_factory=dict)
     """Missing and produced outputs of each `~lsst.daf.butler.DatasetType`
     (`dict`).
     """
 
     def inspect_quantum(
         self,
-        quantum_node: QuantumNode,
+        quantum_id: uuid.UUID,
+        quantum: Quantum,
         status_graph: networkx.DiGraph,
         refs: Mapping[str, Mapping[uuid.UUID, DatasetRef]],
         metadata_name: str,
         log_name: str,
     ) -> None:
         """Inspect a quantum of a quantum graph and ascertain the status of
         each associated data product.
 
         Parameters
         ----------
-        quantum_node : `QuantumNode`
+        quantum_id : `uuid.UUID`
+            Unique identifier for the quantum to inspect.
+        quantum : `Quantum`
             The specific node of the quantum graph to be inspected.
         status_graph : `networkx.DiGraph`
             The quantum graph produced by
             `QuantumGraphExecutionReport.make_reports` which steps through the
             quantum graph of a run and logs the status of each quantum.
         refs : `~collections.abc.Mapping` [ `str`,\
                 `~collections.abc.Mapping` [ `uuid.UUID`,\
@@ -153,35 +155,34 @@
         log_name : `str`
             The name of the log files for the node.
 
         See Also
         --------
         QuantumGraphExecutionReport.make_reports : Make reports.
         """
-        quantum = quantum_node.quantum
         (metadata_ref,) = quantum.outputs[metadata_name]
         (log_ref,) = quantum.outputs[log_name]
         blocked = False
         if metadata_ref.id not in refs[metadata_name]:
             if any(
                 status_graph.nodes[upstream_quantum_id]["failed"]
-                for upstream_dataset_id in status_graph.predecessors(quantum_node.nodeId)
+                for upstream_dataset_id in status_graph.predecessors(quantum_id)
                 for upstream_quantum_id in status_graph.predecessors(upstream_dataset_id)
             ):
                 assert quantum.dataId is not None
-                self.blocked[quantum_node.nodeId] = quantum.dataId
+                self.blocked[quantum_id] = quantum.dataId
                 blocked = True
             else:
-                self.failed[quantum_node.nodeId] = log_ref
+                self.failed[quantum_id] = log_ref
                 # note: log_ref may or may not actually exist
             failed = True
         else:
             failed = False
             self.n_succeeded += 1
-        status_graph.nodes[quantum_node.nodeId]["failed"] = failed
+        status_graph.nodes[quantum_id]["failed"] = failed
 
         # Now, loop over the datasets to make a DatasetTypeExecutionReport.
         for output_ref in itertools.chain.from_iterable(quantum.outputs.values()):
             if output_ref == metadata_ref or output_ref == log_ref:
                 continue
             if (dataset_type_report := self.output_datasets.get(output_ref.datasetType.name)) is None:
                 dataset_type_report = DatasetTypeExecutionReport()
@@ -193,53 +194,76 @@
                     else:
                         dataset_type_report.failed.add(output_ref)
                 else:
                     dataset_type_report.not_produced.add(output_ref)
             else:
                 dataset_type_report.n_produced += 1
 
-    def to_summary_dict(self, butler: Butler, do_store_logs: bool = True) -> dict[str, Any]:
+    def to_summary_dict(
+        self, butler: Butler, do_store_logs: bool = True, human_readable: bool = False
+    ) -> dict[str, Any]:
         """Summarize the results of the TaskExecutionReport in a dictionary.
 
         Parameters
         ----------
         butler : `lsst.daf.butler.Butler`
             The Butler used for this report.
         do_store_logs : `bool`
             Store the logs in the summary dictionary.
+        human_readable : `bool`
+            Store more human-readable information to be printed out to the
+            command-line.
 
         Returns
         -------
         summary_dict : `dict`
             A dictionary containing:
 
             - outputs: A dictionary summarizing the
               DatasetTypeExecutionReport for each DatasetType associated with
               the task
             - failed_quanta: A dictionary of quanta which failed and their
               dataIDs by quantum graph node id
             - n_quanta_blocked: The number of quanta which failed due to
               upstream failures.
             - n_succeded: The number of quanta which succeeded.
+
+            And possibly, if human-readable is passed:
+
+            - errors: A dictionary of data ids associated with each error
+              message. If `human-readable` and `do_store_logs`, this is stored
+              here. Otherwise, if `do_store_logs`, it is stored in
+              `failed_quanta` keyed by the quantum graph node id.
         """
         failed_quanta = {}
         for node_id, log_ref in self.failed.items():
-            quantum_info: dict[str, Any] = {"data_id": dict(log_ref.dataId.required)}
+            data_ids = dict(log_ref.dataId.required)
+            quantum_info: dict[str, Any] = {"data_id": data_ids}
             if do_store_logs:
                 try:
                     log = butler.get(log_ref)
                 except LookupError:
                     quantum_info["error"] = []
                 except FileNotFoundError:
                     quantum_info["error"] = None
                 else:
                     quantum_info["error"] = [
                         record.message for record in log if record.levelno >= logging.ERROR
                     ]
-            failed_quanta[str(node_id)] = quantum_info
+            if human_readable:
+                failed_quanta["data_id"] = data_ids
+                return {
+                    "outputs": {name: r.to_summary_dict() for name, r in self.output_datasets.items()},
+                    "failed_quanta": failed_quanta,
+                    "n_quanta_blocked": len(self.blocked),
+                    "n_succeeded": self.n_succeeded,
+                    "errors": quantum_info,
+                }
+            else:
+                failed_quanta[str(node_id)] = quantum_info
         return {
             "outputs": {name: r.to_summary_dict() for name, r in self.output_datasets.items()},
             "failed_quanta": failed_quanta,
             "n_quanta_blocked": len(self.blocked),
             "n_succeeded": self.n_succeeded,
         }
 
@@ -270,33 +294,38 @@
     TaskExecutionReport : A task report.
     DatasetTypeExecutionReport : A dataset type report.
     """
 
     tasks: dict[str, TaskExecutionReport] = dataclasses.field(default_factory=dict)
     """A dictionary of TaskExecutionReports by task label (`dict`)."""
 
-    def to_summary_dict(self, butler: Butler, do_store_logs: bool = True) -> dict[str, Any]:
+    def to_summary_dict(
+        self, butler: Butler, do_store_logs: bool = True, human_readable: bool = False
+    ) -> dict[str, Any]:
         """Summarize the results of the `QuantumGraphExecutionReport` in a
         dictionary.
 
         Parameters
         ----------
         butler : `lsst.daf.butler.Butler`
             The Butler used for this report.
         do_store_logs : `bool`
             Store the logs in the summary dictionary.
+        human_readable : `bool`
+            Store more human-readable information to be printed out to the
+            command-line.
 
         Returns
         -------
         summary_dict : `dict`
             A dictionary containing a summary of a `TaskExecutionReport` for
             each task in the quantum graph.
         """
         return {
-            task: report.to_summary_dict(butler, do_store_logs=do_store_logs)
+            task: report.to_summary_dict(butler, do_store_logs=do_store_logs, human_readable=human_readable)
             for task, report in self.tasks.items()
         }
 
     def write_summary_yaml(self, butler: Butler, filename: str, do_store_logs: bool = True) -> None:
         """Take the dictionary from
         `QuantumGraphExecutionReport.to_summary_dict` and store its contents in
         a yaml file.
@@ -347,61 +376,45 @@
         if not isinstance(graph, QuantumGraph):
             qg = QuantumGraph.loadUri(graph)
         else:
             qg = graph
         assert qg.metadata is not None, "Saved QGs always have metadata."
         collection = qg.metadata["output_run"]
         report = cls()
-        task_defs = list(qg.iterTaskGraph())
-        pipeline_dataset_types = PipelineDatasetTypes.fromPipeline(task_defs, registry=butler.registry)
-        for dataset_type in itertools.chain(
-            pipeline_dataset_types.initIntermediates,
-            pipeline_dataset_types.initOutputs,
-            pipeline_dataset_types.intermediates,
-            pipeline_dataset_types.outputs,
-        ):
-            if (component := dataset_type.component()) is not None:
-                # Work around the fact that component support has been phased
-                # out of daf_butler queries but not pipe_base's QGs.  This
-                # should go away on DM-40441.
-                parent_dataset_type = dataset_type.makeCompositeDatasetType()
-                refs[dataset_type.name] = {
-                    ref.id: ref.makeComponentRef(component)
-                    for ref in butler.registry.queryDatasets(
-                        parent_dataset_type.name, collections=collection, findFirst=False
-                    )
-                }
-            else:
-                refs[dataset_type.name] = {
-                    ref.id: ref
-                    for ref in butler.registry.queryDatasets(
-                        dataset_type.name, collections=collection, findFirst=False
-                    )
-                }
-        for task_def in qg.iterTaskGraph():
-            for node in qg.getNodesForTask(task_def):
-                status_graph.add_node(node.nodeId)
-                for ref in itertools.chain.from_iterable(node.quantum.outputs.values()):
-                    status_graph.add_edge(node.nodeId, ref.id)
-                for ref in itertools.chain.from_iterable(node.quantum.inputs.values()):
-                    status_graph.add_edge(ref.id, node.nodeId)
+        for dataset_type_node in qg.pipeline_graph.dataset_types.values():
+            if qg.pipeline_graph.producer_of(dataset_type_node.name) is None:
+                continue
+            refs[dataset_type_node.name] = {
+                ref.id: ref
+                for ref in butler.registry.queryDatasets(
+                    dataset_type_node.name, collections=collection, findFirst=False
+                )
+            }
+        for task_node in qg.pipeline_graph.tasks.values():
+            for quantum_id, quantum in qg.get_task_quanta(task_node.label).items():
+                status_graph.add_node(quantum_id)
+                for ref in itertools.chain.from_iterable(quantum.outputs.values()):
+                    status_graph.add_edge(quantum_id, ref.id)
+                for ref in itertools.chain.from_iterable(quantum.inputs.values()):
+                    status_graph.add_edge(ref.id, quantum_id)
 
-        for task_def in qg.iterTaskGraph():
+        for task_node in qg.pipeline_graph.tasks.values():
             task_report = TaskExecutionReport()
-            if task_def.logOutputDatasetName is None:
+            if task_node.log_output is None:
                 raise RuntimeError("QG must have log outputs to use execution reports.")
-            for node in qg.getNodesForTask(task_def):
+            for quantum_id, quantum in qg.get_task_quanta(task_node.label).items():
                 task_report.inspect_quantum(
-                    node,
+                    quantum_id,
+                    quantum,
                     status_graph,
                     refs,
-                    metadata_name=task_def.metadataDatasetName,
-                    log_name=task_def.logOutputDatasetName,
+                    metadata_name=task_node.metadata_output.dataset_type_name,
+                    log_name=task_node.log_output.dataset_type_name,
                 )
-            report.tasks[task_def.label] = task_report
+            report.tasks[task_node.label] = task_report
         return report
 
     def __str__(self) -> str:
         return "\n".join(f"{tasklabel}:{report}" for tasklabel, report in self.tasks.items())
 
 
 def lookup_quantum_data_id(
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/formatters/pexConfig.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/formatters/pexConfig.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_implDetails.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/_implDetails.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_loadHelpers.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/_loadHelpers.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/_versionDeserializers.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/_versionDeserializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -653,14 +653,15 @@
         newGraph._taskGraph = datasetDict.makeNetworkXGraph()
         newGraph._connectedQuanta = graph
         newGraph._initInputRefs = initInputRefs
         newGraph._initOutputRefs = initOutputRefs
         newGraph._globalInitOutputRefs = self.infoMappings.globalInitOutputRefs
         newGraph._registryDatasetTypes = self.infoMappings.registryDatasetTypes
         newGraph._universe = universe
+        newGraph._pipeline_graph = None
         return newGraph
 
 
 DESERIALIZER_MAP: dict[int, type[DeserializerBase]] = {
     1: DeserializerV1,
     2: DeserializerV2,
     3: DeserializerV3,
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/graph.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/graph.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,22 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ("QuantumGraph", "IncompatibleGraphError")
 
+import datetime
+import getpass
 import io
 import json
 import lzma
 import os
 import struct
+import sys
 import time
 import uuid
 from collections import defaultdict, deque
 from collections.abc import Generator, Iterable, Iterator, Mapping, MutableMapping
 from itertools import chain
 from types import MappingProxyType
 from typing import Any, BinaryIO, TypeVar
@@ -49,21 +52,24 @@
     DimensionRecordsAccumulator,
     DimensionUniverse,
     Quantum,
 )
 from lsst.daf.butler.persistence_context import PersistenceContextVars
 from lsst.resources import ResourcePath, ResourcePathExpression
 from lsst.utils.introspection import get_full_type_name
+from lsst.utils.packages import Packages
 from networkx.drawing.nx_agraph import write_dot
 
 from ..connections import iterConnections
 from ..pipeline import TaskDef
+from ..pipeline_graph import PipelineGraph
 from ._implDetails import DatasetTypeName, _DatasetTracker
 from ._loadHelpers import LoadHelper
 from ._versionDeserializers import DESERIALIZER_MAP
+from .graphSummary import QgraphSummary, QgraphTaskSummary
 from .quantumNode import BuildId, QuantumNode
 
 _T = TypeVar("_T", bound="QuantumGraph")
 
 # modify this constant any time the on disk representation of the save file
 # changes, and update the load helpers to behave properly for each version.
 SAVE_VERSION = 3
@@ -170,15 +176,21 @@
         initOutputs: Mapping[TaskDef, Iterable[DatasetRef]] | None = None,
         globalInitOutputs: Iterable[DatasetRef] | None = None,
         registryDatasetTypes: Iterable[DatasetType] | None = None,
     ) -> None:
         """Build the graph that is used to store the relation between tasks,
         and the graph that holds the relations between quanta
         """
-        self._metadata = metadata
+        # Save packages to metadata
+        self._metadata = dict(metadata) if metadata is not None else {}
+        self._metadata["packages"] = Packages.fromSystem()
+        self._metadata["user"] = getpass.getuser()
+        self._metadata["time"] = f"{datetime.datetime.now()}"
+        self._metadata["full_command"] = " ".join(sys.argv)
+
         self._buildId = _buildId if _buildId is not None else BuildId(f"{time.time()}-{os.getpid()}")
         # Data structure used to identify relations between
         # DatasetTypeName -> TaskDef.
         self._datasetDict = _DatasetTracker(createInverse=True)
 
         # Temporary graph that will have dataset UUIDs (as raw bytes) and
         # QuantumNode objects as nodes; will be collapsed down to just quanta
@@ -283,14 +295,55 @@
         if initOutputs is not None:
             self._initOutputRefs = {taskDef: list(refs) for taskDef, refs in initOutputs.items()}
         if globalInitOutputs is not None:
             self._globalInitOutputRefs = list(globalInitOutputs)
         if registryDatasetTypes is not None:
             self._registryDatasetTypes = list(registryDatasetTypes)
 
+        # PipelineGraph is current constructed on first use.
+        # TODO DM-40442: use PipelineGraph instead of TaskDef
+        # collections.
+        self._pipeline_graph: PipelineGraph | None = None
+
+    @property
+    def pipeline_graph(self) -> PipelineGraph:
+        """A graph representation of the tasks and dataset types in the quantum
+        graph.
+        """
+        if self._pipeline_graph is None:
+            # Construct into a temporary for strong exception safety.
+            pipeline_graph = PipelineGraph()
+            for task_def in self._taskToQuantumNode.keys():
+                pipeline_graph.add_task(
+                    task_def.label, task_def.taskClass, task_def.config, connections=task_def.connections
+                )
+            dataset_types = {dataset_type.name: dataset_type for dataset_type in self._registryDatasetTypes}
+            pipeline_graph.resolve(dimensions=self._universe, dataset_types=dataset_types)
+            self._pipeline_graph = pipeline_graph
+        return self._pipeline_graph
+
+    def get_task_quanta(self, label: str) -> Mapping[uuid.UUID, Quantum]:
+        """Return the quanta associated with the given task label.
+
+        Parameters
+        ----------
+        label : `str`
+            Task label.
+
+        Returns
+        -------
+        quanta : `~collections.abc.Mapping` [ uuid.UUID, `Quantum` ]
+            Mapping from quantum ID to quantum.  Empty if ``label`` does not
+            correspond to a task in this graph.
+        """
+        task_def = self.findTaskDefByLabel(label)
+        if not task_def:
+            return {}
+        return {node.nodeId: node.quantum for node in self.getNodesForTask(task_def)}
+
     @property
     def taskGraph(self) -> nx.DiGraph:
         """A graph representing the relations between the tasks inside
         the quantum graph (`networkx.DiGraph`).
         """
         return self._taskGraph
 
@@ -747,22 +800,20 @@
         buffer = self._buildSaveObject()
         path = ResourcePath(uri)
         if path.getExtension() not in (".qgraph"):
             raise TypeError(f"Can currently only save a graph in qgraph format not {uri}")
         path.write(buffer)  # type: ignore  # Ignore because bytearray is safe to use in place of bytes
 
     @property
-    def metadata(self) -> MappingProxyType[str, Any] | None:
+    def metadata(self) -> MappingProxyType[str, Any]:
         """Extra data carried with the graph (mapping [`str`] or `None`).
 
         The mapping is a dynamic view of this object's metadata. Values should
         be able to be serialized in JSON.
         """
-        if self._metadata is None:
-            return None
         return MappingProxyType(self._metadata)
 
     def initInputRefs(self, taskDef: TaskDef) -> list[DatasetRef] | None:
         """Return DatasetRefs for a given task InitInputs.
 
         Parameters
         ----------
@@ -943,15 +994,15 @@
         # node map is a list because json does not accept mapping keys that
         # are not strings, so we store a list of key, value pairs that will
         # be converted to a mapping on load
         nodeMap = []
         taskDefMap = {}
         headerData: dict[str, Any] = {}
 
-        # Store the QauntumGraph BuildId, this will allow validating BuildIds
+        # Store the QuantumGraph BuildId, this will allow validating BuildIds
         # at load time, prior to loading any QuantumNodes. Name chosen for
         # unlikely conflicts.
         headerData["GraphBuildID"] = self.graphID
         headerData["Metadata"] = self._metadata
 
         # Store the universe this graph was created with
         universeConfig = self._universe.dimensionConfig
@@ -1242,19 +1293,17 @@
             task_def: list(_update_intermediate_refs(refs, run, dataset_id_map))
             for task_def, refs in self._initInputRefs.items()
         }
 
         if update_graph_id:
             self._buildId = BuildId(f"{time.time()}-{os.getpid()}")
 
-        # Update metadata if present.
-        if self._metadata is not None and metadata_key is not None:
-            metadata = dict(self._metadata)
-            metadata[metadata_key] = run
-            self._metadata = metadata
+        # Update run if given.
+        if metadata_key is not None:
+            self._metadata[metadata_key] = run
 
     @property
     def graphID(self) -> BuildId:
         """The ID generated by the graph at construction time (`str`)."""
         return self._buildId
 
     @property
@@ -1317,7 +1366,40 @@
             if self.determineInputsToQuantumNode(node) != other.determineInputsToQuantumNode(node):
                 return False
             if self.determineOutputsOfQuantumNode(node) != other.determineOutputsOfQuantumNode(node):
                 return False
         if set(self.allDatasetTypes) != set(other.allDatasetTypes):
             return False
         return set(self.taskGraph) == set(other.taskGraph)
+
+    def getSummary(self) -> QgraphSummary:
+        """Create summary of graph.
+
+        Returns
+        -------
+        summary : `QgraphSummary`
+           Summary of QuantumGraph.
+        """
+        inCollection = self.metadata.get("input", None)
+        if isinstance(inCollection, str):
+            inCollection = [inCollection]
+        summary = QgraphSummary(
+            graphID=self.graphID,
+            cmdLine=self.metadata.get("full_command", None),
+            creationUTC=self.metadata.get("time", None),
+            inputCollection=inCollection,
+            outputCollection=self.metadata.get("output", None),
+            outputRun=self.metadata.get("output_run", None),
+        )
+        for q in self:
+            qts = summary.qgraphTaskSummaries.setdefault(
+                q.taskDef.label, QgraphTaskSummary(taskLabel=q.taskDef.label)
+            )
+            qts.numQuanta += 1
+
+            for k in q.quantum.inputs.keys():
+                qts.numInputs[k.name] += 1
+
+            for k in q.quantum.outputs.keys():
+                qts.numOutputs[k.name] += 1
+
+        return summary
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graph/quantumNode.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graph/quantumNode.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     DimensionRecordsAccumulator,
     DimensionUniverse,
     Quantum,
     SerializedQuantum,
 )
 
 from ..pipeline import TaskDef
+from ..pipeline_graph import PipelineGraph, TaskNode
 
 BuildId = NewType("BuildId", str)
 
 
 def _hashDsRef(ref: DatasetRef) -> int:
     return hash((ref.datasetType, ref.dataId))
 
@@ -97,14 +98,27 @@
     this node.
     """
     nodeId: uuid.UUID
     """The unique position of the node within the graph assigned at graph
     creation.
     """
 
+    @property
+    def task_node(self) -> TaskNode:
+        """Return the node object that represents this task in a pipeline
+        graph.
+        """
+        pipeline_graph = PipelineGraph()
+        return pipeline_graph.add_task(
+            self.taskDef.label,
+            self.taskDef.taskClass,
+            self.taskDef.config,
+            connections=self.taskDef.connections,
+        )
+
     __slots__ = ("quantum", "taskDef", "nodeId", "_precomputedHash")
 
     def __post_init__(self) -> None:
         # use setattr here to preserve the frozenness of the QuantumNode
         self._precomputedHash: int
         object.__setattr__(self, "_precomputedHash", hash((self.taskDef.label, self.quantum)))
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/graphBuilder.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/graphBuilder.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,32 +29,47 @@
 """
 
 from __future__ import annotations
 
 __all__ = ["GraphBuilder"]
 
 
+import warnings
 from collections.abc import Iterable, Mapping
 from typing import Any
 
+from deprecated.sphinx import deprecated
 from lsst.daf.butler import Butler, DataCoordinate, Datastore, Registry
 from lsst.daf.butler.registry.wildcards import CollectionWildcard
+from lsst.utils.introspection import find_outside_stacklevel
 
 from ._datasetQueryConstraints import DatasetQueryConstraintVariant
 from .all_dimensions_quantum_graph_builder import AllDimensionsQuantumGraphBuilder
 from .graph import QuantumGraph
 from .pipeline import Pipeline, TaskDef
 from .pipeline_graph import PipelineGraph
 
 # Re-exports for backwards-compatibility.
 from .quantum_graph_builder import GraphBuilderError  # noqa: F401
 from .quantum_graph_builder import OutputExistsError  # noqa: F401
 from .quantum_graph_builder import PrerequisiteMissingError  # noqa: F401
 
+# TODO: remove this module on DM-40443.
+warnings.warn(
+    "The graphBuilder module is deprecated in favor of quantum_graph_builder, and will be removed after v27.",
+    category=FutureWarning,
+    stacklevel=find_outside_stacklevel("lsst.pipe.base"),
+)
 
+
+@deprecated(
+    "Deprecated in favor of QuantumGraphBuilder and will be removed after v27.",
+    version="v27.0",
+    category=FutureWarning,
+)
 class GraphBuilder:
     """GraphBuilder class is responsible for building task execution graph from
     a Pipeline.
 
     Parameters
     ----------
     registry : `~lsst.daf.butler.Registry`
@@ -168,8 +183,8 @@
             output_run=run,
             skip_existing_in=self.skipExistingIn if self.skipExistingIn is not None else (),
             clobber=self.clobberOutputs,
             where=userQuery if userQuery is not None else "",
             dataset_query_constraint=datasetQueryConstraint,
             bind=bind,
         )
-        return qgb.build(metadata)
+        return qgb.build(metadata, attach_datastore_records=(self.datastore is not None))
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 from collections.abc import Callable, Generator, Iterable, Iterator, Mapping, Set
 from dataclasses import dataclass
 from types import MappingProxyType
 from typing import TYPE_CHECKING, ClassVar, cast
 
 # -----------------------------
 #  Imports for other modules --
+# -----------------------------
+from deprecated.sphinx import deprecated
 from lsst.daf.butler import DataCoordinate, DatasetType, DimensionUniverse, NamedValueSet, Registry
 from lsst.resources import ResourcePath, ResourcePathExpression
 from lsst.utils import doImportType
 from lsst.utils.introspection import get_full_type_name
 
 from . import automatic_connection_constants as acc
 from . import pipeline_graph, pipelineIR
@@ -76,19 +78,23 @@
 
 
 @dataclass
 class LabelSpecifier:
     """A structure to specify a subset of labels to load.
 
     This structure may contain a set of labels to be used in subsetting a
-    pipeline, or a beginning and end point. Beginning or end may be empty,
-    in which case the range will be a half open interval. Unlike python
-    iteration bounds, end bounds are *INCLUDED*. Note that range based
-    selection is not well defined for pipelines that are not linear in nature,
-    and correct behavior is not guaranteed, or may vary from run to run.
+    pipeline, or a beginning and end point. Beginning or end may be empty, in
+    which case the range will be a half open interval. Unlike python iteration
+    bounds, end bounds are *INCLUDED*.
+
+    There are multiple potential definitions of range-based slicing for graphs
+    that are not a simple linear sequence.  The definition used here is the
+    intersection of the tasks downstream of ``begin`` and the tasks upstream of
+    ``end``, i.e. tasks with no dependency relationship to a bounding task are
+    not included.
     """
 
     labels: set[str] | None = None
     begin: str | None = None
     end: str | None = None
 
     def __post_init__(self) -> None:
@@ -380,39 +386,28 @@
             # ordering. Use a dict for fast searching while preserving order.
             # Remove contracts so they do not fail in the expansion step. This
             # is needed because a user may only configure the tasks they intend
             # to run, which may cause some contracts to fail if they will later
             # be dropped
             pipeline = copy.deepcopy(self)
             pipeline._pipelineIR.contracts = []
-            labels = {taskdef.label: True for taskdef in pipeline.toExpandedPipeline()}
+            graph = pipeline.to_graph()
 
             # Verify the bounds are in the labels
-            if labelSpecifier.begin is not None:
-                if labelSpecifier.begin not in labels:
-                    raise ValueError(
-                        f"Beginning of range subset, {labelSpecifier.begin}, not found in pipeline definition"
-                    )
-            if labelSpecifier.end is not None:
-                if labelSpecifier.end not in labels:
-                    raise ValueError(
-                        f"End of range subset, {labelSpecifier.end}, not found in pipeline definition"
-                    )
+            if labelSpecifier.begin is not None and labelSpecifier.begin not in graph.tasks:
+                raise ValueError(
+                    f"Beginning of range subset, {labelSpecifier.begin}, not found in pipeline definition"
+                )
+            if labelSpecifier.end is not None and labelSpecifier.end not in graph.tasks:
+                raise ValueError(
+                    f"End of range subset, {labelSpecifier.end}, not found in pipeline definition"
+                )
 
-            labelSet = set()
-            for label in labels:
-                if labelSpecifier.begin is not None:
-                    if label != labelSpecifier.begin:
-                        continue
-                    else:
-                        labelSpecifier.begin = None
-                labelSet.add(label)
-                if labelSpecifier.end is not None and label == labelSpecifier.end:
-                    break
-        return Pipeline.fromIR(self._pipelineIR.subset_from_labels(labelSet, subsetCtrl))
+            labelSet = set(graph.tasks.between(labelSpecifier.begin, labelSpecifier.end))
+        return Pipeline.fromIR(self._pipelineIR.subset_from_labels(labelSet))
 
     @staticmethod
     def _parse_file_specifier(uri: ResourcePathExpression) -> tuple[ResourcePath, LabelSpecifier | None]:
         """Split appart a uri and any possible label subsets"""
         if isinstance(uri, str):
             # This is to support legacy pipelines during transition
             uri, num_replace = re.subn("[:](?!\\/\\/)", "#", uri)
@@ -598,14 +593,25 @@
             raise ValueError(f"Label {label} does not appear within the pipeline")
         for subset in self._pipelineIR.labeled_subsets.values():
             if label in subset.subset:
                 results.add(subset.label)
         return results
 
     @property
+    def task_labels(self) -> Set[str]:
+        """Labels of all tasks in the pipelines.
+
+        For simple pipelines with no imports, iteration over this set will
+        match the order in which tasks are defined in the pipeline file.  In
+        all other cases the order is unspecified but deterministic.  It is not
+        dependency-ordered (use ``to_graph().tasks.keys()`` for that).
+        """
+        return self._pipelineIR.tasks.keys()
+
+    @property
     def subsets(self) -> MappingProxyType[str, set]:
         """Returns a `MappingProxyType` where the keys are the labels of
         labeled subsets in the `Pipeline` and the values are the set of task
         labels contained within that subset.
         """
         return MappingProxyType(
             {label: subsetIr.subset for label, subsetIr in self._pipelineIR.labeled_subsets.items()}
@@ -859,14 +865,20 @@
                 label, subset.subset, subset.description if subset.description is not None else ""
             )
         graph.sort()
         if registry is not None:
             graph.resolve(registry)
         return graph
 
+    # TODO: remove on DM-40443.
+    @deprecated(
+        reason="Deprecated in favor of to_graph; will be removed after v27.",
+        version="v27.0",
+        category=FutureWarning,
+    )
     def toExpandedPipeline(self) -> Generator[TaskDef, None, None]:
         r"""Return a generator of `TaskDef`\s which can be used to create
         quantum graphs.
 
         Returns
         -------
         generator : generator of `TaskDef`
@@ -905,17 +917,29 @@
             getattr(taskClass, "_DefaultName", ""),
             taskIR.config,
             self._pipelineIR.parameters,
             label,
         )
         graph.add_task(label, taskClass, config)
 
+    # TODO: remove on DM-40443.
+    @deprecated(
+        reason="Deprecated in favor of to_graph; will be removed after v27.",
+        version="v27.0",
+        category=FutureWarning,
+    )
     def __iter__(self) -> Generator[TaskDef, None, None]:
         return self.toExpandedPipeline()
 
+    # TODO: remove on DM-40443.
+    @deprecated(
+        reason="Deprecated in favor of to_graph; will be removed after v27.",
+        version="v27.0",
+        category=FutureWarning,
+    )
     def __getitem__(self, item: str) -> TaskDef:
         # Making a whole graph and then making a TaskDef from that is pretty
         # backwards, but I'm hoping to deprecate this method shortly in favor
         # of making the graph explicitly and working with its node objects.
         graph = pipeline_graph.PipelineGraph()
         self._add_task_to_graph(item, graph)
         (result,) = graph._iter_task_defs()
@@ -928,25 +952,29 @@
         if not isinstance(other, Pipeline):
             return False
         elif self._pipelineIR == other._pipelineIR:
             # Shortcut: if the IR is the same, the expanded pipeline must be
             # the same as well.  But the converse is not true.
             return True
         else:
-            self_expanded = {td.label: (td.taskClass,) for td in self}
-            other_expanded = {td.label: (td.taskClass,) for td in other}
-            if self_expanded != other_expanded:
+            # Compare as much as we can (task classes and their edges).
+            if self.to_graph().diff_tasks(other.to_graph()):
                 return False
-        # After DM-27847, we should compare configuration here, or better,
-        # delegated to TaskDef.__eq__ after making that compare configurations.
+        # After DM-27847, we should compare configuration here.
         raise NotImplementedError(
             "Pipelines cannot be compared because config instances cannot be compared; see DM-27847."
         )
 
 
+# TODO: remove on DM-40443.
+@deprecated(
+    reason="TaskDatasetTypes has been replaced by PipelineGraph, and will be removed after v27.",
+    version="v27.0",
+    category=FutureWarning,
+)
 @dataclass(frozen=True)
 class TaskDatasetTypes:
     """An immutable struct that extracts and classifies the dataset types used
     by a `PipelineTask`.
     """
 
     initInputs: NamedValueSet[DatasetType]
@@ -1243,14 +1271,20 @@
             inputs=inputs,
             queryConstraints=queryConstraints,
             prerequisites=makeDatasetTypesSet("prerequisiteInputs", is_input=True),
             outputs=outputs,
         )
 
 
+# TODO: remove on DM-40443.
+@deprecated(
+    reason="PipelineDatasetTypes has been replaced by PipelineGraph, and will be removed after v27.",
+    version="v27.0",
+    category=FutureWarning,
+)
 @dataclass(frozen=True)
 class PipelineDatasetTypes:
     """An immutable struct that classifies the dataset types used in a
     `Pipeline`.
     """
 
     packagesDatasetName: ClassVar[str] = acc.PACKAGES_INIT_OUTPUT_NAME
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineIR.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipelineIR.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipelineTask.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipelineTask.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__init__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/__main__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/__main__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_dataset_types.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_dataset_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,19 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ("DatasetTypeNode",)
 
 import dataclasses
-from collections.abc import Collection
+from collections.abc import Callable, Collection
 from typing import TYPE_CHECKING, Any
 
 import networkx
-from lsst.daf.butler import DatasetRef, DatasetType, DimensionGroup, Registry, StorageClass
-from lsst.daf.butler.registry import MissingDatasetTypeError
+from lsst.daf.butler import DatasetRef, DatasetType, DimensionGroup, DimensionUniverse, StorageClass
 
 from ._exceptions import DuplicateOutputError
 from ._nodes import NodeKey, NodeType
 
 if TYPE_CHECKING:
     from ._edges import ReadEdge, WriteEdge
 
@@ -80,43 +79,47 @@
     """The edge to the task that produces this dataset type."""
 
     consuming_edges: Collection[ReadEdge]
     """The edges to tasks that consume this dataset type."""
 
     @classmethod
     def _from_edges(
-        cls, key: NodeKey, xgraph: networkx.MultiDiGraph, registry: Registry, previous: DatasetTypeNode | None
+        cls,
+        key: NodeKey,
+        xgraph: networkx.MultiDiGraph,
+        get_registered: Callable[[str], DatasetType | None],
+        dimensions: DimensionUniverse,
+        previous: DatasetTypeNode | None,
     ) -> DatasetTypeNode:
         """Construct a dataset type node from its edges.
 
         Parameters
         ----------
         key : `NodeKey`
             Named tuple that holds the dataset type and serves as the node
             object in the internal networkx graph.
         xgraph : `networkx.MultiDiGraph`
             The internal networkx graph.
-        registry : `lsst.daf.butler.Registry`
-            Registry client for the data repository.  Only used to get
-            dataset type definitions and the dimension universe.
+        get_registered : `~collections.abc.Callable`
+            Callable that takes a dataset type name and returns the
+            `DatasetType` registered in the data repository, or `None` if it is
+            not registered.
+        dimensions : `lsst.daf.butler.DimensionUniverse`
+            Definitions of all dimensions.
         previous : `DatasetTypeNode` or `None`
             Previous node for this dataset type.
 
         Returns
         -------
         node : `DatasetTypeNode`
             Node consistent with all edges pointing to it and the data
             repository.
         """
-        try:
-            dataset_type = registry.getDatasetType(key.name)
-            is_registered = True
-        except MissingDatasetTypeError:
-            dataset_type = None
-            is_registered = False
+        dataset_type = get_registered(key.name)
+        is_registered = dataset_type is not None
         if previous is not None and previous.dataset_type == dataset_type:
             # This node was already resolved (with exactly the same edges
             # contributing, since we clear resolutions when edges are added or
             # removed).  The only thing that might have changed was the
             # definition in the registry, and it didn't.
             return previous
         is_initial_query_constraint = True
@@ -134,28 +137,28 @@
             assert producing_edge is not None, "Should only be None if we never loop."
             if producer is not None:
                 raise DuplicateOutputError(
                     f"Dataset type {key.name!r} is produced by both {producing_edge.task_label!r} "
                     f"and {producer!r}."
                 )
             producer = producing_edge.task_label
-            dataset_type = producing_edge._resolve_dataset_type(dataset_type, universe=registry.dimensions)
+            dataset_type = producing_edge._resolve_dataset_type(dataset_type, universe=dimensions)
             is_prerequisite = False
             is_initial_query_constraint = False
         consuming_edge: ReadEdge
         consumers: list[str] = []
         consuming_edges = list(
             consuming_edge for _, _, consuming_edge in xgraph.out_edges(key, data="instance")
         )
         # Put edges that are not component datasets before any edges that are.
         consuming_edges.sort(key=lambda consuming_edge: consuming_edge.component is not None)
         for consuming_edge in consuming_edges:
             dataset_type, is_initial_query_constraint, is_prerequisite = consuming_edge._resolve_dataset_type(
                 current=dataset_type,
-                universe=registry.dimensions,
+                universe=dimensions,
                 is_initial_query_constraint=is_initial_query_constraint,
                 is_prerequisite=is_prerequisite,
                 is_registered=is_registered,
                 producer=producer,
                 consumers=consumers,
             )
             consumers.append(consuming_edge.task_label)
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_edges.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_edges.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ("Edge", "ReadEdge", "WriteEdge")
 
 from abc import ABC, abstractmethod
-from collections.abc import Mapping, Sequence
-from typing import Any, ClassVar, TypeVar
+from collections.abc import Callable, Mapping, Sequence
+from typing import Any, ClassVar, Self, TypeVar
 
 from lsst.daf.butler import DatasetRef, DatasetType, DimensionUniverse
 from lsst.daf.butler.registry import MissingDatasetTypeError
 from lsst.utils.classes import immutable
 
 from ..connectionTypes import BaseConnection
 from ._exceptions import ConnectionTypeConsistencyError, IncompatibleDatasetTypeError
@@ -190,33 +190,33 @@
             difference is in the task label or connection name (which are not
             checked).  Messages will use 'A' to refer to ``self`` and 'B' to
             refer to ``other``.
         """
         result = []
         if self.dataset_type_name != other.dataset_type_name:
             result.append(
-                f"{connection_type.capitalize()} {self.connection_name!r} has dataset type "
+                f"{connection_type.capitalize()} {self.task_label}.{self.connection_name} has dataset type "
                 f"{self.dataset_type_name!r} in A, but {other.dataset_type_name!r} in B."
             )
         if self.storage_class_name != other.storage_class_name:
             result.append(
-                f"{connection_type.capitalize()} {self.connection_name!r} has storage class "
+                f"{connection_type.capitalize()} {self.task_label}.{self.connection_name} has storage class "
                 f"{self.storage_class_name!r} in A, but {other.storage_class_name!r} in B."
             )
         if self.raw_dimensions != other.raw_dimensions:
             result.append(
-                f"{connection_type.capitalize()} {self.connection_name!r} has raw dimensions "
+                f"{connection_type.capitalize()} {self.task_label}.{self.connection_name} has raw dimensions "
                 f"{set(self.raw_dimensions)} in A, but {set(other.raw_dimensions)} in B "
                 "(differences in raw dimensions may not lead to differences in resolved dimensions, "
                 "but this cannot be checked without re-resolving the dataset type)."
             )
         if self.is_calibration != other.is_calibration:
             result.append(
-                f"{connection_type.capitalize()} {self.connection_name!r} is marked as a calibration "
-                f"{'in A but not in B' if self.is_calibration else 'in B but not in A'}."
+                f"{connection_type.capitalize()} {self.task_label}.{self.connection_name} is marked as a "
+                f"calibration {'in A but not in B' if self.is_calibration else 'in B but not in A'}."
             )
         return result
 
     @abstractmethod
     def adapt_dataset_type(self, dataset_type: DatasetType) -> DatasetType:
         """Transform the graph's definition of a dataset type (parent, with the
         registry or producer's storage class) to the one seen by this task.
@@ -257,14 +257,34 @@
         """
         return {
             "parent_dataset_type_name": self.parent_dataset_type_name,
             "storage_class_name": self.storage_class_name,
             "is_init": bool,
         }
 
+    @classmethod
+    def _unreduce(cls, kwargs: dict[str, Any]) -> Self:
+        """Unpickle an `Edge` instance."""
+        return cls(**kwargs)
+
+    def __reduce__(self) -> tuple[Callable[[dict[str, Any]], Edge], tuple[dict[str, Any]]]:
+        return (
+            self._unreduce,
+            (
+                dict(
+                    task_key=self.task_key,
+                    dataset_type_key=self.dataset_type_key,
+                    storage_class_name=self.storage_class_name,
+                    connection_name=self.connection_name,
+                    is_calibration=self.is_calibration,
+                    raw_dimensions=self.raw_dimensions,
+                ),
+            ),
+        )
+
 
 class ReadEdge(Edge):
     """Representation of an input connection (including init-inputs and
     prerequisites) in a pipeline graph.
 
     Parameters
     ----------
@@ -613,14 +633,32 @@
     def _to_xgraph_state(self) -> dict[str, Any]:
         # Docstring inherited.
         result = super()._to_xgraph_state()
         result["component"] = self.component
         result["is_prerequisite"] = self.is_prerequisite
         return result
 
+    def __reduce__(self) -> tuple[Callable[[dict[str, Any]], Edge], tuple[dict[str, Any]]]:
+        return (
+            self._unreduce,
+            (
+                dict(
+                    dataset_type_key=self.dataset_type_key,
+                    task_key=self.task_key,
+                    storage_class_name=self.storage_class_name,
+                    connection_name=self.connection_name,
+                    is_calibration=self.is_calibration,
+                    raw_dimensions=self.raw_dimensions,
+                    is_prerequisite=self.is_prerequisite,
+                    component=self.component,
+                    defer_query_constraint=self.defer_query_constraint,
+                ),
+            ),
+        )
+
 
 class WriteEdge(Edge):
     """Representation of an output connection (including init-outputs) in a
     pipeline graph.
 
     Notes
     -----
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_exceptions.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_exceptions.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_mapping_views.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_mapping_views.py`

 * *Files 18% similar despite different names*

```diff
@@ -128,14 +128,55 @@
     Mapping keys are task labels and values are `TaskNode` instances.
     Iteration order is topological if and only if the `PipelineGraph` has been
     sorted since its last modification.
     """
 
     _NODE_TYPE = NodeType.TASK
 
+    def between(self, first: str | None = None, last: str | None = None) -> Mapping[str, TaskNode]:
+        """Return a mapping whose tasks are between a range of tasks.
+
+        Parameters
+        ----------
+        first : `str`, optional
+            Label of the first task to include, inclusive.
+        last : `str`, optional
+            Label of the last task to include, inclusive.
+
+        Returns
+        -------
+        between : `~collections.abc.Mapping` [ `str`, `TaskNode` ]
+            Tasks that are downstream of ``first`` and upstream of ``last``.
+            If either ``first`` or ``last`` is `None` (default), that side
+            of the result is unbounded.  Tasks that have no dependency
+            relationship to either task are not included, and if both bounds
+            are provided, included tasks must have the right relationship with
+            both bounding tasks.
+        """
+        # This is definitely not the fastest way to compute this subset, but
+        # it's a very simple one (given what networkx provides), and pipeline
+        # graphs are never *that* big.
+        if first is not None:
+            first_key = NodeKey(NodeType.TASK, first)
+            a: set[NodeKey] = set(networkx.dag.descendants(self._parent_xgraph, first_key))
+            a.add(first_key)
+        else:
+            a = set(self._parent_xgraph.nodes.keys())
+        if last is not None:
+            last_key = NodeKey(NodeType.TASK, last)
+            b: set[NodeKey] = set(networkx.dag.ancestors(self._parent_xgraph, last_key))
+            b.add(last_key)
+        else:
+            b = set(self._parent_xgraph.nodes.keys())
+        return {
+            key.name: self._parent_xgraph.nodes[key]["instance"]
+            for key in a & b
+            if key.node_type is NodeType.TASK
+        }
+
 
 class TaskInitMappingView(MappingView[TaskInitNode]):
     """A mapping view of the nodes representing task initialization in a
     `PipelineGraph`.
 
     Notes
     -----
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_nodes.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_nodes.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_pipeline_graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,21 +27,22 @@
 from __future__ import annotations
 
 __all__ = ("PipelineGraph",)
 
 import gzip
 import itertools
 import json
-from collections.abc import Iterable, Iterator, Mapping, Sequence
+from collections.abc import Callable, Iterable, Iterator, Mapping, Sequence, Set
 from typing import TYPE_CHECKING, Any, BinaryIO, Literal, TypeVar, cast
 
 import networkx
 import networkx.algorithms.bipartite
 import networkx.algorithms.dag
-from lsst.daf.butler import DataCoordinate, DataId, DimensionGroup, DimensionUniverse, Registry
+from lsst.daf.butler import DataCoordinate, DataId, DatasetType, DimensionGroup, DimensionUniverse, Registry
+from lsst.daf.butler.registry import MissingDatasetTypeError
 from lsst.resources import ResourcePath, ResourcePathExpression
 
 from ._dataset_types import DatasetTypeNode
 from ._edges import Edge, ReadEdge, WriteEdge
 from ._exceptions import (
     DuplicateOutputError,
     EdgesChangedError,
@@ -256,14 +257,54 @@
         return self.copy()
 
     def __deepcopy__(self, memo: dict) -> PipelineGraph:
         # Genuine deep copies are unnecessary, since we should only ever care
         # that mutable state is copied.
         return self.copy()
 
+    def diff_tasks(self, other: PipelineGraph) -> list[str]:
+        """Compare two pipeline graphs.
+
+        This only compares graph structure and task classes (including their
+        edges).  It does *not* compare full configuration (which is subject to
+        spurious differences due to import-cache state), dataset type
+        resolutions, or sort state.
+
+        Parameters
+        ----------
+        other : `PipelineGraph`
+            Graph to compare to.
+
+        Returns
+        -------
+        differences : `list` [ `str` ]
+            List of string messages describing differences between the
+            pipelines.  If empty, the graphs have the same tasks and
+            connections.
+        """
+        messages: list[str] = []
+        common_labels: Set[str]
+        if self.tasks.keys() != other.tasks.keys():
+            common_labels = self.tasks.keys() & other.tasks.keys()
+            messages.append(
+                f"Pipelines have different tasks: A & ~B = {list(self.tasks.keys() - common_labels)}, "
+                f"B & ~A = {list(other.tasks.keys() - common_labels)}."
+            )
+        else:
+            common_labels = self.tasks.keys()
+        for label in common_labels:
+            a = self.tasks[label]
+            b = other.tasks[label]
+            if a.task_class != b.task_class:
+                messages.append(
+                    f"Task {label!r} has class {a.task_class_name} in A, " f"but {b.task_class_name} in B."
+                )
+            messages.extend(a.diff_edges(b))
+        return messages
+
     def producing_edge_of(self, dataset_type_name: str) -> WriteEdge | None:
         """Return the `WriteEdge` that links the producing task to the named
         dataset type.
 
         Parameters
         ----------
         dataset_type_name : `str`
@@ -461,32 +502,43 @@
         node: TaskNode | TaskInitNode = self.tasks[task_label] if not init else self.tasks[task_label].init
         iterable = node.iter_all_outputs() if include_automatic_connections else node.outputs.values()
         return {
             edge.parent_dataset_type_name: self._xgraph.nodes[edge.dataset_type_key]["instance"]
             for edge in iterable
         }
 
-    def resolve(self, registry: Registry) -> None:
+    def resolve(
+        self,
+        registry: Registry | None = None,
+        dimensions: DimensionUniverse | None = None,
+        dataset_types: Mapping[str, DatasetType] | None = None,
+    ) -> None:
         """Resolve all dimensions and dataset types and check them for
         consistency.
 
         Resolving a graph also causes it to be sorted.
 
         Parameters
         ----------
-        registry : `lsst.daf.butler.Registry`
-            Client for the data repository to resolve against.
+        registry : `lsst.daf.butler.Registry`, optional
+            Client for the data repository to resolve against.  If not
+            provided, both ``dimensions`` and ``dataset_types`` must be.
+        dimensions : `lsst.daf.butler.DimensionUniverse`, optional
+            Definitions for all dimensions.
+        dataset_types : `~collection.abc.Mapping` [ `str`, \
+                `~lsst.daf.butler.DatasetType` ], optional
+            Mapping of dataset types to consider registered.
 
         Notes
         -----
-        The `universe` attribute is set to ``registry.dimensions`` and used to
-        set all `TaskNode.dimensions` attributes.  Dataset type nodes are
-        resolved by first looking for a registry definition, then using the
-        producing task's definition, then looking for consistency between all
-        consuming task definitions.
+        The `universe` attribute is set to ``dimensions`` and used to set all
+        `TaskNode.dimensions` attributes.  Dataset type nodes are resolved by
+        first looking for a registry definition, then using the producing
+        task's definition, then looking for consistency between all consuming
+        task definitions.
 
         Raises
         ------
         ConnectionTypeConsistencyError
             Raised if a prerequisite input for one task appears as a different
             kind of connection in any other task.
         DuplicateOutputError
@@ -500,27 +552,48 @@
             dataset types that are not produced by a task in the pipeline and
             are consumed with different storage classes or as components by
             tasks in the pipeline.
         EdgesChangedError
             Raised if ``check_edges_unchanged=True`` and the edges of a task do
             change after import and reconfiguration.
         """
+        get_registered: Callable[[str], DatasetType | None]
+        if registry is None:
+            if dimensions is None or dataset_types is None:
+                raise PipelineGraphError(
+                    "Either 'registry' or both 'dimensions' and 'dataset_types' "
+                    "must be passed to PipelineGraph.resolve."
+                )
+
+        else:
+            if dimensions is None:
+                dimensions = registry.dimensions
+
+            def get_registered(name: str) -> DatasetType | None:
+                try:
+                    return registry.getDatasetType(name)
+                except MissingDatasetTypeError:
+                    return None
+
+        if dataset_types is not None:
+            # Ruff seems confused about whether this is used below; it is!
+            get_registered = dataset_types.get
         node_key: NodeKey
         updates: dict[NodeKey, TaskNode | DatasetTypeNode] = {}
         for node_key, node_state in self._xgraph.nodes.items():
             match node_key.node_type:
                 case NodeType.TASK:
                     task_node: TaskNode = node_state["instance"]
-                    new_task_node = task_node._resolved(registry.dimensions)
+                    new_task_node = task_node._resolved(dimensions)
                     if new_task_node is not task_node:
                         updates[node_key] = new_task_node
                 case NodeType.DATASET_TYPE:
                     dataset_type_node: DatasetTypeNode | None = node_state["instance"]
                     new_dataset_type_node = DatasetTypeNode._from_edges(
-                        node_key, self._xgraph, registry, previous=dataset_type_node
+                        node_key, self._xgraph, get_registered, dimensions, previous=dataset_type_node
                     )
                     # Usage of `is`` here is intentional; `_from_edges` returns
                     # `previous=dataset_type_node` if it can determine that it
                     # doesn't need to change.
                     if new_dataset_type_node is not dataset_type_node:
                         updates[node_key] = new_dataset_type_node
         try:
@@ -529,15 +602,15 @@
         except Exception as err:  # pragma: no cover
             # There's no known way to get here, but we want to make it
             # clear it's a big problem if we do.
             raise PipelineGraphExceptionSafetyError(
                 "Error during dataset type resolution has left the graph in an inconsistent state."
             ) from err
         self.sort()
-        self._universe = registry.dimensions
+        self._universe = dimensions
 
     ###########################################################################
     #
     # Graph Modification Interface:
     #
     # - methods to add, remove, and replace tasks;
     #
@@ -548,29 +621,31 @@
     # instead.  (These are also the methods used to make a graph from a
     # Pipeline, or make a graph from another graph.)
     #
     ###########################################################################
 
     def add_task(
         self,
-        label: str,
+        label: str | None,
         task_class: type[PipelineTask],
-        config: PipelineTaskConfig,
+        config: PipelineTaskConfig | None = None,
         connections: PipelineTaskConnections | None = None,
     ) -> TaskNode:
         """Add a new task to the graph.
 
         Parameters
         ----------
-        label : `str`
-            Label for the task in the pipeline.
+        label : `str` or `None`
+            Label for the task in the pipeline.  If `None`, `Task._DefaultName`
+            is used.
         task_class : `type` [ `PipelineTask` ]
             Class object for the task.
-        config : `PipelineTaskConfig`
-            Configuration for the task.
+        config : `PipelineTaskConfig`, optional
+            Configuration for the task.  If not provided, a default-constructed
+            instance of ``task_class.ConfigClass`` is used.
         connections : `PipelineTaskConnections`, optional
             Object that describes the dataset types used by the task.  If not
             provided, one will be constructed from the given configuration.  If
             provided, it is assumed that ``config`` has already been validated
             and frozen.
 
         Returns
@@ -596,14 +671,18 @@
         until `resolve` is called, since the resolution depends on both the
         state of the data repository and all contributing tasks.
 
         Adding new tasks removes any existing resolutions of all dataset types
         it references and marks the graph as unsorted.  It is most effiecient
         to add all tasks up front and only then resolve and/or sort the graph.
         """
+        if label is None:
+            label = task_class._DefaultName
+        if config is None:
+            config = task_class.ConfigClass()
         task_node = TaskNode._from_imported_data(
             key=NodeKey(NodeType.TASK, label),
             init_key=NodeKey(NodeType.TASK_INIT, label),
             data=_TaskNodeImportedData.configure(label, task_class, config, connections),
             universe=self.universe,
         )
         self.add_task_nodes([task_node])
@@ -1454,15 +1533,15 @@
         from ..pipeline import TaskDef
 
         for node in self._tasks.values():
             yield TaskDef(
                 config=node.config,
                 taskClass=node.task_class,
                 label=node.label,
-                connections=node._get_imported_data().connections,
+                connections=node.get_connections(),
             )
 
     def _init_from_args(
         self,
         xgraph: networkx.MultiDiGraph | None,
         sorted_keys: Sequence[NodeKey] | None,
         task_subsets: dict[str, TaskSubset] | None,
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_task_subsets.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_task_subsets.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/_tasks.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/_tasks.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     DataCoordinate,
     DatasetRef,
     DatasetType,
     DimensionGroup,
     DimensionUniverse,
     Registry,
 )
+from lsst.pex.config import FieldValidationError
 from lsst.utils.classes import immutable
 from lsst.utils.doImport import doImportType
 from lsst.utils.introspection import get_full_type_name
 
 from .. import automatic_connection_constants as acc
 from ..connections import PipelineTaskConnections
 from ..connectionTypes import BaseConnection, InitOutput, Output
@@ -143,20 +144,24 @@
             Instance of this struct.
         """
         if connections is None:
             # If we don't have connections yet, assume the config hasn't been
             # validated yet.
             try:
                 config.validate()
+            except FieldValidationError as err:
+                err.fullname = f"{label}: {err.fullname}"
+                raise err
             except Exception as err:
                 raise ValueError(
                     f"Configuration validation failed for task {label!r} (see chained exception)."
                 ) from err
             config.freeze()
-            connections = task_class.ConfigClass.ConnectionsClass(config=config)
+            # MyPy doesn't see the metaclass attribute defined for this.
+            connections = config.ConnectionsClass(config=config)  # type: ignore
         connection_map = dict(connections.allConnections)
         connection_map[acc.CONFIG_INIT_OUTPUT_CONNECTION_NAME] = InitOutput(
             acc.CONFIG_INIT_OUTPUT_TEMPLATE.format(label=label),
             acc.CONFIG_INIT_OUTPUT_STORAGE_CLASS,
         )
         connection_map[acc.METADATA_OUTPUT_CONNECTION_NAME] = Output(
             acc.METADATA_OUTPUT_TEMPLATE.format(label=label),
@@ -407,14 +412,43 @@
             return self._imported_data
         except AttributeError:
             raise TaskNotImportedError(
                 f"Task class {self.task_class_name!r} for label {self.label!r} has not been imported "
                 "(see PipelineGraph.import_and_configure)."
             ) from None
 
+    @staticmethod
+    def _unreduce(kwargs: dict[str, Any]) -> TaskInitNode:
+        """Unpickle a `TaskInitNode` instance."""
+        # Connections classes are not pickleable, so we can't use the
+        # dataclass-provided pickle implementation of _TaskNodeImportedData,
+        # and it's easier to just call its `configure` method than to fix it.
+        if (imported_data_args := kwargs.pop("imported_data_args", None)) is not None:
+            imported_data = _TaskNodeImportedData.configure(*imported_data_args)
+        else:
+            imported_data = None
+        return TaskInitNode(imported_data=imported_data, **kwargs)
+
+    def __reduce__(self) -> tuple[Callable[[dict[str, Any]], TaskInitNode], tuple[dict[str, Any]]]:
+        kwargs = dict(
+            key=self.key,
+            inputs=self.inputs,
+            outputs=self.outputs,
+            config_output=self.config_output,
+            task_class_name=getattr(self, "_task_class_name", None),
+            config_str=getattr(self, "_config_str", None),
+        )
+        if hasattr(self, "_imported_data"):
+            kwargs["imported_data_args"] = (
+                self.label,
+                self.task_class,
+                self.config,
+            )
+        return (self._unreduce, (kwargs,))
+
 
 @immutable
 class TaskNode:
     """A node in a pipeline graph that represents a labeled configuration of a
     `PipelineTask`.
 
     Parameters
@@ -439,15 +473,15 @@
 
         This does not include the special `log_output` and `metadata_output`
         edges; use `iter_all_outputs` to include that, too.
     log_output : `WriteEdge` or `None`
         The special runtime output that persists the task's logs.
     metadata_output : `WriteEdge`
         The special runtime output that persists the task's metadata.
-    dimensions : `lsst.daf.butler.DimensionGroup` or `frozenset`
+    dimensions : `lsst.daf.butler.DimensionGroup` or `frozenset` [ `str` ]
         Dimensions of the task.  If a `frozenset`, the dimensions have not been
         resolved by a `~lsst.daf.butler.DimensionUniverse` and cannot be safely
         compared to other sets of dimensions.
 
     Notes
     -----
     Task nodes are intentionally not equality comparable, since there are many
@@ -456,28 +490,28 @@
 
     When included in an exported `networkx` graph (e.g.
     `PipelineGraph.make_xgraph`), task nodes set the following node attributes:
 
     - ``task_class_name``
     - ``bipartite`` (see `NodeType.bipartite`)
     - ``task_class`` (only if `is_imported` is `True`)
-    - ``config`` (only if `is_importd` is `True`)
+    - ``config`` (only if `is_imported` is `True`)
     """
 
     def __init__(
         self,
         key: NodeKey,
         init: TaskInitNode,
         *,
         prerequisite_inputs: Mapping[str, ReadEdge],
         inputs: Mapping[str, ReadEdge],
         outputs: Mapping[str, WriteEdge],
         log_output: WriteEdge | None,
         metadata_output: WriteEdge,
-        dimensions: DimensionGroup | frozenset,
+        dimensions: DimensionGroup | frozenset[str],
     ):
         self.key = key
         self.init = init
         self.prerequisite_inputs = prerequisite_inputs
         self.inputs = inputs
         self.outputs = outputs
         self.log_output = log_output
@@ -523,14 +557,15 @@
         prerequisite_inputs = {
             name: ReadEdge._from_connection_map(key, name, data.connection_map, is_prerequisite=True)
             for name in data.connections.prerequisiteInputs
         }
         inputs = {
             name: ReadEdge._from_connection_map(key, name, data.connection_map)
             for name in data.connections.inputs
+            if not getattr(data.connections, name).deferBinding
         }
         init_outputs = {
             name: WriteEdge._from_connection_map(init_key, name, data.connection_map)
             for name in data.connections.initOutputs
         }
         outputs = {
             name: WriteEdge._from_connection_map(key, name, data.connection_map)
@@ -759,14 +794,25 @@
             Callable that takes a dataset type, a butler registry, a data
             coordinate (the quantum data ID), and an ordered list of
             collections to search, and returns an iterable of
             `~lsst.daf.butler.DatasetRef`.
         """
         return getattr(self._get_imported_data().connection_map[connection_name], "lookupFunction", None)
 
+    def get_connections(self) -> PipelineTaskConnections:
+        """Return the connections class instance for this task.
+
+        Returns
+        -------
+        connections : `.PipelineTaskConnections`
+            Task-provided object that defines inputs and outputs from
+            configuration.
+        """
+        return self._get_imported_data().connections
+
     def get_spatial_bounds_connections(self) -> frozenset[str]:
         """Return the names of connections whose data IDs should be included
         in the calculation of the spatial bounds for this task's quanta.
 
         Returns
         -------
         connection_names : `frozenset` [ `str` ]
@@ -922,14 +968,36 @@
         Raises
         ------
         TaskNotImportedError
             Raised if `is_imported` is `False`.
         """
         return self.init._get_imported_data()
 
+    @staticmethod
+    def _unreduce(kwargs: dict[str, Any]) -> TaskNode:
+        """Unpickle a `TaskNode` instance."""
+        return TaskNode(**kwargs)
+
+    def __reduce__(self) -> tuple[Callable[[dict[str, Any]], TaskNode], tuple[dict[str, Any]]]:
+        return (
+            self._unreduce,
+            (
+                dict(
+                    key=self.key,
+                    init=self.init,
+                    prerequisite_inputs=self.prerequisite_inputs,
+                    inputs=self.inputs,
+                    outputs=self.outputs,
+                    log_output=self.log_output,
+                    metadata_output=self.metadata_output,
+                    dimensions=self._dimensions,
+                ),
+            ),
+        )
+
 
 def _diff_edge_mapping(
     a_mapping: Mapping[str, Edge], b_mapping: Mapping[str, Edge], task_label: str, connection_type: str
 ) -> list[str]:
     """Compare a pair of mappings of edges.
 
     Parameters
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/io.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/io.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_formatting.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_layout.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_merge.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_options.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_options.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_printer.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/pipeline_graph/visualization/_show.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/pipeline_graph/visualization/_show.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/prerequisite_helpers.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/prerequisite_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -669,27 +669,27 @@
         quantum_data_id: DataCoordinate,
     ) -> None:
         timespan = (
             cast(Timespan, quantum_data_id.timespan)
             if task_node.dimensions.temporal
             else Timespan.makeEmpty()
         )
-        self._begin_nsec = timespan._nsec[0]
-        self._end_nsec = timespan._nsec[1]
+        self._begin_nsec = timespan.nsec[0]
+        self._end_nsec = timespan.nsec[1]
         self._dataset_type_names = set()
         for connection_name in bounds_connections:
             if edge := task_node.inputs.get(connection_name):
                 self._dataset_type_names.add(edge.parent_dataset_type_name)
             else:
                 self._dataset_type_names.add(task_node.outputs[connection_name].parent_dataset_type_name)
             # Note that we end up raising if the input is a prerequisite (and
             # hence not in task_node.inputs or task_node.outputs); this
             # justifies the cast in `handle_dataset`.
 
     def handle_dataset(self, parent_dataset_type_name: str, data_id: DataCoordinate) -> None:
         if parent_dataset_type_name in self._dataset_type_names:
-            nsec = cast(Timespan, data_id.timespan)._nsec
+            nsec = cast(Timespan, data_id.timespan).nsec
             self._begin_nsec = min(self._begin_nsec, nsec[0])
             self._end_nsec = max(self._end_nsec, nsec[1])
 
     def finish(self) -> Timespan:
         return Timespan(None, None, _nsec=(self._begin_nsec, self._end_nsec))
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_builder.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/quantum_graph_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 )
 
 import dataclasses
 from abc import ABC, abstractmethod
 from collections.abc import Iterable, Mapping, Sequence
 from typing import TYPE_CHECKING, Any, final
 
+from deprecated.sphinx import deprecated
 from lsst.daf.butler import (
     Butler,
     CollectionType,
     DataCoordinate,
     DatasetRef,
     DatasetType,
     DimensionUniverse,
@@ -80,14 +81,21 @@
 
 class QuantumGraphBuilderError(Exception):
     """Base class for exceptions generated by QuantumGraphBuilder."""
 
     pass
 
 
+# TODO: remove class and switch downstream inheritance to just
+# QuantumGraphBuilderError on DM-40443.
+@deprecated(
+    "Deprecated in favor of QuantumGraphBuilderError and will be removed after v27.",
+    version="v27.0",
+    category=FutureWarning,
+)
 class GraphBuilderError(QuantumGraphBuilderError):
     """Backwards-compatibility near-alias for QuantumGraphBuilderError."""
 
     pass
 
 
 # Inherit from backwards-compatibility alias for backwards-compatibility.
@@ -317,21 +325,26 @@
     @property
     def universe(self) -> DimensionUniverse:
         """Definitions of all data dimensions."""
         return self.butler.dimensions
 
     @final
     @timeMethod
-    def build(self, metadata: Mapping[str, Any] | None = None) -> QuantumGraph:
+    def build(
+        self, metadata: Mapping[str, Any] | None = None, attach_datastore_records: bool = True
+    ) -> QuantumGraph:
         """Build the quantum graph.
 
         Parameters
         ----------
         metadata : `~collections.abc.Mapping`, optional
             Flexible metadata to add to the quantum graph.
+        attach_datastore_records : `bool`, optional
+            Whether to include datastore records in the graph.  Required for
+            `lsst.daf.butler.QuantumBackedButler` execution.
 
         Returns
         -------
         quantum_graph : `QuantumGraph`
             DAG describing processing to be performed.
 
         Notes
@@ -369,15 +382,16 @@
                 full_skeleton[dataset_key]["ref"] = ref
             # Remove dataset nodes with no edges that are not global init
             # outputs, which are generally overall-inputs whose original quanta
             # end up skipped or with no work to do (we can't remove these along
             # with the quanta because no quantum knows if its the only
             # consumer).
             full_skeleton.remove_orphan_datasets()
-            self._attach_datastore_records(full_skeleton)
+            if attach_datastore_records:
+                self._attach_datastore_records(full_skeleton)
             # TODO initialize most metadata here instead of in ctrl_mpexec.
             if metadata is None:
                 metadata = {}
             return self._construct_quantum_graph(full_skeleton, metadata)
 
     @abstractmethod
     def process_subgraph(self, subgraph: PipelineGraph) -> QuantumGraphSkeleton:
@@ -504,17 +518,15 @@
             )
             # Give the task's Connections class an opportunity to remove
             # some inputs, or complain if they are unacceptable.  This will
             # raise if one of the check conditions is not met, which is the
             # intended behavior.
             helper = AdjustQuantumHelper(inputs=adjusted_inputs, outputs=adjusted_outputs)
             try:
-                helper.adjust_in_place(
-                    task_node._get_imported_data().connections, task_node.label, quantum_data_id
-                )
+                helper.adjust_in_place(task_node.get_connections(), task_node.label, quantum_data_id)
             except NoWorkFound as err:
                 # Do not generate this quantum; it would not produce any
                 # outputs.  Remove it and all of the outputs it might have
                 # produced from the skeleton.
                 try:
                     _, connection_name, _ = err.args
                     details = f"not enough datasets for connection {connection_name}."
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/quantum_graph_skeleton.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/quantum_graph_skeleton.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/__init__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/register_instrument.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/register_instrument.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/script/transfer_from_graph.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/script/transfer_from_graph.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/struct.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/struct.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/task.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 import contextlib
 import logging
 import weakref
 from collections.abc import Callable, Iterator, Sequence
 from typing import TYPE_CHECKING, Any, ClassVar
 
 import lsst.utils
+import lsst.utils.introspection
 import lsst.utils.logging
 from lsst.pex.config import ConfigurableField
 from lsst.utils.timer import logInfo
 
 if TYPE_CHECKING:
     from lsst.pex.config import Config
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/taskFactory.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/taskFactory.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,34 +36,40 @@
 from collections.abc import Iterable
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     from lsst.daf.butler import DatasetRef, LimitedButler
 
     from .pipeline import TaskDef
+    from .pipeline_graph import TaskNode
     from .pipelineTask import PipelineTask
 
 
 class TaskFactory(metaclass=ABCMeta):
     """Abstract base class for task factory.
 
     Task factory is responsible for creating instances of PipelineTask
     subclasses.
     """
 
     @abstractmethod
     def makeTask(
-        self, taskDef: TaskDef, butler: LimitedButler, initInputRefs: Iterable[DatasetRef] | None
+        self,
+        task_node: TaskDef | TaskNode,  # TODO: remove TaskDef on DM-40443.
+        /,
+        butler: LimitedButler,
+        initInputRefs: Iterable[DatasetRef] | None,
     ) -> PipelineTask:
         """Create new PipelineTask instance from its `~lsst.pipe.base.TaskDef`.
 
         Parameters
         ----------
-        taskDef : `~lsst.pipe.base.TaskDef`
-            Task definition structure.
+        task_node : `~pipeline_graph.TaskNode` or `TaskDef`
+            Task definition structure.  `TaskDef` support is deprecated and
+            will be removed after v27.
         butler : `lsst.daf.butler.LimitedButler`
             Butler instance used to obtain initialization inputs for task.
         initInputRefs : `~collections.abc.Iterable` of \
                 `~lsst.daf.butler.DatasetRef` or `None`
             List of resolved dataset references for init inputs for this task.
 
         Returns
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/testUtils.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/testUtils.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/__init__.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_data_id_match.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/_data_id_match.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_pipeline_task.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/_pipeline_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,124 +28,93 @@
 
 from lsst.pipe.base.connectionTypes import BaseInput, Output
 
 __all__ = (
     "DynamicConnectionConfig",
     "DynamicTestPipelineTask",
     "DynamicTestPipelineTaskConfig",
+    "ForcedFailure",
     "MockPipelineTask",
     "MockPipelineTaskConfig",
-    "mock_task_defs",
     "mock_pipeline_graph",
 )
 
 import dataclasses
 import logging
 from collections.abc import Collection, Iterable, Mapping
 from typing import TYPE_CHECKING, Any, ClassVar, TypeVar
 
+from astropy.units import Quantity
 from lsst.daf.butler import DataCoordinate, DatasetRef, DeferredDatasetHandle, SerializedDatasetType
 from lsst.pex.config import Config, ConfigDictField, ConfigurableField, Field, ListField
 from lsst.utils.doImport import doImportType
 from lsst.utils.introspection import get_full_type_name
 from lsst.utils.iteration import ensure_iterable
 
 from ... import automatic_connection_constants as acc
 from ... import connectionTypes as cT
 from ...config import PipelineTaskConfig
 from ...connections import InputQuantizedConnection, OutputQuantizedConnection, PipelineTaskConnections
-from ...pipeline import TaskDef
 from ...pipeline_graph import PipelineGraph
 from ...pipelineTask import PipelineTask
 from ._data_id_match import DataIdMatch
 from ._storage_class import MockDataset, MockDatasetQuantum, MockStorageClass, get_mock_name
 
 _LOG = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from ..._quantumContext import QuantumContext
 
 
 _T = TypeVar("_T", bound=cT.BaseConnection)
 
 
-def mock_task_defs(
-    originals: Iterable[TaskDef],
-    unmocked_dataset_types: Iterable[str] = (),
-    force_failures: Mapping[str, tuple[str, type[Exception] | None]] | None = None,
-) -> list[TaskDef]:
-    """Create mocks for an iterable of TaskDefs.
+@dataclasses.dataclass
+class ForcedFailure:
+    """Information about an exception that should be raised by one or more
+    quanta.
+    """
 
-    Parameters
-    ----------
-    originals : `~collections.abc.Iterable` [ `TaskDef` ]
-        Original tasks and configuration to mock.
-    unmocked_dataset_types : `~collections.abc.Iterable` [ `str` ], optional
-        Names of overall-input dataset types that should not be replaced with
-        mocks.
-    force_failures : `~collections.abc.Mapping` [ `str`, `tuple` [ `str`, \
-            `type` [ `Exception` ] or `None` ] ]
-        Mapping from original task label to a 2-tuple indicating that some
-        quanta should raise an exception when executed.  The first entry is a
-        data ID match using the butler expression language (i.e. a string of
-        the sort passed ass the ``where`` argument to butler query methods),
-        while the second is the type of exception to raise when the quantum
-        data ID matches the expression.  An exception type of `None` uses
-        the default, `ValueError`.
+    condition: str
+    """Butler expression-language string that matches the data IDs that should
+    raise.
+    """
 
-    Returns
-    -------
-    mocked : `list` [ `TaskDef` ]
-        List of `TaskDef` objects using `MockPipelineTask` configurations that
-        target the original tasks, in the same order.
+    exception_type: type[Exception] | None = None
+    """The type of exception to raise."""
+
+    memory_required: Quantity | None = None
+    """If not `None`, this failure simulates an out-of-memory failure by
+    raising only if this value exceeds `ExecutionResources.max_mem`.
     """
-    unmocked_dataset_types = tuple(unmocked_dataset_types)
-    if force_failures is None:
-        force_failures = {}
-    results: list[TaskDef] = []
-    for original_task_def in originals:
-        config = MockPipelineTaskConfig()
-        config.original.retarget(original_task_def.taskClass)
-        config.original = original_task_def.config
-        config.unmocked_dataset_types.extend(unmocked_dataset_types)
-        if original_task_def.label in force_failures:
-            condition, exception_type = force_failures[original_task_def.label]
-            config.fail_condition = condition
-            if exception_type is not None:
-                config.fail_exception = get_full_type_name(exception_type)
-        mock_task_def = TaskDef(
-            config=config, taskClass=MockPipelineTask, label=get_mock_name(original_task_def.label)
-        )
-        results.append(mock_task_def)
-    return results
+
+    def set_config(self, config: MockPipelineTaskConfig) -> None:
+        config.fail_condition = self.condition
+        if self.exception_type:
+            config.fail_exception = get_full_type_name(self.exception_type)
+        config.memory_required = self.memory_required
 
 
 def mock_pipeline_graph(
     original_graph: PipelineGraph,
     unmocked_dataset_types: Iterable[str] = (),
-    force_failures: Mapping[str, tuple[str, type[Exception] | None]] | None = None,
+    force_failures: Mapping[str, ForcedFailure] | None = None,
 ) -> PipelineGraph:
     """Create mocks for a full pipeline graph.
 
     Parameters
     ----------
     original_graph : `~..pipeline_graph.PipelineGraph`
         Original tasks and configuration to mock.
     unmocked_dataset_types : `~collections.abc.Iterable` [ `str` ], optional
         Names of overall-input dataset types that should not be replaced with
         mocks.
-    force_failures : `~collections.abc.Mapping` [ `str`, `tuple` [ `str`, \
-            `type` [ `Exception` ] or `None` ] ]
-        Mapping from original task label to a 2-tuple indicating that some
-        quanta should raise an exception when executed.  The first entry is a
-        data ID match using the butler expression language (i.e. a string of
-        the sort passed as the ``where`` argument to butler query methods),
-        while the second is the type of exception to raise when the quantum
-        data ID matches the expression.  An exception type of `None` uses
-        the default, `ValueError`.
+    force_failures : `~collections.abc.Mapping` [ `str`, `ForcedFailure` ]
+        Mapping from original task label to information about an exception one
+        or more quanta for this task should raise.
 
     Returns
     -------
     mocked : `~..pipeline_graph.PipelineGraph`
         Pipeline graph using `MockPipelineTask` configurations that target the
         original tasks.  Never resolved.
     """
@@ -155,18 +124,15 @@
     result = PipelineGraph(description=original_graph.description)
     for original_task_node in original_graph.tasks.values():
         config = MockPipelineTaskConfig()
         config.original.retarget(original_task_node.task_class)
         config.original = original_task_node.config
         config.unmocked_dataset_types.extend(unmocked_dataset_types)
         if original_task_node.label in force_failures:
-            condition, exception_type = force_failures[original_task_node.label]
-            config.fail_condition = condition
-            if exception_type is not None:
-                config.fail_exception = get_full_type_name(exception_type)
+            force_failures[original_task_node.label].set_config(config)
         result.add_task(get_mock_name(original_task_node.label), MockPipelineTask, config=config)
     return result
 
 
 class BaseTestPipelineTaskConnections(PipelineTaskConnections, dimensions=()):
     pass
 
@@ -186,14 +152,25 @@
         default="builtins.ValueError",
         doc=(
             "Class name of the exception to raise when fail condition is triggered. Can be "
             "'lsst.pipe.base.NoWorkFound' to specify non-failure exception."
         ),
     )
 
+    memory_required = Field[str](
+        dtype=str,
+        default=None,
+        optional=True,
+        doc=(
+            "If not None, simulate an out-of-memory failure by raising only if ExecutionResource.max_mem "
+            "exceeds this value.  This string should include units as parsed by astropy.units.Quantity "
+            "(e.g. '4GB')."
+        ),
+    )
+
     def data_id_match(self) -> DataIdMatch | None:
         if not self.fail_condition:
             return None
         return DataIdMatch(self.fail_condition)
 
 
 class BaseTestPipelineTask(PipelineTask):
@@ -236,14 +213,17 @@
         **kwargs: Any,
     ):
         super().__init__(config=config, **kwargs)
         self.fail_exception: type | None = None
         self.data_id_match = self.config.data_id_match()
         if self.data_id_match:
             self.fail_exception = doImportType(self.config.fail_exception)
+            self.memory_required = (
+                Quantity(self.config.memory_required) if self.config.memory_required is not None else None
+            )
         # Look for, check, and record init-inputs.
         task_connections = self.ConfigClass.ConnectionsClass(config=config)
         mock_dataset_quantum = MockDatasetQuantum(task_label=self.getName(), data_id={}, inputs={})
         for connection_name in task_connections.initInputs:
             input_dataset = initInputs[connection_name]
             if not isinstance(input_dataset, MockDataset):
                 raise TypeError(
@@ -295,18 +275,27 @@
 
         _LOG.info("Mocking execution of task '%s' on quantum %s", self.getName(), quantum.dataId)
 
         assert quantum.dataId is not None, "Quantum DataId cannot be None"
 
         # Possibly raise an exception.
         if self.data_id_match is not None and self.data_id_match.match(quantum.dataId):
-            _LOG.info("Simulating failure of task '%s' on quantum %s", self.getName(), quantum.dataId)
-            message = f"Simulated failure: task={self.getName()} dataId={quantum.dataId}"
             assert self.fail_exception is not None, "Exception type must be defined"
-            raise self.fail_exception(message)
+            message = f"Simulated failure: task={self.getName()} dataId={quantum.dataId}"
+            if self.memory_required is not None:
+                if butlerQC.resources.max_mem < self.memory_required:
+                    _LOG.info(
+                        "Simulating out-of-memory failure for task '%s' on quantum %s",
+                        self.getName(),
+                        quantum.dataId,
+                    )
+                    raise self.fail_exception(message)
+            else:
+                _LOG.info("Simulating failure of task '%s' on quantum %s", self.getName(), quantum.dataId)
+                raise self.fail_exception(message)
 
         # Populate the bit of provenance we store in all outputs.
         _LOG.info("Reading input data for task '%s' on quantum %s", self.getName(), quantum.dataId)
         mock_dataset_quantum = MockDatasetQuantum(
             task_label=self.getName(), data_id=dict(quantum.dataId.mapping), inputs={}
         )
         for name, refs in inputRefs:
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/mocks/_storage_class.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/mocks/_storage_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -211,14 +211,18 @@
             """See `pydantic.BaseModel.copy`."""
             return super().copy(*args, **kwargs)
 
         def model_dump(self, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_dump`."""
             return super().model_dump(*args, **kwargs)
 
+        def model_dump_json(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_dump_json`."""
+            return super().model_dump(*args, **kwargs)
+
         def model_copy(self, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_copy`."""
             return super().model_copy(*args, **kwargs)
 
         @classmethod
         def model_json_schema(cls, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_json_schema`."""
@@ -252,14 +256,18 @@
             """See `pydantic.BaseModel.copy`."""
             return super().copy(*args, **kwargs)
 
         def model_dump(self, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_dump`."""
             return super().model_dump(*args, **kwargs)
 
+        def model_dump_json(self, *args: Any, **kwargs: Any) -> Any:
+            """See `pydantic.BaseModel.model_dump_json`."""
+            return super().model_dump(*args, **kwargs)
+
         def model_copy(self, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_copy`."""
             return super().model_copy(*args, **kwargs)
 
         @classmethod
         def model_json_schema(cls, *args: Any, **kwargs: Any) -> Any:
             """See `pydantic.BaseModel.model_json_schema`."""
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/no_dimensions.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/no_dimensions.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/pipelineStepTester.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/pipelineStepTester.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/simpleQGraph.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/simpleQGraph.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,36 +27,38 @@
 
 """Bunch of common classes and methods for use in unit tests.
 """
 from __future__ import annotations
 
 __all__ = ["AddTaskConfig", "AddTask", "AddTaskFactoryMock"]
 
-import itertools
 import logging
+import warnings
 from collections.abc import Iterable, Mapping, MutableMapping
 from typing import TYPE_CHECKING, Any, cast
 
 import lsst.daf.butler.tests as butlerTests
 import lsst.pex.config as pexConfig
 import numpy
 from lsst.daf.butler import Butler, Config, DataId, DatasetRef, DatasetType, Formatter, LimitedButler
 from lsst.daf.butler.logging import ButlerLogRecords
 from lsst.resources import ResourcePath
 from lsst.utils import doImportType
-from lsst.utils.introspection import get_full_type_name
+from lsst.utils.introspection import find_outside_stacklevel, get_full_type_name
 
 from .. import connectionTypes as cT
 from .._instrument import Instrument
+from ..all_dimensions_quantum_graph_builder import AllDimensionsQuantumGraphBuilder
+from ..all_dimensions_quantum_graph_builder import DatasetQueryConstraintVariant as DSQVariant
+from ..automatic_connection_constants import PACKAGES_INIT_OUTPUT_NAME, PACKAGES_INIT_OUTPUT_STORAGE_CLASS
 from ..config import PipelineTaskConfig
 from ..connections import PipelineTaskConnections
 from ..graph import QuantumGraph
-from ..graphBuilder import DatasetQueryConstraintVariant as DSQVariant
-from ..graphBuilder import GraphBuilder
-from ..pipeline import Pipeline, TaskDatasetTypes, TaskDef
+from ..pipeline import Pipeline, TaskDef
+from ..pipeline_graph import PipelineGraph, TaskNode
 from ..pipelineTask import PipelineTask
 from ..struct import Struct
 from ..task import _TASK_FULL_METADATA_TYPE
 from ..taskFactory import TaskFactory
 
 if TYPE_CHECKING:
     from lsst.daf.butler import Registry
@@ -171,59 +173,81 @@
     """
 
     def __init__(self, stopAt: int = -1):
         self.countExec = 0  # incremented by AddTask
         self.stopAt = stopAt  # AddTask raises exception at this call to run()
 
     def makeTask(
-        self, taskDef: TaskDef, butler: LimitedButler, initInputRefs: Iterable[DatasetRef] | None
+        self,
+        task_node: TaskDef | TaskNode,
+        /,
+        butler: LimitedButler,
+        initInputRefs: Iterable[DatasetRef] | None,
     ) -> PipelineTask:
-        taskClass = taskDef.taskClass
-        assert taskClass is not None
-        task = taskClass(config=taskDef.config, initInputs=None, name=taskDef.label)
+        if isinstance(task_node, TaskDef):
+            # TODO: remove support on DM-40443.
+            warnings.warn(
+                "Passing TaskDef to TaskFactory is deprecated and will not be supported after v27.",
+                FutureWarning,
+                find_outside_stacklevel("lsst.pipe.base"),
+            )
+            task_class = task_node.taskClass
+            assert task_class is not None
+        else:
+            task_class = task_node.task_class
+        task = task_class(config=task_node.config, initInputs=None, name=task_node.label)
         task.taskFactory = self  # type: ignore
         return task
 
 
-def registerDatasetTypes(registry: Registry, pipeline: Pipeline | Iterable[TaskDef]) -> None:
+def registerDatasetTypes(registry: Registry, pipeline: Pipeline | Iterable[TaskDef] | PipelineGraph) -> None:
     """Register all dataset types used by tasks in a registry.
 
     Copied and modified from `PreExecInit.initializeDatasetTypes`.
 
     Parameters
     ----------
     registry : `~lsst.daf.butler.Registry`
         Registry instance.
-    pipeline : `typing.Iterable` of `TaskDef`
-        Iterable of TaskDef instances, likely the output of the method
-        `Pipelines.toExpandedPipeline` on a `~lsst.pipe.base.Pipeline` object.
+    pipeline : `.Pipeline`, `~collections.abc..Iterable` of `.TaskDef`, or \
+            `.pipeline_graph.PipelineGraph`
+        The pipeline whose dataset types should be registered, as a `.Pipeline`
+        instance, `.PipelineGraph` instance, or iterable of `.TaskDef`
+        instances.  Support for `.TaskDef` is deprecated and will be removed
+        after v27.
     """
-    for taskDef in pipeline:
-        configDatasetType = DatasetType(
-            taskDef.configDatasetName, {}, storageClass="Config", universe=registry.dimensions
+    match pipeline:
+        case PipelineGraph() as pipeline_graph:
+            pass
+        case Pipeline():
+            pipeline_graph = pipeline.to_graph()
+        case _:
+            warnings.warn(
+                "Passing TaskDefs is deprecated and will not be supported after v27.",
+                category=FutureWarning,
+                stacklevel=find_outside_stacklevel("lsst.pipe.base"),
+            )
+            pipeline_graph = PipelineGraph()
+            for task_def in pipeline:
+                pipeline_graph.add_task(
+                    task_def.label, task_def.taskClass, task_def.config, connections=task_def.connections
+                )
+    pipeline_graph.resolve(registry)
+    dataset_types = [node.dataset_type for node in pipeline_graph.dataset_types.values()]
+    dataset_types.append(
+        DatasetType(
+            PACKAGES_INIT_OUTPUT_NAME,
+            {},
+            storageClass=PACKAGES_INIT_OUTPUT_STORAGE_CLASS,
+            universe=registry.dimensions,
         )
-        storageClass = "Packages"
-        packagesDatasetType = DatasetType(
-            "packages", {}, storageClass=storageClass, universe=registry.dimensions
-        )
-        datasetTypes = TaskDatasetTypes.fromTaskDef(taskDef, registry=registry)
-        for datasetType in itertools.chain(
-            datasetTypes.initInputs,
-            datasetTypes.initOutputs,
-            datasetTypes.inputs,
-            datasetTypes.outputs,
-            datasetTypes.prerequisites,
-            [configDatasetType, packagesDatasetType],
-        ):
-            _LOG.info("Registering %s with registry", datasetType)
-            # this is a no-op if it already exists and is consistent,
-            # and it raises if it is inconsistent. But components must be
-            # skipped
-            if not datasetType.isComponent():
-                registry.registerDatasetType(datasetType)
+    )
+    for dataset_type in dataset_types:
+        _LOG.info("Registering %s with registry", dataset_type)
+        registry.registerDatasetType(dataset_type)
 
 
 def makeSimplePipeline(nQuanta: int, instrument: str | None = None) -> Pipeline:
     """Make a simple Pipeline for tests.
 
     This is called by `makeSimpleQGraph()` if no pipeline is passed to that
     function. It can also be used to customize the pipeline used by
@@ -290,60 +314,74 @@
         butler_config["datastore", "cls"] = "lsst.daf.butler.datastores.fileDatastore.FileDatastore"
     repo = butlerTests.makeTestRepo(str(root_path), {}, config=butler_config)
     butler = Butler.from_config(butler=repo, run=run)
     return butler
 
 
 def populateButler(
-    pipeline: Pipeline, butler: Butler, datasetTypes: dict[str | None, list[str]] | None = None
+    pipeline: Pipeline | PipelineGraph,
+    butler: Butler,
+    datasetTypes: dict[str | None, list[str]] | None = None,
+    instrument: str | None = None,
 ) -> None:
     """Populate data butler with data needed for test.
 
     Initializes data butler with a bunch of items:
     - registers dataset types which are defined by pipeline
     - create dimensions data for (instrument, detector)
     - adds datasets based on ``datasetTypes`` dictionary, if dictionary is
-      missing then a single dataset with type "add_dataset0" is added
+      missing then a single dataset with type "add_dataset0" is added.
 
     All datasets added to butler have ``dataId={instrument=instrument,
     detector=0}`` where ``instrument`` is extracted from pipeline, "INSTR" is
     used if pipeline is missing instrument definition. Type of the dataset is
     guessed from dataset type name (assumes that pipeline is made of `AddTask`
     tasks).
 
     Parameters
     ----------
-    pipeline : `~lsst.pipe.base.Pipeline`
-        Pipeline instance.
+    pipeline : `.Pipeline` or `.pipeline_graph.PipelineGraph`
+        Pipeline or pipeline graph instance.
     butler : `~lsst.daf.butler.Butler`
         Data butler instance.
     datasetTypes : `dict` [ `str`, `list` ], optional
         Dictionary whose keys are collection names and values are lists of
         dataset type names. By default a single dataset of type "add_dataset0"
         is added to a ``butler.run`` collection.
+    instrument : `str`, optional
+        Fully-qualified name of the instrumemnt class (as it appears in a
+        pipeline).  This is needed to propagate the instrument from the
+        original pipeline if a pipeline graph is passed instead.
     """
     # Add dataset types to registry
-    taskDefs = list(pipeline.toExpandedPipeline())
-    registerDatasetTypes(butler.registry, taskDefs)
+    match pipeline:
+        case PipelineGraph() as pipeline_graph:
+            pass
+        case Pipeline():
+            pipeline_graph = pipeline.to_graph()
+            if instrument is None:
+                instrument = pipeline.getInstrument()
+        case _:
+            raise TypeError(f"Unexpected pipeline object: {pipeline!r}.")
+
+    registerDatasetTypes(butler.registry, pipeline_graph)
 
-    instrument = pipeline.getInstrument()
     if instrument is not None:
         instrument_class = doImportType(instrument)
         instrumentName = cast(Instrument, instrument_class).getName()
         instrumentClass = get_full_type_name(instrument_class)
     else:
         instrumentName = "INSTR"
         instrumentClass = None
 
     # Add all needed dimensions to registry
     butler.registry.insertDimensionData("instrument", dict(name=instrumentName, class_name=instrumentClass))
     butler.registry.insertDimensionData("detector", dict(instrument=instrumentName, id=0, full_name="det0"))
 
-    taskDefMap = {taskDef.label: taskDef for taskDef in taskDefs}
-    # Add inputs to butler
+    # Add inputs to butler.
     if not datasetTypes:
         datasetTypes = {None: ["add_dataset0"]}
     for run, dsTypes in datasetTypes.items():
         if run is not None:
             butler.registry.registerRun(run)
         for dsType in dsTypes:
             if dsType == "packages":
@@ -351,31 +389,31 @@
                 # Dict is convertible to Packages if Packages is installed.
                 data: Any = {"python": "9.9.99"}
                 butler.put(data, dsType, run=run)
             else:
                 if dsType.endswith("_config"):
                     # find a config from matching task name or make a new one
                     taskLabel, _, _ = dsType.rpartition("_")
-                    taskDef = taskDefMap.get(taskLabel)
-                    if taskDef is not None:
-                        data = taskDef.config
+                    task_node = pipeline_graph.tasks.get(taskLabel)
+                    if task_node is not None:
+                        data = task_node.config
                     else:
                         data = AddTaskConfig()
                 elif dsType.endswith("_metadata"):
                     data = _TASK_FULL_METADATA_TYPE()
                 elif dsType.endswith("_log"):
                     data = ButlerLogRecords.from_records([])
                 else:
                     data = numpy.array([0.0, 1.0, 2.0, 5.0])
                 butler.put(data, dsType, run=run, instrument=instrumentName, detector=0)
 
 
 def makeSimpleQGraph(
     nQuanta: int = 5,
-    pipeline: Pipeline | None = None,
+    pipeline: Pipeline | PipelineGraph | None = None,
     butler: Butler | None = None,
     root: str | None = None,
     callPopulateButler: bool = True,
     run: str = "test",
     instrument: str | None = None,
     skipExistingIn: Any = None,
     inMemory: bool = True,
@@ -392,17 +430,17 @@
     and butler, fills them with minimal data, and generates QuantumGraph with
     all of that.
 
     Parameters
     ----------
     nQuanta : `int`
         Number of quanta in a graph, only used if ``pipeline`` is None.
-    pipeline : `~lsst.pipe.base.Pipeline`
-        If `None` then a pipeline is made with `AddTask` and default
-        `AddTaskConfig`.
+    pipeline : `.Pipeline` or `.pipeline_graph.PipelineGraph`
+        Pipeline or pipeline graph to build the graph from. If `None`, a
+        pipeline is made with `AddTask` and default `AddTaskConfig`.
     butler : `~lsst.daf.butler.Butler`, optional
         Data butler instance, if None then new data butler is created by
         calling `makeSimpleButler`.
     root : `str`
         Path or URI to the root location of the new repository. Only used if
         ``butler`` is None.
     callPopulateButler : `bool`, optional
@@ -443,52 +481,60 @@
     Returns
     -------
     butler : `~lsst.daf.butler.Butler`
         Butler instance.
     qgraph : `~lsst.pipe.base.QuantumGraph`
         Quantum graph instance.
     """
-    if pipeline is None:
-        pipeline = makeSimplePipeline(nQuanta=nQuanta, instrument=instrument)
+    match pipeline:
+        case PipelineGraph() as pipeline_graph:
+            pass
+        case Pipeline():
+            pipeline_graph = pipeline.to_graph()
+            if instrument is None:
+                instrument = pipeline.getInstrument()
+        case None:
+            pipeline_graph = makeSimplePipeline(nQuanta=nQuanta, instrument=instrument).to_graph()
+        case _:
+            raise TypeError(f"Unexpected pipeline object: {pipeline!r}.")
 
     if butler is None:
         if root is None:
             raise ValueError("Must provide `root` when `butler` is None")
         if callPopulateButler is False:
             raise ValueError("populateButler can only be False when butler is supplied as an argument")
         butler = makeSimpleButler(root, run=run, inMemory=inMemory)
 
     if callPopulateButler:
-        populateButler(pipeline, butler, datasetTypes=datasetTypes)
+        populateButler(pipeline_graph, butler, datasetTypes=datasetTypes, instrument=instrument)
 
     # Make the graph
-    _LOG.debug("Instantiating GraphBuilder, skipExistingIn=%s", skipExistingIn)
-    builder = GraphBuilder(
-        registry=butler.registry,
-        skipExistingIn=skipExistingIn,
-        datastore=butler._datastore if makeDatastoreRecords else None,
-    )
-    if not run:
-        assert butler.run is not None, "Butler must have run defined"
-        run = butler.run
     _LOG.debug(
-        "Calling GraphBuilder.makeGraph, collections=%r, run=%r, userQuery=%r bind=%s",
+        "Instantiating QuantumGraphBuilder, "
+        "skip_existing_in=%s, input_collections=%r, output_run=%r, where=%r, bind=%s.",
+        skipExistingIn,
         butler.collections,
         run,
         userQuery,
         bind,
     )
+    if not run:
+        assert butler.run is not None, "Butler must have run defined"
+        run = butler.run
+    builder = AllDimensionsQuantumGraphBuilder(
+        pipeline_graph,
+        butler,
+        skip_existing_in=skipExistingIn if skipExistingIn is not None else [],
+        input_collections=butler.collections if butler.collections is not None else [run],
+        output_run=run,
+        where=userQuery,
+        bind=bind,
+        dataset_query_constraint=datasetQueryConstraint,
+    )
+    _LOG.debug("Calling QuantumGraphBuilder.build.")
     if not metadata:
         metadata = {}
     metadata["output_run"] = run
 
-    qgraph = builder.makeGraph(
-        pipeline,
-        collections=butler.collections,
-        run=run,
-        userQuery=userQuery,
-        datasetQueryConstraint=datasetQueryConstraint,
-        bind=bind,
-        metadata=metadata,
-    )
+    qgraph = builder.build(metadata=metadata, attach_datastore_records=makeDatastoreRecords)
 
     return butler, qgraph
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst/pipe/base/tests/util.py` & `lsst_pipe_base-27.0.0rc1/python/lsst/pipe/base/tests/util.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/PKG-INFO` & `lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-pipe-base
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: Pipeline infrastructure for the Rubin Science Pipelines.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/pipe_base
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-pipe-base-26.2024.900/python/lsst_pipe_base.egg-info/SOURCES.txt` & `lsst_pipe_base-27.0.0rc1/python/lsst_pipe_base.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 python/lsst/pipe/base/_instrument.py
 python/lsst/pipe/base/_observation_dimension_packer.py
 python/lsst/pipe/base/_quantumContext.py
 python/lsst/pipe/base/_status.py
 python/lsst/pipe/base/_task_metadata.py
 python/lsst/pipe/base/all_dimensions_quantum_graph_builder.py
 python/lsst/pipe/base/automatic_connection_constants.py
+python/lsst/pipe/base/caching_limited_butler.py
 python/lsst/pipe/base/config.py
 python/lsst/pipe/base/configOverrides.py
 python/lsst/pipe/base/connectionTypes.py
 python/lsst/pipe/base/connections.py
 python/lsst/pipe/base/executionButlerBuilder.py
 python/lsst/pipe/base/execution_reports.py
 python/lsst/pipe/base/graphBuilder.py
@@ -58,14 +59,15 @@
 python/lsst/pipe/base/formatters/__init__.py
 python/lsst/pipe/base/formatters/pexConfig.py
 python/lsst/pipe/base/graph/__init__.py
 python/lsst/pipe/base/graph/_implDetails.py
 python/lsst/pipe/base/graph/_loadHelpers.py
 python/lsst/pipe/base/graph/_versionDeserializers.py
 python/lsst/pipe/base/graph/graph.py
+python/lsst/pipe/base/graph/graphSummary.py
 python/lsst/pipe/base/graph/quantumNode.py
 python/lsst/pipe/base/pipeline_graph/__init__.py
 python/lsst/pipe/base/pipeline_graph/__main__.py
 python/lsst/pipe/base/pipeline_graph/_dataset_types.py
 python/lsst/pipe/base/pipeline_graph/_edges.py
 python/lsst/pipe/base/pipeline_graph/_exceptions.py
 python/lsst/pipe/base/pipeline_graph/_mapping_views.py
@@ -95,26 +97,26 @@
 python/lsst/pipe/base/tests/mocks/_storage_class.py
 python/lsst_pipe_base.egg-info/PKG-INFO
 python/lsst_pipe_base.egg-info/SOURCES.txt
 python/lsst_pipe_base.egg-info/dependency_links.txt
 python/lsst_pipe_base.egg-info/requires.txt
 python/lsst_pipe_base.egg-info/top_level.txt
 python/lsst_pipe_base.egg-info/zip-safe
+tests/test_caching_limited_butler.py
 tests/test_cliCmdRegisterInstrument.py
 tests/test_configOverrides.py
 tests/test_config_formatter.py
 tests/test_connections.py
 tests/test_dataid_match.py
 tests/test_dataset_handle.py
 tests/test_dynamic_connections.py
 tests/test_executionButler.py
 tests/test_execution_reports.py
 tests/test_graphBuilder.py
 tests/test_instrument.py
-tests/test_pipeTools.py
 tests/test_pipeline.py
 tests/test_pipelineIR.py
 tests/test_pipelineLoadSubset.py
 tests/test_pipelineTask.py
 tests/test_pipeline_graph.py
 tests/test_quantumGraph.py
 tests/test_struct.py
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_cliCmdRegisterInstrument.py` & `lsst_pipe_base-27.0.0rc1/tests/test_cliCmdRegisterInstrument.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_configOverrides.py` & `lsst_pipe_base-27.0.0rc1/tests/test_configOverrides.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_config_formatter.py` & `lsst_pipe_base-27.0.0rc1/tests/test_config_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_connections.py` & `lsst_pipe_base-27.0.0rc1/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_dataid_match.py` & `lsst_pipe_base-27.0.0rc1/tests/test_dataid_match.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_dataset_handle.py` & `lsst_pipe_base-27.0.0rc1/tests/test_dataset_handle.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_dynamic_connections.py` & `lsst_pipe_base-27.0.0rc1/tests/test_dynamic_connections.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_executionButler.py` & `lsst_pipe_base-27.0.0rc1/tests/test_executionButler.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_execution_reports.py` & `lsst_pipe_base-27.0.0rc1/tests/test_execution_reports.py`

 * *Files 18% similar despite different names*

```diff
@@ -43,13 +43,24 @@
 
     def test_make_reports(self) -> None:
         """Test make_reports to verify that output exists."""
         with temporaryDirectory() as root:
             # make a simple qgraph to make an execution report on
             butler, qgraph = simpleQGraph.makeSimpleQGraph(root=root)
             report = QuantumGraphExecutionReport.make_reports(butler, qgraph)
-            dict_of_expected_failures = report.to_summary_dict(butler, do_store_logs=False)
-            self.assertIsNotNone(dict_of_expected_failures["task0"]["failed_quanta"])
-            self.assertEqual(dict_of_expected_failures["task1"]["outputs"]["add_dataset2"]["blocked"], 1)
-            self.assertDictEqual(dict_of_expected_failures["task2"]["failed_quanta"], {})
-            self.assertEqual(dict_of_expected_failures["task3"]["outputs"]["add_dataset4"]["produced"], 0)
-            self.assertEqual(dict_of_expected_failures["task4"]["n_quanta_blocked"], 1)
+            # make a summary dictionary with a certain amount of
+            # expected failures and check that they are there
+            exp_failures = report.to_summary_dict(butler, do_store_logs=False)
+            self.assertIsNotNone(exp_failures["task0"]["failed_quanta"])
+            self.assertEqual(exp_failures["task1"]["outputs"]["add_dataset2"]["blocked"], 1)
+            self.assertDictEqual(exp_failures["task2"]["failed_quanta"], {})
+            self.assertEqual(exp_failures["task3"]["outputs"]["add_dataset4"]["produced"], 0)
+            self.assertEqual(exp_failures["task4"]["n_quanta_blocked"], 1)
+
+            # now we'll make a human-readable summary dict and
+            # repeat the tests:
+            hr_exp_failures = report.to_summary_dict(butler, do_store_logs=False, human_readable=True)
+            self.assertIsNotNone(hr_exp_failures["task0"]["failed_quanta"])
+            self.assertEqual(hr_exp_failures["task1"]["outputs"]["add_dataset2"]["blocked"], 1)
+            self.assertDictEqual(hr_exp_failures["task2"]["failed_quanta"], {})
+            self.assertEqual(hr_exp_failures["task3"]["outputs"]["add_dataset4"]["produced"], 0)
+            self.assertEqual(hr_exp_failures["task4"]["n_quanta_blocked"], 1)
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_graphBuilder.py` & `lsst_pipe_base-27.0.0rc1/tests/test_graphBuilder.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 import io
 import logging
 import unittest
 
 import lsst.utils.tests
 from lsst.daf.butler.registry import UserExpressionError
 from lsst.pipe.base import QuantumGraph
-from lsst.pipe.base.graphBuilder import DatasetQueryConstraintVariant
+from lsst.pipe.base.all_dimensions_quantum_graph_builder import DatasetQueryConstraintVariant
 from lsst.pipe.base.tests import simpleQGraph
 from lsst.utils.tests import temporaryDirectory
 
 _LOG = logging.getLogger(__name__)
 
 
 class GraphBuilderTestCase(unittest.TestCase):
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_instrument.py` & `lsst_pipe_base-27.0.0rc1/tests/test_instrument.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,16 +36,16 @@
 from lsst.daf.butler.formatters.json import JsonFormatter
 from lsst.daf.butler.registry.sql_registry import SqlRegistry
 from lsst.pex.config import Config
 from lsst.pipe.base import Instrument
 from lsst.utils.introspection import get_full_type_name
 
 
-class DummyInstrument(Instrument):
-    """Test instrument."""
+class BaseDummyInstrument(Instrument):
+    """Test instrument base class."""
 
     @classmethod
     def getName(cls):
         return "DummyInstrument"
 
     def register(self, registry, update=False):
         detector_max = 2
@@ -61,14 +61,25 @@
         with registry.transaction():
             registry.syncDimensionData("instrument", record, update=update)
 
     def getRawFormatter(self, dataId):
         return JsonFormatter
 
 
+class DummyInstrument(BaseDummyInstrument):
+    """Test instrument."""
+
+
+class NotInstrument:
+    """Not an instrument class at all."""
+
+    def __init__(self, collection_prefix: str = ""):
+        self.collection_prefix = collection_prefix
+
+
 class BadInstrument(DummyInstrument):
     """Instrument with wrong class name."""
 
     raw_definition = ("raw2", ("instrument", "detector", "exposure"), "StructuredDataDict")
 
     @classmethod
     def getName(cls):
@@ -152,14 +163,42 @@
         UnimportableInstrument().register(registry)
         with self.assertRaises(ImportError):
             Instrument.fromName("NoImportInstr", registry)
 
         # This should work even with the bad class name.
         self.instrument.importAll(registry)
 
+        # Check that from_string falls back to fromName.
+        from_string = DummyInstrument.from_string("DummyInstrument", registry)
+        self.assertIsInstance(from_string, type(from_registry))
+
+    def test_from_string(self):
+        """Test Instrument.from_string works."""
+        with self.assertRaises(RuntimeError):
+            # No registry.
+            DummyInstrument.from_string("DummyInstrument")
+
+        with self.assertRaises(TypeError):
+            # This will raise because collection_prefix is not understood.
+            DummyInstrument.from_string("lsst.pipe.base.Task")
+
+        with self.assertRaises(TypeError):
+            # Not an instrument but does have collection_prefix.
+            DummyInstrument.from_string(get_full_type_name(NotInstrument))
+
+        with self.assertRaises(TypeError):
+            # This will raise because BaseDummyInstrument is not a subclass
+            # of DummyInstrument.
+            DummyInstrument.from_string(get_full_type_name(BaseDummyInstrument))
+
+        instrument = DummyInstrument.from_string(
+            get_full_type_name(DummyInstrument), collection_prefix="test"
+        )
+        self.assertEqual(instrument.collection_prefix, "test")
+
     def test_defaults(self):
         self.assertEqual(self.instrument.makeDefaultRawIngestRunName(), "DummyInstrument/raw/all")
         self.assertEqual(
             self.instrument.makeUnboundedCalibrationRunName("a", "b"), "DummyInstrument/calib/a/b/unbounded"
         )
         self.assertEqual(
             self.instrument.makeCuratedCalibrationRunName("2018-05-04", "a"),
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_pipeline.py` & `lsst_pipe_base-27.0.0rc1/tests/test_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 """
 
 import pickle
 import textwrap
 import unittest
 
 import lsst.utils.tests
-from lsst.pipe.base import Pipeline, PipelineDatasetTypes, TaskDef
+from lsst.pipe.base import Pipeline, TaskDef
 from lsst.pipe.base.pipelineIR import LabeledSubset
 from lsst.pipe.base.tests.simpleQGraph import AddTask, makeSimplePipeline
 
 
 class PipelineTestCase(unittest.TestCase):
     """A test case for TaskDef and Pipeline."""
 
@@ -56,21 +56,22 @@
         pipeline = Pipeline("test")
         self.assertEqual(len(pipeline), 0)
 
     def testInitial(self):
         """Testing constructor with initial data."""
         pipeline = makeSimplePipeline(2)
         self.assertEqual(len(pipeline), 2)
-        expandedPipeline = list(pipeline.toExpandedPipeline())
-        self.assertEqual(expandedPipeline[0].taskName, "lsst.pipe.base.tests.simpleQGraph.AddTask")
-        self.assertEqual(expandedPipeline[1].taskName, "lsst.pipe.base.tests.simpleQGraph.AddTask")
-        self.assertEqual(expandedPipeline[0].taskClass, AddTask)
-        self.assertEqual(expandedPipeline[1].taskClass, AddTask)
-        self.assertEqual(expandedPipeline[0].label, "task0")
-        self.assertEqual(expandedPipeline[1].label, "task1")
+        pipeline_graph = pipeline.to_graph()
+        pipeline_graph.sort()
+        task_nodes = list(pipeline_graph.tasks.values())
+        self.assertEqual(task_nodes[0].task_class, AddTask)
+        self.assertEqual(task_nodes[1].task_class, AddTask)
+        self.assertEqual(task_nodes[0].label, "task0")
+        self.assertEqual(task_nodes[1].label, "task1")
+        self.assertEqual(pipeline.task_labels, {"task0", "task1"})
 
     def testModifySubset(self):
         pipeline = makeSimplePipeline(2)
 
         # Test adding labels.
         with self.assertRaises(ValueError):
             pipeline.addLabelToSubset("test", "new_label")
@@ -144,49 +145,34 @@
                 class: test_pipeline.AddTask
                 config:
                   addend: parameters.testValue
         """
         )
         # verify that parameters are used in expanding a pipeline
         pipeline = Pipeline.fromString(pipeline_str)
-        expandedPipeline = list(pipeline.toExpandedPipeline())
-        self.assertEqual(expandedPipeline[0].config.addend, 5)
+        pipeline_graph = pipeline.to_graph()
+        self.assertEqual(pipeline_graph.tasks["add"].config.addend, 5)
 
         # verify that a parameter can be overridden on the "command line"
         pipeline.addConfigOverride("parameters", "testValue", 14)
-        expandedPipeline = list(pipeline.toExpandedPipeline())
-        self.assertEqual(expandedPipeline[0].config.addend, 14)
+        pipeline_graph = pipeline.to_graph()
+        self.assertEqual(pipeline_graph.tasks["add"].config.addend, 14)
 
         # verify that parameters does not support files or python overrides
         with self.assertRaises(ValueError):
             pipeline.addConfigFile("parameters", "fakeFile")
         with self.assertRaises(ValueError):
             pipeline.addConfigPython("parameters", "fakePythonString")
 
     def testSerialization(self):
         pipeline = makeSimplePipeline(2)
         dump = str(pipeline)
         load = Pipeline.fromString(dump)
         self.assertEqual(pipeline, load)
 
-    def test_initOutputNames(self):
-        """Test for PipelineDatasetTypes.initOutputNames method."""
-        pipeline = makeSimplePipeline(3)
-        dsType = set(PipelineDatasetTypes.initOutputNames(pipeline))
-        expected = {
-            "packages",
-            "add_init_output1",
-            "add_init_output2",
-            "add_init_output3",
-            "task0_config",
-            "task1_config",
-            "task2_config",
-        }
-        self.assertEqual(dsType, expected)
-
 
 class MyMemoryTestCase(lsst.utils.tests.MemoryTestCase):
     """Run file leak tests."""
 
 
 def setup_module(module):
     """Configure pytest."""
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_pipelineIR.py` & `lsst_pipe_base-27.0.0rc1/tests/test_pipelineIR.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,20 +40,14 @@
 class ConfigIRTestCase(unittest.TestCase):
     """A test case for ConfigIR Objects.
 
     ConfigIR contains a method that is not exercised by the PipelineIR task,
     so it should be tested here.
     """
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
     def testMergeConfig(self):
         # Create some configs to merge
         config1 = ConfigIR(
             python="config.foo=6", dataId={"visit": 7}, file=["test1.py"], rest={"a": 1, "b": 2}
         )
         config2 = ConfigIR(python=None, dataId=None, file=["test2.py"], rest={"c": 1, "d": 2})
         config3 = ConfigIR(python="config.bar=7", dataId=None, file=["test3.py"], rest={"c": 1, "d": 2})
@@ -80,20 +74,14 @@
         # Cant merge configs with shared keys
         self.assertEqual(list(config6.maybe_merge(config7)), [config6, config7])
 
 
 class PipelineIRTestCase(unittest.TestCase):
     """A test case for PipelineIR objects."""
 
-    def setUp(self):
-        pass
-
-    def tearDown(self):
-        pass
-
     def testPipelineIRInitChecks(self):
         # Missing description
         pipeline_str = """
         tasks:
           a: module.A
         """
         with self.assertRaises(ValueError):
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_pipelineLoadSubset.py` & `lsst_pipe_base-27.0.0rc1/tests/test_pipelineLoadSubset.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_pipelineTask.py` & `lsst_pipe_base-27.0.0rc1/tests/test_pipelineTask.py`

 * *Files 10% similar despite different names*

```diff
@@ -96,55 +96,67 @@
         return pipeBase.Struct(output=output)
 
 
 class AddTask2(pipeBase.PipelineTask):
     """Example task which overrides runQuantum() method."""
 
     ConfigClass = AddConfig
-    _DefaultName = "add_task"
+    _DefaultName = "add_task_2"
 
     def runQuantum(
         self, butlerQC: pipeBase.QuantumContext, inputRefs: DatasetRef, outputRefs: DatasetRef
     ) -> None:
         self.metadata.add("add", self.config.addend)
         inputs = butlerQC.get(inputRefs)
         outputs = inputs["input"] + self.config.addend
         butlerQC.put(pipeBase.Struct(output=outputs), outputRefs)
 
 
 class PipelineTaskTestCase(unittest.TestCase):
     """A test case for PipelineTask."""
 
-    def _makeDSRefVisit(self, dstype: DatasetType, visitId: int, universe: DimensionUniverse) -> DatasetRef:
+    def _makeDSRefVisit(self, dstype: DatasetType, visitId: int) -> DatasetRef:
         dataId = DataCoordinate.standardize(
             detector="X",
             visit=visitId,
             physical_filter="a",
             band="b",
             instrument="TestInstrument",
-            universe=universe,
+            graph=dstype.dimensions,
         )
         run = "test"
         ref = DatasetRef(datasetType=dstype, dataId=dataId, run=run)
         return ref
 
-    def _makeQuanta(self, config: pipeBase.PipelineTaskConfig, nquanta: int = 100) -> list[Quantum]:
-        """Create set of Quanta."""
-        universe = DimensionUniverse()
-        connections = config.connections.ConnectionsClass(config=config)
-
-        dstype0 = connections.input.makeDatasetType(universe)
-        dstype1 = connections.output.makeDatasetType(universe)
-
+    def _makeQuanta(
+        self,
+        task_node: pipeBase.pipeline_graph.TaskNode,
+        pipeline_graph: pipeBase.PipelineGraph,
+        nquanta: int = 100,
+    ) -> list[Quantum]:
+        """Create set of Quanta"""
         quanta = []
         for visit in range(nquanta):
-            inputRef = self._makeDSRefVisit(dstype0, visit, universe)
-            outputRef = self._makeDSRefVisit(dstype1, visit, universe)
             quantum = Quantum(
-                inputs={inputRef.datasetType: [inputRef]}, outputs={outputRef.datasetType: [outputRef]}
+                inputs={
+                    pipeline_graph.dataset_types[edge.dataset_type_name].dataset_type: [
+                        self._makeDSRefVisit(
+                            pipeline_graph.dataset_types[edge.dataset_type_name].dataset_type, visit
+                        )
+                    ]
+                    for edge in task_node.inputs.values()
+                },
+                outputs={
+                    pipeline_graph.dataset_types[edge.dataset_type_name].dataset_type: [
+                        self._makeDSRefVisit(
+                            pipeline_graph.dataset_types[edge.dataset_type_name].dataset_type, visit
+                        )
+                    ]
+                    for edge in task_node.outputs.values()
+                },
             )
             quanta.append(quantum)
 
         return quanta
 
     def testRunQuantumFull(self):
         """Test for AddTask.runQuantum() implementation with full butler."""
@@ -154,30 +166,35 @@
         """Test for AddTask.runQuantum() implementation with limited butler."""
         self._testRunQuantum(full_butler=False)
 
     def _testRunQuantum(self, full_butler: bool) -> None:
         """Test for AddTask.runQuantum() implementation."""
         butler = ButlerMock()
         task = AddTask(config=AddConfig())
-        connections = task.config.connections.ConnectionsClass(config=task.config)
+        input_name = task.config.connections.input
+        output_name = task.config.connections.output
+
+        pipeline_graph = pipeBase.PipelineGraph()
+        task_node = pipeline_graph.add_task(None, type(task), task.config)
+        pipeline_graph.resolve(dimensions=butler.dimensions, dataset_types={})
 
         # make all quanta
-        quanta = self._makeQuanta(task.config)
+        quanta = self._makeQuanta(task_node, pipeline_graph)
 
         # add input data to butler
-        dstype0 = connections.input.makeDatasetType(butler.dimensions)
+        dstype0 = pipeline_graph.dataset_types[input_name].dataset_type
         for i, quantum in enumerate(quanta):
             ref = quantum.inputs[dstype0.name][0]
             butler.put(100 + i, ref)
 
         # run task on each quanta
         checked_get = False
         for quantum in quanta:
             butlerQC = pipeBase.QuantumContext(butler, quantum)
-            inputRefs, outputRefs = connections.buildDatasetRefs(quantum)
+            inputRefs, outputRefs = task_node.get_connections().buildDatasetRefs(quantum)
             task.runQuantum(butlerQC, inputRefs, outputRefs)
 
             # Test getting of datasets in different ways.
             # (only need to do this one time)
             if not checked_get:
                 # Force the periodic logger to issue messages.
                 lsst.utils.logging.PeriodicLogger.LOGGING_INTERVAL = 0.0
@@ -206,91 +223,97 @@
 
                 # Output ref won't be known to this quantum.
                 outputs = [ref for _, ref in outputRefs]
                 with self.assertRaises(ValueError):
                     butlerQC.get(outputs[0])
 
         # look at the output produced by the task
-        outputName = connections.output.name
-        dsdata = butler.datasets[outputName]
+        dsdata = butler.datasets[output_name]
         self.assertEqual(len(dsdata), len(quanta))
         for i, quantum in enumerate(quanta):
-            ref = quantum.outputs[outputName][0]
+            ref = quantum.outputs[output_name][0]
             self.assertEqual(dsdata[ref.dataId], 100 + i + 3)
 
     def testChain2Full(self) -> None:
         """Test for two-task chain with full butler."""
         self._testChain2(full_butler=True)
 
     def testChain2Limited(self) -> None:
         """Test for two-task chain with limited butler."""
         self._testChain2(full_butler=False)
 
     def _testChain2(self, full_butler: bool) -> None:
         """Test for two-task chain."""
         butler = ButlerMock()
         config1 = AddConfig()
-        connections1 = config1.connections.ConnectionsClass(config=config1)
+        overall_input_name = config1.connections.input
+        intermediate_name = config1.connections.output
         task1 = AddTask(config=config1)
         config2 = AddConfig()
         config2.addend = 200
-        config2.connections.input = task1.config.connections.output
-        config2.connections.output = "add_output_2"
+        config2.connections.input = intermediate_name
+        overall_output_name = "add_output_2"
+        config2.connections.output = overall_output_name
         task2 = AddTask2(config=config2)
-        connections2 = config2.connections.ConnectionsClass(config=config2)
+
+        pipeline_graph = pipeBase.PipelineGraph()
+        task1_node = pipeline_graph.add_task(None, type(task1), task1.config)
+        task2_node = pipeline_graph.add_task(None, type(task2), task2.config)
+        pipeline_graph.resolve(dimensions=butler.dimensions, dataset_types={})
 
         # make all quanta
-        quanta1 = self._makeQuanta(task1.config)
-        quanta2 = self._makeQuanta(task2.config)
+        quanta1 = self._makeQuanta(task1_node, pipeline_graph)
+        quanta2 = self._makeQuanta(task2_node, pipeline_graph)
 
         # add input data to butler
-        task1Connections = task1.config.connections.ConnectionsClass(config=task1.config)
-        dstype0 = task1Connections.input.makeDatasetType(butler.dimensions)
+        dstype0 = pipeline_graph.dataset_types[overall_input_name].dataset_type
         for i, quantum in enumerate(quanta1):
             ref = quantum.inputs[dstype0.name][0]
             butler.put(100 + i, ref)
 
         # run task on each quanta
         for quantum in quanta1:
             butlerQC = pipeBase.QuantumContext(butler, quantum)
-            inputRefs, outputRefs = connections1.buildDatasetRefs(quantum)
+            inputRefs, outputRefs = task1_node.get_connections().buildDatasetRefs(quantum)
             task1.runQuantum(butlerQC, inputRefs, outputRefs)
         for quantum in quanta2:
             butlerQC = pipeBase.QuantumContext(butler, quantum)
-            inputRefs, outputRefs = connections2.buildDatasetRefs(quantum)
+            inputRefs, outputRefs = task2_node.get_connections().buildDatasetRefs(quantum)
             task2.runQuantum(butlerQC, inputRefs, outputRefs)
 
         # look at the output produced by the task
-        outputName = task1.config.connections.output
-        dsdata = butler.datasets[outputName]
+        dsdata = butler.datasets[intermediate_name]
         self.assertEqual(len(dsdata), len(quanta1))
         for i, quantum in enumerate(quanta1):
-            ref = quantum.outputs[outputName][0]
+            ref = quantum.outputs[intermediate_name][0]
             self.assertEqual(dsdata[ref.dataId], 100 + i + 3)
 
-        outputName = task2.config.connections.output
-        dsdata = butler.datasets[outputName]
+        dsdata = butler.datasets[overall_output_name]
         self.assertEqual(len(dsdata), len(quanta2))
         for i, quantum in enumerate(quanta2):
-            ref = quantum.outputs[outputName][0]
+            ref = quantum.outputs[overall_output_name][0]
             self.assertEqual(dsdata[ref.dataId], 100 + i + 3 + 200)
 
     def testButlerQC(self):
         """Test for QuantumContext. Full and limited share get
         implementation so only full is tested.
         """
         butler = ButlerMock()
         task = AddTask(config=AddConfig())
-        connections = task.config.connections.ConnectionsClass(config=task.config)
+        input_name = task.config.connections.input
+
+        pipeline_graph = pipeBase.PipelineGraph()
+        task_node = pipeline_graph.add_task(None, type(task), config=task.config)
+        pipeline_graph.resolve(dimensions=butler.dimensions, dataset_types={})
 
         # make one quantum
-        (quantum,) = self._makeQuanta(task.config, 1)
+        (quantum,) = self._makeQuanta(task_node, pipeline_graph, 1)
 
         # add input data to butler
-        dstype0 = connections.input.makeDatasetType(butler.dimensions)
+        dstype0 = pipeline_graph.dataset_types[input_name].dataset_type
         ref = quantum.inputs[dstype0.name][0]
         butler.put(100, ref)
 
         butlerQC = pipeBase.QuantumContext(butler, quantum)
         self.assertEqual(butlerQC.resources.num_cores, 1)
         self.assertIsNone(butlerQC.resources.max_mem)
 
@@ -307,15 +330,15 @@
         self.assertEqual(obj, [None])
 
         # COmbine a ref and None.
         obj = butlerQC.get([ref, None])
         self.assertEqual(obj, [100, None])
 
         # Use refs from a QuantizedConnection.
-        inputRefs, outputRefs = connections.buildDatasetRefs(quantum)
+        inputRefs, outputRefs = task_node.get_connections().buildDatasetRefs(quantum)
         obj = butlerQC.get(inputRefs)
         self.assertEqual(obj, {"input": 100})
 
         # Add few None values to a QuantizedConnection.
         inputRefs.input = [None, ref]
         inputRefs.input2 = None
         obj = butlerQC.get(inputRefs)
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_pipeline_graph.py` & `lsst_pipe_base-27.0.0rc1/tests/test_pipeline_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 """Tests of things related to the GraphBuilder class."""
 
 import copy
 import io
 import logging
+import pickle
 import textwrap
 import unittest
 from typing import Any
 
 import lsst.pipe.base.automatic_connection_constants as acc
 import lsst.utils.tests
 from lsst.daf.butler import DataCoordinate, DatasetRef, DatasetType, DimensionUniverse, StorageClassFactory
@@ -152,23 +153,30 @@
         serialization.
         """
         with lsst.utils.tests.getTempFilePath(".json.gz") as filename:
             self.graph._write_uri(filename)
             roundtripped = PipelineGraph._read_uri(filename)
         self.check_make_xgraph(roundtripped, resolved=False)
 
+    def test_unresolved_pickle(self) -> None:
+        """Test that unresolved PipelineGraph objects can be pickled."""
+        self.check_make_xgraph(pickle.loads(pickle.dumps(self.graph)), resolved=False)
+
     def test_unresolved_deferred_import_io(self) -> None:
         """Test round-tripping an unresolved PipelineGraph through
         serialization, without immediately importing tasks on read.
         """
         stream = io.BytesIO()
         self.graph._write_stream(stream)
         stream.seek(0)
         roundtripped = PipelineGraph._read_stream(stream, import_mode=TaskImportMode.DO_NOT_IMPORT)
         self.check_make_xgraph(roundtripped, resolved=False, imported_and_configured=False)
+        self.check_make_xgraph(
+            pickle.loads(pickle.dumps(roundtripped)), resolved=False, imported_and_configured=False
+        )
         # Check that we can still resolve the graph without importing tasks.
         roundtripped.resolve(MockRegistry(self.dimensions, {}))
         self.check_make_xgraph(roundtripped, resolved=True, imported_and_configured=False)
         roundtripped._import_and_configure(TaskImportMode.ASSUME_CONSISTENT_EDGES)
         self.check_make_xgraph(roundtripped, resolved=True, imported_and_configured=True)
 
     def test_resolved_accessors(self) -> None:
@@ -218,24 +226,32 @@
         """
         self.graph.resolve(MockRegistry(self.dimensions, {}))
         with lsst.utils.tests.getTempFilePath(".json.gz") as filename:
             self.graph._write_uri(filename)
             roundtripped = PipelineGraph._read_uri(filename)
         self.check_make_xgraph(roundtripped, resolved=True)
 
+    def test_resolved_pickle(self) -> None:
+        """Test that resolved PipelineGraph objects can be pickled."""
+        self.graph.resolve(MockRegistry(self.dimensions, {}))
+        self.check_make_xgraph(pickle.loads(pickle.dumps(self.graph)), resolved=True)
+
     def test_resolved_deferred_import_io(self) -> None:
         """Test round-tripping a resolved PipelineGraph through serialization,
         without immediately importing tasks on read.
         """
         self.graph.resolve(MockRegistry(self.dimensions, {}))
         stream = io.BytesIO()
         self.graph._write_stream(stream)
         stream.seek(0)
         roundtripped = PipelineGraph._read_stream(stream, import_mode=TaskImportMode.DO_NOT_IMPORT)
         self.check_make_xgraph(roundtripped, resolved=True, imported_and_configured=False)
+        self.check_make_xgraph(
+            pickle.loads(pickle.dumps(roundtripped)), resolved=True, imported_and_configured=False
+        )
         roundtripped._import_and_configure(TaskImportMode.REQUIRE_CONSISTENT_EDGES)
         self.check_make_xgraph(roundtripped, resolved=True, imported_and_configured=True)
 
     def test_unresolved_copies(self) -> None:
         """Test making copies of an unresolved PipelineGraph."""
         copy1 = self.graph.copy()
         self.assertIsNot(copy1, self.graph)
@@ -841,23 +857,29 @@
         expected[htm7_dims][1]["prereq_1"] = self.graph.dataset_types["prereq_1"]
         self.assertEqual(self.graph.group_by_dimensions(prerequisites=True), expected)
 
     def test_add_and_remove(self) -> None:
         """Tests for adding and removing tasks and task subsets from a
         PipelineGraph.
         """
+        original = self.graph.copy()
         # Can't remove a task while it's still in a subset.
         with self.assertRaises(PipelineGraphError):
             self.graph.remove_tasks(["b"], drop_from_subsets=False)
+        self.assertEqual(original.diff_tasks(self.graph), [])
         # ...unless you remove the subset.
         self.graph.remove_task_subset("only_b")
         self.assertFalse(self.graph.task_subsets)
         ((b, referencing_subsets),) = self.graph.remove_tasks(["b"], drop_from_subsets=False)
         self.assertFalse(referencing_subsets)
         self.assertEqual(self.graph.tasks.keys(), {"a"})
+        self.assertEqual(
+            original.diff_tasks(self.graph),
+            ["Pipelines have different tasks: A & ~B = ['b'], B & ~A = []."],
+        )
         # Add that task back in.
         self.graph.add_task_nodes([b])
         self.assertEqual(self.graph.tasks.keys(), {"a", "b"})
         # Add the subset back in.
         self.graph.add_task_subset("only_b", {"b"})
         self.assertEqual(self.graph.task_subsets.keys(), {"only_b"})
         # Resolve the graph's dataset types and task dimensions.
@@ -876,33 +898,42 @@
         self.assertTrue(self.graph.dataset_types.is_resolved("input_1"))
         self.assertNotIn("output1", self.graph.dataset_types)
         self.assertFalse(self.graph.dataset_types.is_resolved("schema"))
         self.assertFalse(self.graph.dataset_types.is_resolved("intermediate_1"))
 
     def test_reconfigure(self) -> None:
         """Tests for PipelineGraph.reconfigure."""
+        original = self.graph.copy()
         self.graph.resolve(MockRegistry(self.dimensions, {}))
         self.b_config.outputs["output1"].storage_class = "TaskMetadata"
         with self.assertRaises(ValueError):
             # Can't check and assume together.
             self.graph.reconfigure_tasks(
                 b=self.b_config, assume_edges_unchanged=True, check_edges_unchanged=True
             )
         # Check that graph is unchanged after error.
         self.check_base_accessors(self.graph)
         with self.assertRaises(EdgesChangedError):
             self.graph.reconfigure_tasks(b=self.b_config, check_edges_unchanged=True)
         self.check_base_accessors(self.graph)
+        self.assertEqual(original.diff_tasks(self.graph), [])
         # Make a change that does affect edges; this will unresolve most
         # dataset types.
         self.graph.reconfigure_tasks(b=self.b_config)
         self.assertTrue(self.graph.dataset_types.is_resolved("input_1"))
         self.assertFalse(self.graph.dataset_types.is_resolved("output_1"))
         self.assertFalse(self.graph.dataset_types.is_resolved("schema"))
         self.assertFalse(self.graph.dataset_types.is_resolved("intermediate_1"))
+        self.assertEqual(
+            original.diff_tasks(self.graph),
+            [
+                "Output b.output1 has storage class '_mock_StructuredDataDict' in A, "
+                "but '_mock_TaskMetadata' in B."
+            ],
+        )
         # Resolving again will pick up the new storage class
         self.graph.resolve(MockRegistry(self.dimensions, {}))
         self.assertEqual(
             self.graph.dataset_types["output_1"].storage_class_name, get_mock_name("TaskMetadata")
         )
 
     def check_visualization(self, graph: PipelineGraph, expected: str, **kwargs: Any) -> None:
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_quantumGraph.py` & `lsst_pipe_base-27.0.0rc1/tests/test_quantumGraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,32 +27,32 @@
 
 import os
 import pickle
 import random
 import tempfile
 import unittest
 import uuid
-from collections.abc import Iterable
 from itertools import chain
 
 import lsst.pipe.base.connectionTypes as cT
 import lsst.utils.tests
 from lsst.daf.butler import Config, DataCoordinate, DatasetRef, DatasetType, DimensionUniverse, Quantum
 from lsst.pex.config import Field
 from lsst.pipe.base import (
     DatasetTypeName,
     PipelineTask,
     PipelineTaskConfig,
     PipelineTaskConnections,
     QuantumGraph,
     TaskDef,
 )
-from lsst.pipe.base.graph.quantumNode import BuildId, QuantumNode
+from lsst.pipe.base.graph.quantumNode import BuildId
 from lsst.pipe.base.tests.util import check_output_run, get_output_refs
 from lsst.utils.introspection import get_full_type_name
+from lsst.utils.packages import Packages
 
 METADATA = {"a": [1, 2, 3]}
 
 
 class Dummy1Connections(PipelineTaskConnections, dimensions=("A", "B")):
     """Dummy connections class #1."""
 
@@ -254,14 +254,15 @@
                         initInputs=initRefs,
                         inputs={inputDSType: inputRefs},
                         outputs={outputDSType: outputRefs},
                     )
                 )
             quantumMap[taskDef] = quantumSet
         self.tasks = tasks
+        self.quanta_by_task_label = {task_def.label: set(quanta) for task_def, quanta in quantumMap.items()}
         self.quantumMap = quantumMap
         self.packagesDSType = DatasetType("packages", universe.empty, storageClass="Packages")
         dataset_types.add(self.packagesDSType)
         globalInitOutputs = [
             DatasetRef(self.packagesDSType, DataCoordinate.make_empty(universe), run=self.output_run)
         ]
         self.qGraph = QuantumGraph(
@@ -273,16 +274,19 @@
             globalInitOutputs=globalInitOutputs,
             registryDatasetTypes=dataset_types,
         )
         self.universe = universe
         self.num_dataset_types = len(dataset_types)
 
     def testTaskGraph(self) -> None:
+        task_def_labels: list[str] = []
         for taskDef in self.quantumMap:
+            task_def_labels.append(taskDef.label)
             self.assertIn(taskDef, self.qGraph.taskGraph)
+        self.assertCountEqual(task_def_labels, self.qGraph.pipeline_graph.tasks.keys())
 
     def testGraph(self) -> None:
         graphSet = {q.quantum for q in self.qGraph.graph}
         for quantum in chain.from_iterable(self.quantumMap.values()):
             self.assertIn(quantum, graphSet)
 
     def testGetQuantumNodeByNodeId(self) -> None:
@@ -315,17 +319,22 @@
 
     def testGetNumberOfQuantaForTask(self) -> None:
         for task in self.tasks:
             self.assertEqual(self.qGraph.getNumberOfQuantaForTask(task), len(self.quantumMap[task]))
 
     def testGetNodesForTask(self) -> None:
         for task in self.tasks:
-            nodes: Iterable[QuantumNode] = self.qGraph.getNodesForTask(task)
+            nodes = list(self.qGraph.getNodesForTask(task))
             quanta_in_node = {n.quantum for n in nodes}
             self.assertEqual(quanta_in_node, self.quantumMap[task])
+            for node in nodes:
+                self.assertEqual(
+                    node.task_node.task_class_name,
+                    self.qGraph.pipeline_graph.tasks[node.task_node.label].task_class_name,
+                )
 
     def testFindTasksWithInput(self) -> None:
         self.assertEqual(
             tuple(self.qGraph.findTasksWithInput(DatasetTypeName("Dummy1Output")))[0], self.tasks[1]
         )
 
     def testFindTasksWithOutput(self) -> None:
@@ -494,15 +503,15 @@
     def testSaveLoadUri(self) -> None:
         uri = None
         try:
             with tempfile.NamedTemporaryFile(delete=False, suffix=".qgraph") as tmpFile:
                 uri = tmpFile.name
                 self.qGraph.saveUri(uri)
                 restore = QuantumGraph.loadUri(uri)
-                self.assertEqual(restore.metadata, METADATA)
+                self.assertEqual(restore.metadata, self.qGraph.metadata)
                 self.assertEqual(self.qGraph, restore)
                 nodeNumberId = random.randint(0, len(self.qGraph) - 1)
                 nodeNumber = [n.nodeId for n in self.qGraph][nodeNumberId]
                 restoreSub = QuantumGraph.loadUri(
                     uri, self.universe, nodes=(nodeNumber,), graphID=self.qGraph._buildId
                 )
                 self.assertEqual(len(restoreSub), 1)
@@ -576,26 +585,42 @@
         self.assertEqual(self.qGraph.graphID, graph_id)
         output_refs2 = get_output_refs(self.qGraph)
         self.assertEqual(len(output_refs2), len(output_refs))
         # All output dataset IDs must be updated.
         self.assertTrue(set(ref.id for ref in output_refs).isdisjoint(set(ref.id for ref in output_refs2)))
 
         # Also update metadata.
-        self.qGraph.updateRun("updated-run2", metadata_key="ouput_run")
+        self.qGraph.updateRun("updated-run2", metadata_key="output_run")
         self.assertEqual(check_output_run(self.qGraph, "updated-run2"), [])
         self.assertEqual(self.qGraph.graphID, graph_id)
         assert self.qGraph.metadata is not None
-        self.assertIn("ouput_run", self.qGraph.metadata)
-        self.assertEqual(self.qGraph.metadata["ouput_run"], "updated-run2")
+        self.assertIn("output_run", self.qGraph.metadata)
+        self.assertEqual(self.qGraph.metadata["output_run"], "updated-run2")
 
         # Update graph ID.
-        self.qGraph.updateRun("updated-run3", metadata_key="ouput_run", update_graph_id=True)
+        self.qGraph.updateRun("updated-run3", metadata_key="output_run", update_graph_id=True)
         self.assertEqual(check_output_run(self.qGraph, "updated-run3"), [])
         self.assertNotEqual(self.qGraph.graphID, graph_id)
 
+    def testMetadataPackage(self) -> None:
+        """Test package versions added to QuantumGraph metadata."""
+        packages = Packages.fromSystem()
+        self.assertFalse(self.qGraph.metadata["packages"].difference(packages))
+
+    def test_get_task_quanta(self) -> None:
+        for task_label in self.qGraph.pipeline_graph.tasks.keys():
+            quanta = self.qGraph.get_task_quanta(task_label)
+            self.assertCountEqual(quanta.values(), self.quanta_by_task_label[task_label])
+
+    def testGetSummary(self) -> None:
+        """Test for QuantumGraph.getSummary method."""
+        summary = self.qGraph.getSummary()
+        self.assertEqual(self.qGraph.graphID, summary.graphID)
+        self.assertEqual(len(summary.qgraphTaskSummaries), len(self.qGraph.taskGraph))
+
 
 class MyMemoryTestCase(lsst.utils.tests.MemoryTestCase):
     """Run file leak tests."""
 
 
 def setup_module(module) -> None:
     """Configure pytest."""
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_struct.py` & `lsst_pipe_base-27.0.0rc1/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `lsst-pipe-base-26.2024.900/tests/test_task.py` & `lsst_pipe_base-27.0.0rc1/tests/test_task.py`

 * *Files 5% similar despite different names*

```diff
@@ -135,20 +135,14 @@
         addend = self.config.addend
         return pipeBase.Struct(val=val + (2 * addend))
 
 
 class TaskTestCase(unittest.TestCase):
     """A test case for Task."""
 
-    def setUp(self):
-        self.valDict = dict()
-
-    def tearDown(self):
-        self.valDict = None
-
     def testBasics(self):
         """Test basic construction and use of a task."""
         for addend in (1.1, -3.5):
             for multiplicand in (0.9, -45.0):
                 config = AddMultTask.ConfigClass()
                 config.add.addend = addend
                 config.mult["stdMult"].multiplicand = multiplicand
@@ -321,14 +315,49 @@
             j = addMultTask.metadata.model_dump_json()
             new_meta = pipeBase.TaskMetadata.model_validate(json.loads(j))
         else:
             y = yaml.dump(addMultTask.metadata)
             new_meta = yaml.safe_load(y)
         self.assertEqual(new_meta, addMultTask.metadata)
 
+    def test_annotate_exception(self):
+        """Test annotating failures in the task metadata when a non-Task
+        exception is raised (when there is no `metadata` on the exception).
+        """
+        task = AddMultTask()
+        msg = "something failed!"
+        error = ValueError(msg)
+        with self.assertLogs("addMult", level="ERROR") as cm:
+            pipeBase.AnnotatedPartialOutputsError.annotate(error, task, log=task.log)
+        self.assertIn(msg, "\n".join(cm.output))
+        self.assertEqual(task.metadata["failure"]["message"], msg)
+        self.assertEqual(task.metadata["failure"]["type"], "ValueError")
+        self.assertNotIn("metadata", task.metadata["failure"])
+
+    def test_annotate_task_exception(self):
+        """Test annotating failures in the task metadata when a Task-specific
+        exception is raised.
+        """
+
+        class TestError(pipeBase.AlgorithmError):
+            @property
+            def metadata(self):
+                return {"something": 12345}
+
+        task = AddMultTask()
+        msg = "something failed!"
+        error = TestError(msg)
+        with self.assertLogs("addMult", level="ERROR") as cm:
+            pipeBase.AnnotatedPartialOutputsError.annotate(error, task, log=task.log)
+        self.assertIn(msg, "\n".join(cm.output))
+        self.assertEqual(task.metadata["failure"]["message"], msg)
+        result = "test_task.TaskTestCase.test_annotate_task_exception.<locals>.TestError"
+        self.assertEqual(task.metadata["failure"]["type"], result)
+        self.assertEqual(task.metadata["failure"]["metadata"]["something"], 12345)
+
 
 class MyMemoryTestCase(lsst.utils.tests.MemoryTestCase):
     """Run file leak tests."""
 
 
 def setup_module(module):
     """Configure pytest."""
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_taskmetadata.py` & `lsst_pipe_base-27.0.0rc1/tests/test_taskmetadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-import json
+import math
 import unittest
 
 try:
     import numpy
 except ImportError:
     numpy = None
 
@@ -179,29 +179,36 @@
 
         with self.assertRaises(ValueError):
             meta.add("int", ["string", "array"])
 
         with self.assertRaises(ValueError):
             meta["mixed"] = [1, "one"]
 
+    def test_nan(self):
+        """Check that NaN round trips as a NaN."""
+        meta = TaskMetadata()
+        meta["nan"] = float("NaN")
+        new_meta = TaskMetadata.model_validate_json(meta.model_dump_json())
+        self.assertTrue(math.isnan(new_meta["nan"]))
+
     def testDict(self):
         """Construct a TaskMetadata from a dictionary."""
         d = {"a": "b", "c": 1, "d": [1, 2], "e": {"f": "g", "h": {"i": [3, 4]}}}
 
         meta = TaskMetadata.from_dict(d)
         self.assertEqual(meta["a"], "b")
         self.assertEqual(meta["e.f"], "g")
         self.assertEqual(meta.getArray("d"), [1, 2])
         self.assertEqual(meta["e.h.i"], 4)
 
         d2 = meta.to_dict()
         self.assertEqual(d2, d)
 
         j = meta.model_dump_json()
-        meta2 = TaskMetadata.model_validate(json.loads(j))
+        meta2 = TaskMetadata.model_validate_json(j)
         self.assertEqual(meta2, meta)
 
         # Round trip.
         meta3 = TaskMetadata.from_metadata(meta)
         self.assertEqual(meta3, meta)
 
         # Add a new element that would be a single-element array.
```

### Comparing `lsst-pipe-base-26.2024.900/tests/test_testUtils.py` & `lsst_pipe_base-27.0.0rc1/tests/test_testUtils.py`

 * *Files identical despite different names*

