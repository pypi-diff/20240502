# Comparing `tmp/discopop-3.1.1.tar.gz` & `tmp/discopop-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discopop-3.1.1.tar", last modified: Wed Jan 17 10:29:47 2024, max compression
+gzip compressed data, was "discopop-3.2.0.tar", last modified: Thu May  2 12:46:22 2024, max compression
```

## Comparing `discopop-3.1.1.tar` & `discopop-3.2.0.tar`

### file list

```diff
@@ -1,366 +1,518 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.092188 discopop-3.1.1/DEPRECATED_discopop_profiler/
--rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_profiler/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_profiler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.092188 discopop-3.1.1/DEPRECATED_discopop_wizard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.092188 discopop-3.1.1/DEPRECATED_discopop_wizard/assets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/assets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.092188 discopop-3.1.1/DEPRECATED_discopop_wizard/assets/icons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/assets/icons/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.092188 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/CodePreview.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Console.py
--rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/ExecutionConfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Pragma.py
--rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/ProfilingContainer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Suggestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/TKVarStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/DEPRECATED_discopop_wizard/headless/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/headless/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/headless/headless_execution.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/optimizer/binding.py
--rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/suggestions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/suggestions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/suggestions/overview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/widgets/ScrollableText.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/screens/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-01-17 10:29:46.000000 discopop-3.1.1/DEPRECATED_discopop_wizard/wizard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-01-17 10:29:46.000000 discopop-3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-17 10:29:46.000000 discopop-3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-17 10:29:47.124188 discopop-3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-01-17 10:29:46.000000 discopop-3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/discopop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15938 2024-01-17 10:29:47.000000 discopop-3.1.1/discopop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      507 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/discopop_explorer/
--rw-r--r--   0 runner    (1001) docker     (127)    66229 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/PEGraphX.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7847 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8670 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/discopop_explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/generate_Data_CUInst.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/parallel_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     7287 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.096188 discopop-3.1.1/discopop_explorer/pattern_detectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/PatternBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/PatternInfo.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.100188 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)    22504 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/CombinedGPURegions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.100188 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/EntryPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/ExitPoint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/combined_gpu_pattern_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/prepare_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_1.py
--rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_2.py
--rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_3.py
--rw-r--r--   0 runner    (1001) docker     (127)    34261 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_4.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_5.py
--rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_6.py
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/device_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10240 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/do_all_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/geometric_decomposition_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7991 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/pipeline_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)     7885 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/reduction_detector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.100188 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/
--rw-r--r--   0 runner    (1001) docker     (127)    30160 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPULoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPUMemory.py
--rw-r--r--   0 runner    (1001) docker     (127)    23684 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPURegions.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/gpu_pattern_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16587 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/alias_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    35613 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (127)    20640 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (127)    23094 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/barriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/data_sharing_clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/dependency_clauses.py
--rw-r--r--   0 runner    (1001) docker     (127)    20787 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8068 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/task_parallelism_detector.py
--rw-r--r--   0 runner    (1001) docker     (127)    31607 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/tp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_explorer/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/plugins/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_explorer/test/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    34170 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_explorer/variable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/CodeGenerator/
--rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/CodeGenerator.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/CodeGeneratorArguments.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/CodeGenerator/classes/
--rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/classes/ContentBuffer.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/classes/Enums.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/classes/Line.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/classes/Pragma.py
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/classes/UnpackedSuggestion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/CodeGenerator/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/ConfigProvider/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/ConfigProvider/ConfigProviderArguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     1854 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/ConfigProvider/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/ConfigProvider/assets/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/ConfigProvider/assets/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/ConfigProvider/config_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/JSONHandler/
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/JSONHandler/JSONHandler.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/JSONHandler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/LineMapping/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/LineMapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/LineMapping/diff_modifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/LineMapping/initialize.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/LineMapping/load.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/LineMapping/save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.104188 discopop-3.1.1/discopop_library/MemoryRegions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/MemoryRegions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/MemoryRegions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/PatchApplicator/
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/PatchApplicatorArguments.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3043 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/clear.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/patch_applicator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchApplicator/rollback.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/PatchGenerator/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/PatchGeneratorArguments.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/diffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2904 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/from_json_patterns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/from_optimizer_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatchGenerator/patch_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/PathManagement/
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PathManagement/PathManagement.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PathManagement/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/PatternIdManagement/
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/PatternIdManagement/unique_pattern_id.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/discopop_optimizer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/CostModel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/DataTransfer/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/DataTransfer/DataTransferCosts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/DataTransfer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16958 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.108188 discopop-3.1.1/discopop_library/discopop_optimizer/DataTransfers/
--rw-r--r--   0 runner    (1001) docker     (127)    11655 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/DataTransfers/DataTransfers.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/DataTransfers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/
--rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/DelaunayInterpolatedMicrobench.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/ExtrapInterpolatedMicrobench.py
--rw-r--r--   0 runner    (1001) docker     (127)     3760 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/Microbench.py
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/MicrobenchParser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/MixedMicrobench.py
--rw-r--r--   0 runner    (1001) docker     (127)     7971 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/PureDataMicrobench.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10325 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/OptimizationGraph.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/OptimizerArguments.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/DataAccesses/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/DataAccesses/CalculateUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/DataAccesses/FromCUs.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/DataAccesses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36357 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/PETParser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/LoopInitializationUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/RemoveDuplicatedUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/RemoveLoopIndexUpdates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/Variables/
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Variables/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Variables/ExperimentUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/Variables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3561 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/bindings/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/bindings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/bindings/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.112188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/
--rw-r--r--   0 runner    (1001) docker     (127)    13031 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/ContextObject.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/ContextObjectUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4010 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/Update.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/ChildEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/DataFlowEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/GenericEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/MutuallyExclusiveEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/OptionEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/RequirementEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/SuccessorEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/TemporaryEdge.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/enums/Distributions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/enums/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextMerge.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextRestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextSave.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshotPop.py
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/FunctionRoot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/GenericNode.py
--rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/Loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/Workload.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/
--rw-r--r--   0 runner    (1001) docker     (127)     2865 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/Network.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/System.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/CPU.py
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/Device.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/DeviceTypeEnum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/GPU.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/system_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/classes/types/
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/types/Aliases.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/types/DataAccessType.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/classes/types/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/gui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.116188 discopop-3.1.1/discopop_library/discopop_optimizer/gui/plotting/
--rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/plotting/CostModels.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/plotting/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/gui/presentation/
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/presentation/ChoiceDetails.py
--rw-r--r--   0 runner    (1001) docker     (127)    11200 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/presentation/OptionTable.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/presentation/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/gui/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/queries/ValueTableQuery.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/queries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/gui/widgets/
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/widgets/ScrollableFrame.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/gui/widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     6215 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/optimization/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/optimization/evaluate_all_decision_combinations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/optimization/evolutionary_algorithm.py
--rw-r--r--   0 runner    (1001) docker     (127)     6165 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/optimization/validation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/scheduling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/scheduling/workload_delta.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9134 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/do_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     8540 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/reduction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/optimizers/
--rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/optimizers/loop_collapse.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/optimizers/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/MOGUtilities.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/
--rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/RandomSamples.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/
--rw-r--r--   0 runner    (1001) docker     (127)     8823 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/TopDown.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/simple_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.120188 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/visualization/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/visualization/plotting.py
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/discopop_optimizer/utilities/visualization/update_graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/discopop_library/global_data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/discopop_library/global_data/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/discopop_library/global_data/version/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/version/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/version/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/discopop_library/global_data/version/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/version/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/version/__pycache__/utils.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/global_data/version/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/discopop_library/result_classes/
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/result_classes/DetectionResult.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/result_classes/OptimizerOutputPattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/result_classes/PatternStorage.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/discopop_library/result_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-01-17 10:29:46.000000 discopop-3.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-17 10:29:47.124188 discopop-3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-01-17 10:29:46.000000 discopop-3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/do_all/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/do_all/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/do_all/daxpy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/do_all/daxpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-01-17 10:29:46.000000 discopop-3.1.1/test/do_all/daxpy/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/optimizer/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/optimizer/loop_collapse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/optimizer/loop_collapse/negative/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/negative/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/optimizer/loop_collapse/negative/simple_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/negative/simple_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/negative/simple_1/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/optimizer/loop_collapse/positive/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/positive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/optimizer/loop_collapse/positive/simple_1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/positive/simple_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-01-17 10:29:46.000000 discopop-3.1.1/test/optimizer/loop_collapse/positive/simple_1/test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:47.124188 discopop-3.1.1/test/utils/validator_classes/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-01-17 10:29:46.000000 discopop-3.1.1/test/utils/validator_classes/DoAllInfoForValidation.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 10:29:46.000000 discopop-3.1.1/test/utils/validator_classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_profiler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3848 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_profiler/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_profiler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/assets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/assets/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/assets/icons/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4142 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/CodePreview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Console.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19153 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/ExecutionConfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Pragma.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6608 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/ProfilingContainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6224 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/TKVarStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/headless/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/headless/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/headless/headless_execution.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5050 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6571 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/optimizer/binding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7799 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/suggestions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/suggestions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6419 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/suggestions/overview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.200863 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/widgets/ScrollableText.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/screens/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2174 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-02 12:46:21.000000 discopop-3.2.0/DEPRECATED_discopop_wizard/wizard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-02 12:46:21.000000 discopop-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 12:46:21.000000 discopop-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:46:22.240863 discopop-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4608 2024-05-02 12:46:21.000000 discopop-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.204863 discopop-3.2.0/discopop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21639 2024-05-02 12:46:22.000000 discopop-3.2.0/discopop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      507 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.204863 discopop-3.2.0/discopop_explorer/
+-rw-r--r--   0 runner    (1001) docker     (127)    67834 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/PEGraphX.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8538 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10547 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/discopop_explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9006 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/generate_Data_CUInst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/parallel_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.204863 discopop-3.2.0/discopop_explorer/pattern_detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/PatternBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/PatternInfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.204863 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)    22512 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/CombinedGPURegions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5473 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/EntryPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/ExitPoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12780 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/combined_gpu_pattern_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1619 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/prepare_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_1.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14460 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7811 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34261 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_4.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16902 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_6.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/device_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14089 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/do_all_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7290 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/geometric_decomposition_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8123 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/pipeline_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8035 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/reduction_detector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/
+-rw-r--r--   0 runner    (1001) docker     (127)    30160 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPULoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6601 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPUMemory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23684 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPURegions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/gpu_pattern_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16587 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/alias_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7120 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35613 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6946 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20640 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13383 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23094 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/barriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2838 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/data_sharing_clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57649 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/dependency_clauses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20787 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/task_parallelism_detector.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31607 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/tp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_explorer/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5839 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/plugins/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_explorer/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36170 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_explorer/variable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_library/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_library/ArgumentClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/ArgumentClasses/GeneralArguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.208863 discopop-3.2.0/discopop_library/CodeGenerator/
+-rw-r--r--   0 runner    (1001) docker     (127)     8926 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/CodeGenerator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/CodeGeneratorArguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/CodeGenerator/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)    10845 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/classes/ContentBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/classes/Enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/classes/Line.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/classes/Pragma.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22552 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/classes/UnpackedSuggestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/CodeGenerator/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/ConfigProvider/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/ConfigProvider/ConfigProviderArguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1865 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/ConfigProvider/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/ConfigProvider/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/ConfigProvider/assets/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/ConfigProvider/config_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/GlobalLogger/
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/GlobalLogger/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/HostpotLoader/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/HostpotLoader/HotspotLoaderArguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/HostpotLoader/HotspotNodeType.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/HostpotLoader/HotspotType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/HostpotLoader/hostpot_loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/JSONHandler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/JSONHandler/JSONHandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/JSONHandler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/LineMapping/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/LineMapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5572 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/LineMapping/diff_modifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/LineMapping/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/LineMapping/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/LineMapping/save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/MemoryRegions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/MemoryRegions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/MemoryRegions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/PatchApplicator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/PatchApplicatorArguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3428 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6484 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/clear.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/patch_applicator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6661 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchApplicator/rollback.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/PatchGenerator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/PatchGeneratorArguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4176 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/diffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/from_json_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4570 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/from_optimizer_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatchGenerator/patch_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.212863 discopop-3.2.0/discopop_library/PathManagement/
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PathManagement/PathManagement.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PathManagement/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/PatternIdManagement/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/PatternIdManagement/unique_pattern_id.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/CostModel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/DataTransfer/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/DataTransfer/DataTransferCosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/DataTransfer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19766 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/
+-rw-r--r--   0 runner    (1001) docker     (127)    16001 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/DataTransfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23296 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/NewDataTransfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/calculate_configuration_data_movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4784 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/prepare_force_branch_end_data_movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/prepare_forced_data_movement.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/prepare_forced_data_movement_prior_to_call.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     3276 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/DelaunayInterpolatedMicrobench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3756 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/ExtrapInterpolatedMicrobench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/Microbench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/MicrobenchParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2340 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/MixedMicrobench.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7997 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/PureDataMicrobench.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10327 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/OptimizationGraph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/OptimizerArguments.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/DataAccesses/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/DataAccesses/CalculateUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/DataAccesses/FromCUs.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/DataAccesses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73054 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/PETParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.216863 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/AddRangesToUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/LoopInitializationUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6239 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/RemoveDuplicatedUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/RemoveLoopIndexUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/RemoveSameDeviceUpdates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2986 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/Variables/
+-rw-r--r--   0 runner    (1001) docker     (127)     5728 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Variables/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9918 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Variables/ExperimentUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/Variables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/bindings/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/bindings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/bindings/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/ContextObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/ContextObjectUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/Update.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/CallEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/ChildEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/DataFlowEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/GenericEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/MutuallyExclusiveEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/OptionEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/RequirementEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/SuccessorEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/TemporaryEdge.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/enums/Distributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/enums/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.220863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextMerge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextRestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextSave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshotPop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/DeviceSwitch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/FunctionReturn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/FunctionRoot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/GenericNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5779 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/Loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/SynchronizationTrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/Workload.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/
+-rw-r--r--   0 runner    (1001) docker     (127)     3002 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/Network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8638 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/System.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/CPU.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/Device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/DeviceTypeEnum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/GPU.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/system_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/classes/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/types/Aliases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/types/DataAccessType.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/classes/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/gui/plotting/
+-rw-r--r--   0 runner    (1001) docker     (127)    16066 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/plotting/CostModels.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/plotting/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/gui/presentation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/presentation/ChoiceDetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/presentation/OptionTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/presentation/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/gui/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/queries/ValueTableQuery.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/queries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/gui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/widgets/ScrollableFrame.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/gui/widgets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/interactive/
+-rw-r--r--   0 runner    (1001) docker     (127)     8562 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/interactive/interactive_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/optimization/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8685 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/optimization/evaluate_all_decision_combinations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18605 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/optimization/evolutionary_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10545 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/optimization/greedy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/optimization/validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14083 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10278 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/scheduling/workload_delta.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.224863 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13189 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/do_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8738 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/reduction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (127)    15007 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/optimizers/loop_collapse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/optimizers/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)    29289 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/MOGUtilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6691 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/insert_device_switch_nodes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     4770 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/RandomSamples.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     8908 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/TopDown.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/simple_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/visualization/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6704 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/visualization/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/discopop_optimizer/utilities/visualization/update_graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/global_data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/global_data/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/global_data/version/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/version/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/version/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/global_data/version/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/version/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/version/__pycache__/utils.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/global_data/version/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/discopop_library/result_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/result_classes/DetectionResult.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/result_classes/MergedPattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3461 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/result_classes/OptimizerOutputPattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/result_classes/PatternStorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/discopop_library/result_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-02 12:46:21.000000 discopop-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 12:46:22.240863 discopop-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-02 12:46:21.000000 discopop-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/test/do_all/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/test/do_all/backwards_array_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/backwards_array_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2704 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/backwards_array_access/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.228863 discopop-3.2.0/test/do_all/calls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/allowing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/allowing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/allowing/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/preventing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/preventing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/preventing/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/preventing/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/preventing/simple/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/second_order/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/second_order/allowing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/allowing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/allowing/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/second_order/allowing_2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/allowing_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/allowing_2/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/second_order/preventing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/preventing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/preventing/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/calls/second_order/preventing_2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/preventing_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/calls/second_order/preventing_2/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/daxpy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/daxpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/daxpy/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/negative/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/negative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/negative/nested/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/negative/nested/OMPSCR/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/negative/nested/OMPSCR/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/negative/nested/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/global_vars/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_arrays/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_arrays/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_arrays/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_struct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_struct/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_vectors/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_vectors_and_struct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_vectors_and_struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/global_vars/miniFE_CSRMatrix_proxy/global_vectors_and_struct/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/nested/depth_2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/both_loops_doall/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/both_loops_doall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/both_loops_doall/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.232863 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/inner_loop_doall/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/inner_loop_doall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/inner_loop_doall/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/outer_loop_doall/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/outer_loop_doall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/nested/depth_2/positive/outer_loop_doall/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/simple/not_nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/simple/not_nested/negative/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/negative/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/simple/not_nested/negative/minimal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/negative/minimal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/negative/minimal/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/simple/not_nested/negative/stack_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/negative/stack_access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/negative/stack_access/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/simple/not_nested/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/positive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/simple/not_nested/positive/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/nested/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/nested/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/nested/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/nested/positive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/nested/positive/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/case_0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_0/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/case_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/case_2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_2/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/case_3/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_3/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/case_4/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_4/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_4/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/stack_access/various/case_5/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/stack_access/various/case_5/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/struct/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/access_outside_struct/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/access_outside_struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/access_outside_struct/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/std_data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/std_data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/std_data_types/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/template_data_types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/template_data_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-02 12:46:21.000000 discopop-3.2.0/test/do_all/struct/positive/miniFE_CSRMatrix_proxy/template_data_types/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.236863 discopop-3.2.0/test/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/optimizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/optimizer/loop_collapse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/optimizer/loop_collapse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/optimizer/loop_collapse/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/optimizer/loop_collapse/positive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/optimizer/loop_collapse/positive/simple_1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/optimizer/loop_collapse/positive/simple_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-02 12:46:21.000000 discopop-3.2.0/test/optimizer/loop_collapse/positive/simple_1/test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/reduction_pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/reduction_pattern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/reduction_pattern/positive/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/reduction_pattern/positive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/reduction_pattern/positive/nested/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/reduction_pattern/positive/nested/OMPSCR/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/reduction_pattern/positive/nested/OMPSCR/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/reduction_pattern/positive/nested/OMPSCR/c_Mandelbrot/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/reduction_pattern/positive/nested/OMPSCR/c_Mandelbrot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-02 12:46:21.000000 discopop-3.2.0/test/reduction_pattern/positive/nested/OMPSCR/c_Mandelbrot/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/reduction_pattern/positive/nested/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:22.240863 discopop-3.2.0/test/utils/validator_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-02 12:46:21.000000 discopop-3.2.0/test/utils/validator_classes/DoAllInfoForValidation.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 12:46:21.000000 discopop-3.2.0/test/utils/validator_classes/__init__.py
```

### Comparing `discopop-3.1.1/DEPRECATED_discopop_profiler/__init__.py` & `discopop-3.2.0/DEPRECATED_discopop_profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_profiler/__main__.py` & `discopop-3.2.0/DEPRECATED_discopop_profiler/__main__.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_profiler/utils.py` & `discopop-3.2.0/DEPRECATED_discopop_profiler/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/__main__.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/__main__.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/CodePreview.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/CodePreview.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Console.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Console.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/ExecutionConfiguration.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/ExecutionConfiguration.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Pragma.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Pragma.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/ProfilingContainer.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/ProfilingContainer.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Settings.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Settings.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/Suggestion.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/Suggestion.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/classes/TKVarStorage.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/classes/TKVarStorage.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/headless/headless_execution.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/headless/headless_execution.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/execution.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/execution.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/main.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/main.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/optimizer/binding.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/optimizer/binding.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/settings.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/settings.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/suggestions/overview.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/suggestions/overview.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/utils.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/screens/widgets/ScrollableText.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/screens/widgets/ScrollableText.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/utils.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/DEPRECATED_discopop_wizard/wizard.py` & `discopop-3.2.0/DEPRECATED_discopop_wizard/wizard.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/LICENSE` & `discopop-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/MANIFEST.in` & `discopop-3.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/PKG-INFO` & `discopop-3.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discopop
-Version: 3.1.1
+Version: 3.2.0
 Summary: DiscoPoP is a tool that helps software developers parallelize their programs with threads. It discovers potential parallelism in a sequential program and makes recommendations on how to exploit it.
 Home-page: https://www.discopop.tu-darmstadt.de/
 Author: TU Darmstadt and Iowa State University
 Author-email: discopop@lists.parallel.informatik.tu-darmstadt.de
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `discopop-3.1.1/README.md` & `discopop-3.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,78 +8,78 @@
  * the 3-Clause BSD License. See the LICENSE file in the package base
  * directory for details.
  *
  */
  -->
 
 # DiscoPoP - Discovery of Potential Parallelism
-DiscoPoP is an open-source tool that helps software developers parallelize their programs with threads. It is a joint project of the [Laboratory for Parallel Programming @ TU Darmstadt](https://github.com/tuda-parallel) and the Iowa State University.
+DiscoPoP is an open-source tool that helps software developers parallelize their programs with threads. It is a joint project of the [Laboratory for Parallel Programming @ TU Darmstadt](https://github.com/tuda-parallel) and the [Software Analytics and Pervasive Parallelism Lab](https://www.cs.iastate.edu/swapp/) at Iowa State University.
 
 In a nutshell, DiscoPoP performs the following steps:
 * detect parts of the code (computational units or CUs) with little to no internal parallelization potential,
 * find data dependences among them,
 * identify parallel patterns that can be used to parallelize a code region,
-* and finally suggest corresponding OpenMP parallelization constructs and clauses to programmers.
+* and finally, suggest corresponding OpenMP parallelization constructs and clauses to programmers.
 
-DiscoPoP is built on top of LLVM. Therefore, DiscoPoP can perform the above-mentioned steps on any source code which can be transferred into the LLVM IR.
+DiscoPoP is built on top of LLVM. Therefore, DiscoPoP can perform the above-mentioned steps on any source code that can be transferred into the LLVM IR.
 
 A more comprehensive overview of DiscoPoP can be found on our [project website](https://www.discopop.tu-darmstadt.de/).
 
 ## Getting started
 Follow the steps in [setup](https://discopop-project.github.io/discopop/setup/discopop/) to install DiscoPoP.
 To setup the [Visual Studio Code Extension](https://marketplace.visualstudio.com/items?itemName=TUDarmstadt-LaboratoryforParallelProgramming.discopop) (recommended for general use of the framework), please follow [these steps](https://discopop-project.github.io/discopop/setup/vscx/).
 
-For a brief introduction into the [VSCode Extension](https://marketplace.visualstudio.com/items?itemName=TUDarmstadt-LaboratoryforParallelProgramming.discopop), please follow the [walk-through example](https://discopop-project.github.io/discopop/examples/walk_through_gui/).
-For a brief introduction into the command line tools, please refer to the [tools overview](https://discopop-project.github.io/discopop/Tools) and follow the [command-line walk-through example](https://discopop-project.github.io/discopop/examples/walk_through/).
+For a brief introduction to the [VSCode Extension](https://marketplace.visualstudio.com/items?itemName=TUDarmstadt-LaboratoryforParallelProgramming.discopop), please follow the [walk-through example](https://discopop-project.github.io/discopop/examples/walk_through_gui/).
+For a brief introduction to the command line tools, please refer to the [tools overview](https://discopop-project.github.io/discopop/Tools) and follow the [command-line walk-through example](https://discopop-project.github.io/discopop/examples/walk_through/).
 
 For detailed information on the gathered and stored data as well as the tools themselves, please refer to [data](https://discopop-project.github.io/discopop/Data) and the pages of the individual tools in the [tools overview](https://discopop-project.github.io/discopop/Tools).
 
 ## TL;DR
-This example installs DiscoPoP, instruments and builds the provided example, analyzes the results and prints the identified parallelization suggestions to the console.
+This example installs DiscoPoP, instruments and builds the provided example, analyzes the results, and prints the identified parallelization suggestions to the console.
 In case any issues arise during the process, please refer to the detailed [setup instructions](https://discopop-project.github.io/discopop/Setup), contact us via GitHub messages, or get in contact by mail to [discopop-support@lists.parallel.informatik.tu-darmstadt.de](mailto:discopop-support@lists.parallel.informatik.tu-darmstadt.de).
 ```
 # setup DiscoPoP
 git clone git@github.com:discopop-project/discopop.git
 cd discopop
 mkdir build && cd build
 DP_BUILD=$(pwd)
-cmake .. && make 
+cmake .. && make
 # instrument and build the example code
 cd ../example
 mkdir build && cd build && cmake -DCMAKE_CXX_COMPILER=${DP_BUILD}/scripts/CXX_wrapper.sh .. && make
 # execute instrumented code
 ./cmake_example
 # identify parallel patterns
 cd .discopop
 discopop_explorer
 # create applicable patches from patterns
 discopop_patch_generator
 # print patches to the console
 for f in $(find patch_generator -maxdepth 1 -type d); do
     echo "SUGGESTION: $f"
-    cat $f/1.patch 
+    cat $f/1.patch
     echo ""
 done
 # apply patch with id 1
 discopop_patch_applicator -a 1
 # reset code to the original state
 discopop_patch_applicator -C
 ```
 
 
 ## Exemplary output
-The following is an automatically generated, exemplary output patch file generated and applicable as show in the provided [examples](https://discopop-project.github.io/discopop/Examples).
+The following is an automatically generated, exemplary output patch file generated and applicable as shown in the provided [examples](https://discopop-project.github.io/discopop/Examples).
 ```
  --- /home/lukas/temp/discopop_tmp/discopop/example/example.cpp	2024-01-09 10:11:50.369555235 +0100
 +++ /home/lukas/temp/discopop_tmp/discopop/example/example.cpp.discopop_patch_generator.temp	2024-01-09 11:14:20.904823624 +0100
 @@ -20,6 +20,7 @@
          Arr[i] = i % 13;
      }
- 
-+    #pragma omp parallel for shared(Arr,N) reduction(+:sum) 
+
++    #pragma omp parallel for shared(Arr,N) reduction(+:sum)
      for(int i = 0; i < N; i++){
          sum += Arr[i];
      }
 ```
 
 ## License
-© DiscoPoP is available under the terms of the BSD-3-Clause license, as specified in the LICENSE file.
+© DiscoPoP is available under the terms of the BSD-3-Clause license, as specified in the LICENSE file.
```

### Comparing `discopop-3.1.1/discopop.egg-info/PKG-INFO` & `discopop-3.2.0/discopop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discopop
-Version: 3.1.1
+Version: 3.2.0
 Summary: DiscoPoP is a tool that helps software developers parallelize their programs with threads. It discovers potential parallelism in a sequential program and makes recommendations on how to exploit it.
 Home-page: https://www.discopop.tu-darmstadt.de/
 Author: TU Darmstadt and Iowa State University
 Author-email: discopop@lists.parallel.informatik.tu-darmstadt.de
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `discopop-3.1.1/discopop_explorer/PEGraphX.py` & `discopop-3.2.0/discopop_explorer/PEGraphX.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,17 @@
 from enum import IntEnum, Enum
 from typing import Dict, List, Sequence, Tuple, Set, Optional, Type, TypeVar, cast, Union, overload, Any
 
 import jsonpickle  # type:ignore
 import matplotlib.pyplot as plt  # type:ignore
 import networkx as nx  # type:ignore
 from alive_progress import alive_bar  # type: ignore
-from lxml.objectify import ObjectifiedElement  # type:ignore
+from lxml.objectify import ObjectifiedElement  # type: ignore
+
+from discopop_library.HostpotLoader.HotspotNodeType import HotspotNodeType  # type:ignore
 
 from .parser import LoopData, readlineToCUIdMap, writelineToCUIdMap, DependenceItem
 from .variable import Variable
 
 global_pet = None
 
 # unused
@@ -154,17 +156,17 @@
     id: NodeID
     file_id: int
     node_id: int
     start_line: int
     end_line: int
     type: NodeType
     name: str
-    parent_function_id: Optional[
-        NodeID
-    ] = None  # metadata to speedup some calculations (TODO FunctionNodes have themselves as parent)
+    parent_function_id: Optional[NodeID] = (
+        None  # metadata to speedup some calculations (TODO FunctionNodes have themselves as parent)
+    )
     workload: Optional[int] = None
 
     # properties of CU Nodes
     node_calls: List[Dict[str, str]] = []
     recursive_function_calls: List[str] = []
 
     # properties related to pattern analysis
@@ -689,16 +691,14 @@
         for node_id in [n.id for n in self.all_nodes(CUNode)]:
             out_deps = [(s, t, d) for s, t, d in self.out_edges(node_id) if d.etype == EdgeType.DATA]
 
             # for outgoing dependencies, the scope must be equal
             # as a result, comparing variable names to match memory regions is valid
             for _, _, d1 in out_deps:
                 for _, _, d2 in out_deps:
-                    if d1 == d2:
-                        continue
                     if d1.var_name == d2.var_name:
                         if d1.memory_region != d2.memory_region:
                             if d1.memory_region not in mem_reg_mappings:
                                 mem_reg_mappings[d1.memory_region] = set()
                             if d2.memory_region not in mem_reg_mappings:
                                 mem_reg_mappings[d2.memory_region] = set()
                             mem_reg_mappings[d1.memory_region].add(d2.memory_region)
@@ -720,18 +720,34 @@
                         ]:
                             edge_data = copy.deepcopy(d)
                             edge_data.memory_region = dynamic_mapping
                             self.g.add_edge(s, t, data=edge_data)
 
         print("Done.")
 
-    def calculateFunctionMetadata(self) -> None:
+    def calculateFunctionMetadata(self, hotspot_information=None, func_nodes=None) -> None:
         # store id of parent function in each node
         # and store in each function node a list of all children ids
-        func_nodes = self.all_nodes(FunctionNode)
+        if func_nodes is None:
+            func_nodes = self.all_nodes(FunctionNode)
+
+            if hotspot_information is not None:
+                all_hotspot_functions: Set[Tuple[int, str]] = set()
+                for key in hotspot_information:
+                    for entry in hotspot_information[key]:
+                        if entry[2] == HotspotNodeType.FUNCTION:
+                            all_hotspot_functions.add((entry[0], entry[3]))
+
+                filtered_func_nodes = [
+                    func_node
+                    for func_node in func_nodes
+                    if (func_node.file_id, func_node.name) in all_hotspot_functions
+                ]
+                func_nodes = filtered_func_nodes
+
         print("Calculating local metadata results for functions...")
         import tqdm  # type: ignore
         from multiprocessing import Pool
         from .parallel_utils import pet_function_metadata_initialize_worker, pet_function_metadata_parse_func
 
         param_list = func_nodes
         with Pool(initializer=pet_function_metadata_initialize_worker, initargs=(self,)) as pool:
@@ -748,45 +764,47 @@
             # set parent function for visited nodes
             for child_id in local_children_ids:
                 self.node_at(child_id).parent_function_id = parsed_function_id
 
         print("\tMetadata calculation done.")
 
         # cleanup dependencies (remove dependencies, if it is overwritten by a more specific Intra-iteration dependency
-        print("Cleaning duplicated dependencies...")
-        to_be_removed = []
-        for cu_node in self.all_nodes(CUNode):
-            out_deps = self.out_edges(cu_node.id, EdgeType.DATA)
-            for dep_1 in out_deps:
-                for dep_2 in out_deps:
-                    if dep_1 == dep_2:
-                        continue
-                    if (
-                        dep_1[2].dtype == dep_2[2].dtype
-                        and dep_1[2].etype == dep_2[2].etype
-                        and dep_1[2].memory_region == dep_2[2].memory_region
-                        and dep_1[2].sink_line == dep_2[2].sink_line
-                        and dep_1[2].source_line == dep_2[2].source_line
-                        and dep_1[2].var_name == dep_2[2].var_name
-                    ):
-                        if not dep_1[2].intra_iteration and dep_2[2].intra_iteration:
-                            # dep_2 is a more specific duplicate of dep_1
-                            # remove dep_1
-                            to_be_removed.append(dep_1)
-
-        to_be_removed_with_keys = []
-        for dep in to_be_removed:
-            graph_edges = self.g.out_edges(dep[0], keys=True, data="data")
-
-            for s, t, key, data in graph_edges:
-                if dep[0] == s and dep[1] == t and dep[2] == data:
-                    to_be_removed_with_keys.append((s, t, key))
-        for edge in set(to_be_removed_with_keys):
-            self.g.remove_edge(edge[0], edge[1], edge[2])
-        print("Cleaning dependencies done.")
+        # note: this can introduce false positives! Keep the analysis pessimistic to ensure correctness
+        if False:
+            print("Cleaning duplicated dependencies...")
+            to_be_removed = []
+            for cu_node in self.all_nodes(CUNode):
+                out_deps = self.out_edges(cu_node.id, EdgeType.DATA)
+                for dep_1 in out_deps:
+                    for dep_2 in out_deps:
+                        if dep_1 == dep_2:
+                            continue
+                        if (
+                            dep_1[2].dtype == dep_2[2].dtype
+                            and dep_1[2].etype == dep_2[2].etype
+                            and dep_1[2].memory_region == dep_2[2].memory_region
+                            and dep_1[2].sink_line == dep_2[2].sink_line
+                            and dep_1[2].source_line == dep_2[2].source_line
+                            and dep_1[2].var_name == dep_2[2].var_name
+                        ):
+                            if not dep_1[2].intra_iteration and dep_2[2].intra_iteration:
+                                # dep_2 is a more specific duplicate of dep_1
+                                # remove dep_1
+                                to_be_removed.append(dep_1)
+
+            to_be_removed_with_keys = []
+            for dep in to_be_removed:
+                graph_edges = self.g.out_edges(dep[0], keys=True, data="data")
+
+                for s, t, key, data in graph_edges:
+                    if dep[0] == s and dep[1] == t and dep[2] == data:
+                        to_be_removed_with_keys.append((s, t, key))
+            for edge in set(to_be_removed_with_keys):
+                self.g.remove_edge(edge[0], edge[1], edge[2])
+            print("Cleaning dependencies done.")
 
         # cleanup dependencies II : only consider the Intra-iteration dependencies with the highest level
         print("Cleaning duplicated dependencies II...")
         to_be_removed = []
         for cu_node in self.all_nodes(CUNode):
             out_deps = self.out_edges(cu_node.id, EdgeType.DATA)
             for dep_1 in out_deps:
@@ -937,20 +955,18 @@
         """
         return cast(Node, self.g.nodes[node_id]["data"])
 
     # generic type for subclasses of Node
     NodeT = TypeVar("NodeT", bound=Node)
 
     @overload
-    def all_nodes(self) -> List[Node]:
-        ...
+    def all_nodes(self) -> List[Node]: ...
 
     @overload
-    def all_nodes(self, type: Union[Type[NodeT], Tuple[Type[NodeT], ...]]) -> List[NodeT]:
-        ...
+    def all_nodes(self, type: Union[Type[NodeT], Tuple[Type[NodeT], ...]]) -> List[NodeT]: ...
 
     def all_nodes(self, type=Node):
         """List of all nodes of specified type
 
         :param type: type(s) of nodes
         :return: List of all nodes
         """
@@ -985,39 +1001,35 @@
             return [t for t in self.g.in_edges(node_id, data="data")]
         elif type(etype) == list:
             return [t for t in self.g.in_edges(node_id, data="data") if t[2].etype in etype]
         else:
             return [t for t in self.g.in_edges(node_id, data="data") if t[2].etype == etype]
 
     @overload
-    def subtree_of_type(self, root: Node) -> List[Node]:
-        ...
+    def subtree_of_type(self, root: Node) -> List[Node]: ...
 
     @overload
-    def subtree_of_type(self, root: Node, type: Union[Type[NodeT], Tuple[Type[NodeT], ...]]) -> List[NodeT]:
-        ...
+    def subtree_of_type(self, root: Node, type: Union[Type[NodeT], Tuple[Type[NodeT], ...]]) -> List[NodeT]: ...
 
     def subtree_of_type(self, root, type=Node):
         """Gets all nodes in subtree of specified type including root
 
         :param root: root node
         :param type: type of children, None is equal to a wildcard
         :return: list of nodes in subtree
         """
         return self.subtree_of_type_rec(root, set(), type)
 
     @overload
-    def subtree_of_type_rec(self, root: Node, visited: Set[Node]) -> List[Node]:
-        ...
+    def subtree_of_type_rec(self, root: Node, visited: Set[Node]) -> List[Node]: ...
 
     @overload
     def subtree_of_type_rec(
         self, root: Node, visited: Set[Node], type: Union[Type[NodeT], Tuple[Type[NodeT], ...]]
-    ) -> List[NodeT]:
-        ...
+    ) -> List[NodeT]: ...
 
     def subtree_of_type_rec(self, root, visited, type=Node):
         """recursive helper function for subtree_of_type"""
         # check if root is of type target
         res = []
         if isinstance(root, type):
             res.append(root)
@@ -1396,14 +1408,29 @@
         """Finds the parent of a node
 
         :param node: current node
         :return: node of parent function
         """
         if isinstance(node, FunctionNode):
             return node
+        if node.parent_function_id is None:
+            # no precalculated information found.
+            current_node = node
+            parent_node: Optional[Node] = node
+            while parent_node is not None:
+                current_node = parent_node
+                if type(self.node_at(current_node.id)) == FunctionNode:
+                    node.parent_function_id = current_node.id
+                    break
+                parents = [e[0] for e in self.in_edges(current_node.id, etype=EdgeType.CHILD)]
+                if len(parents) == 0:
+                    parent_node = None
+                else:
+                    parent_node = self.node_at(parents[0])
+
         assert node.parent_function_id
         return cast(FunctionNode, self.node_at(node.parent_function_id))
 
     def get_left_right_subtree(
         self, target: Node, right_subtree: bool, ignore_called_nodes: bool = False
     ) -> List[Node]:
         """Searches for all subnodes of main which are to the left or to the right of the specified node
```

### Comparing `discopop-3.1.1/discopop_explorer/__main__.py` & `discopop-3.2.0/discopop_explorer/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 from argparse import ArgumentParser
 from pathlib import Path
+from discopop_library.GlobalLogger.setup import setup_logger
 
 from discopop_library.PathManagement.PathManagement import get_path, get_path_or_none
 from .discopop_explorer import ExplorerArguments, run
 
 
 def parse_args() -> ExplorerArguments:
     """Parse the arguments passed to the discopop_explorer"""
@@ -67,14 +68,17 @@
         "--dump-detection-result", type=str, nargs="?", default="explorer/detection_result_dump.json",
         help="Dump DetectionResult object to JSON file. If a path is given, the DetectionResult object is written to the given file, otherwise to detection_result_dump.json. Contents are equivalent to the json output. NOTE: This dump contains a dump of the PET Graph!",
     )
     parser.add_argument(
         "--enable-patterns", type=str, nargs="?", default="*",
         help="Specify comma-separated list of pattern types to be identified. Options: reduction,doall,pipeline,geodec,simplegpu. Default: *",
     )
+    parser.add_argument("--load-existing-doall-and-reduction-patterns", action="store_true", help="Skip pattern detection and insert existing patterns.json contents into the created detection_result.json")
+    parser.add_argument("--log", type=str, default="WARNING", help="Specify log level: DEBUG, INFO, WARNING, ERROR, CRITICAL")
+    parser.add_argument("--write-log", action="store_true", help="Create Logfile.")
 
     # EXPERIMENTAL FLAGS:
     # temporary flag for microbenchmark file
     experimental_parser.add_argument(
         "--microbench-file", type=str, default=None,
         help="path to a microbenchmark json file",
     )
@@ -145,17 +149,21 @@
         enable_pet_dump_file=arguments.dump_pet,
         enable_detection_result_dump_file=arguments.dump_detection_result,
         enable_patterns=arguments.enable_patterns,
         generate_data_cu_inst=arguments.generate_data_cu_inst,
         cu_inst_result_file=arguments.cu_inst_res,
         llvm_cxxfilt_path=arguments.llvm_cxxfilt_path,
         enable_json_file=arguments.json,
+        log_level=arguments.log.upper(),
+        write_log=arguments.write_log,
+        load_existing_doall_and_reduction_patterns=arguments.load_existing_doall_and_reduction_patterns,
     )
 
 
 def main():
     arguments = parse_args()
+    setup_logger(arguments)
     run(arguments)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `discopop-3.1.1/discopop_explorer/discopop_explorer.py` & `discopop-3.2.0/discopop_explorer/discopop_explorer.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,38 +4,45 @@
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 import cProfile
 import json
+import logging
 import os
 import sys
 import time
 from dataclasses import dataclass
 from pathlib import Path
-from typing import List, Optional
+from typing import Dict, List, Optional, Tuple
 
 import pstats2  # type:ignore
-from pluginbase import PluginBase  # type:ignore
+from pluginbase import PluginBase  # type: ignore
+from discopop_library.ArgumentClasses.GeneralArguments import GeneralArguments  # type: ignore
+from discopop_library.HostpotLoader.HotspotLoaderArguments import HotspotLoaderArguments
+from discopop_library.HostpotLoader.HotspotNodeType import HotspotNodeType
+from discopop_library.HostpotLoader.HotspotType import HotspotType  # type:ignore
 
 from discopop_library.LineMapping.initialize import initialize_line_mapping
 from discopop_library.PathManagement.PathManagement import get_path, load_file_mapping
 from discopop_library.discopop_optimizer.Microbench.ExtrapInterpolatedMicrobench import (
     ExtrapInterpolatedMicrobench,
 )
 from discopop_library.result_classes.DetectionResult import DetectionResult
 from .PEGraphX import PEGraphX
 from .json_serializer import PatternBaseSerializer
 from .parser import parse_inputs
 from .pattern_detection import PatternDetectorX
 
+from discopop_library.HostpotLoader.hostpot_loader import run as load_hotspots
+
 
 @dataclass
-class ExplorerArguments(object):
+class ExplorerArguments(GeneralArguments):
     """Container Class for the arguments passed to the discopop_explorer"""
 
     # input files and configuration
     discopop_build_path: str
     project_path: str
     cu_xml_file: str
     dep_file: str
@@ -52,14 +59,15 @@
     # experimental features:
     enable_task_pattern: bool
     detect_scheduling_clauses: bool
     generate_data_cu_inst: Optional[str]  # none: generate Data_CUInst.txt & exit
     cu_inst_result_file: Optional[str]
     llvm_cxxfilt_path: Optional[str]
     microbench_file: Optional[str]
+    load_existing_doall_and_reduction_patterns: bool
 
     def __post_init__(self):
         self.__validate()
 
     def __validate(self):
         """Validate the arguments passed to the discopop_explorer, e.g check if given files exist"""
         validation_failure = False
@@ -99,14 +107,16 @@
     file_mapping: Optional[str] = None,
     cu_inst_result_file: Optional[str] = None,
     llvm_cxxfilt_path: Optional[str] = None,
     discopop_build_path: Optional[str] = None,
     enable_patterns: str = "*",
     enable_task_pattern: bool = False,
     enable_detection_of_scheduling_clauses: bool = False,
+    hotspot_functions: Optional[Dict[HotspotType, List[Tuple[int, int, HotspotNodeType, str]]]] = None,
+    load_existing_doall_and_reduction_patterns: bool = False,
 ) -> DetectionResult:
     pet = PEGraphX.from_parsed_input(*parse_inputs(cu_xml, dep_file, reduction_file, file_mapping))
     print("PET CREATION FINISHED.")
     # pet.show()
     # TODO add visualization
 
     plugin_base = PluginBase(package="plugins")
@@ -116,39 +126,59 @@
     for plugin_name in plugins:
         p = plugin_source.load_plugin(plugin_name)
         print("executing plugin before: " + plugin_name)
         pet = p.run_before(pet)
 
     pattern_detector = PatternDetectorX(pet)
 
-    res: DetectionResult = pattern_detector.detect_patterns(
-        project_path,
-        cu_xml,
-        dep_file,
-        loop_counter_file,
-        reduction_file,
-        file_mapping,
-        cu_inst_result_file,
-        llvm_cxxfilt_path,
-        discopop_build_path,
-        enable_patterns,
-        enable_task_pattern,
-        enable_detection_of_scheduling_clauses,
-    )
+    if load_existing_doall_and_reduction_patterns:
+        res: DetectionResult = pattern_detector.load_existing_doall_and_reduction_patterns(
+            project_path,
+            cu_xml,
+            dep_file,
+            loop_counter_file,
+            reduction_file,
+            file_mapping,
+            cu_inst_result_file,
+            llvm_cxxfilt_path,
+            discopop_build_path,
+            enable_patterns,
+            enable_task_pattern,
+            enable_detection_of_scheduling_clauses,
+            hotspot_functions,
+        )
+    else:
+        res = pattern_detector.detect_patterns(
+            project_path,
+            cu_xml,
+            dep_file,
+            loop_counter_file,
+            reduction_file,
+            file_mapping,
+            cu_inst_result_file,
+            llvm_cxxfilt_path,
+            discopop_build_path,
+            enable_patterns,
+            enable_task_pattern,
+            enable_detection_of_scheduling_clauses,
+            hotspot_functions,
+        )
 
     for plugin_name in plugins:
         p = plugin_source.load_plugin(plugin_name)
         # print("executing plugin after: " + plugin_name)
         pet = p.run_after(pet)
 
     return res
 
 
 def run(arguments: ExplorerArguments):
     """Run the discopop_explorer with the given arguments"""
+    logger = logging.getLogger("Explorer")
+
     # create explorer directory if not already present
     if not os.path.exists(os.path.join(arguments.project_path, "explorer")):
         os.mkdir(os.path.join(arguments.project_path, "explorer"))
     # create file to store next free pattern ids if not already present
     if not os.path.exists("next_free_pattern_id.txt"):
         with open("next_free_pattern_id.txt", "w") as f:
             f.write(str(0))
@@ -169,14 +199,31 @@
             arguments.dep_file,
             arguments.loop_counter_file,
             arguments.reduction_file,
             arguments.generate_data_cu_inst,
         )
         sys.exit(0)
 
+    print("Loading Hotspots...")
+
+    hotspots = load_hotspots(
+        HotspotLoaderArguments(
+            verbose=True,
+            get_loops=True,
+            get_functions=True,
+            get_YES=True,
+            get_MAYBE=True,
+            get_NO=False,
+            log_level=arguments.log_level,
+            write_log=arguments.write_log,
+        )
+    )
+
+    print("Done.")
+
     start = time.time()
 
     res = __run(
         arguments.project_path,
         arguments.cu_xml_file,
         arguments.dep_file,
         arguments.loop_counter_file,
@@ -185,14 +232,16 @@
         file_mapping=arguments.file_mapping_file,
         cu_inst_result_file=arguments.cu_inst_result_file,
         llvm_cxxfilt_path=arguments.llvm_cxxfilt_path,
         discopop_build_path=arguments.discopop_build_path,
         enable_patterns=arguments.enable_patterns,
         enable_task_pattern=arguments.enable_task_pattern,
         enable_detection_of_scheduling_clauses=arguments.detect_scheduling_clauses,
+        hotspot_functions=hotspots,
+        load_existing_doall_and_reduction_patterns=arguments.load_existing_doall_and_reduction_patterns,
     )
 
     end = time.time()
 
     if arguments.enable_pet_dump_file is not None:
         with open(arguments.enable_pet_dump_file, "w+") as f:
             f.write(res.pet.dump_to_pickled_json())
```

### Comparing `discopop-3.1.1/discopop_explorer/generate_Data_CUInst.py` & `discopop-3.2.0/discopop_explorer/generate_Data_CUInst.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/json_serializer.py` & `discopop-3.2.0/discopop_explorer/json_serializer.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/parallel_utils.py` & `discopop-3.2.0/discopop_explorer/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/parser.py` & `discopop-3.2.0/discopop_explorer/parser.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/PatternBase.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/PatternBase.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
     """Base class for pattern info"""
 
     pattern_id: int
     _node: Node
     node_id: NodeID
     start_line: LineID
     end_line: LineID
+    applicable_pattern: bool
 
     def __init__(self, node: Node):
         # create a file lock to synchronize processes
         with FileLock(os.path.join(os.getcwd(), "next_free_pattern_id.txt.lock")):
             with open(os.path.join(os.getcwd(), "next_free_pattern_id.txt"), "r+") as f:
                 lines = f.readlines()
                 f.truncate(0)
@@ -37,14 +38,15 @@
                         line = line.replace("\n", "").replace("\x00", "")
                         self.pattern_id = int(line)
                         f.write(str(self.pattern_id + 1))
         self._node = node
         self.node_id = node.id
         self.start_line = node.start_position()
         self.end_line = node.end_position()
+        self.applicable_pattern = True
 
     def to_json(self):
         dic = self.__dict__
         keys = [k for k in dic.keys()]
         for key in keys:
             if key.startswith("_"):
                 del dic[key]
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/PatternInfo.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/PatternInfo.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/CombinedGPURegions.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/CombinedGPURegions.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,44 +119,44 @@
         read_memory_regions_by_cu: Dict[NodeID, Set[MemoryRegion]]
         (
             written_memory_regions_by_cu,
             read_memory_regions_by_cu,
         ) = get_written_and_read_memory_regions_by_cu(self.contained_regions, pet)
 
         # get memory region and variable associations for each CU
-        cu_and_variable_to_memory_regions: Dict[
-            NodeID, Dict[VarName, Set[MemoryRegion]]
-        ] = get_cu_and_varname_to_memory_regions(self.contained_regions, pet, written_memory_regions_by_cu)
+        cu_and_variable_to_memory_regions: Dict[NodeID, Dict[VarName, Set[MemoryRegion]]] = (
+            get_cu_and_varname_to_memory_regions(self.contained_regions, pet, written_memory_regions_by_cu)
+        )
 
         print("WRITTEN MEMORY REGIONS BY CU: ", file=sys.stderr)
         print(written_memory_regions_by_cu, file=sys.stderr)
         print(file=sys.stderr)
 
         print("READ MEMORY REGIONS BY CU: ", file=sys.stderr)
         print(read_memory_regions_by_cu, file=sys.stderr)
         print(file=sys.stderr)
 
         # get memory regions to cus and variables names
-        memory_regions_to_cus_and_variables: Dict[
-            MemoryRegion, Dict[NodeID, Set[VarName]]
-        ] = get_memory_region_to_cu_and_variables_dict(cu_and_variable_to_memory_regions)
+        memory_regions_to_cus_and_variables: Dict[MemoryRegion, Dict[NodeID, Set[VarName]]] = (
+            get_memory_region_to_cu_and_variables_dict(cu_and_variable_to_memory_regions)
+        )
         print("MEMORY REGIONS TO CUS AND VARIABLES:", file=sys.stderr)
         print(memory_regions_to_cus_and_variables, file=sys.stderr)
         print(file=sys.stderr)
 
         # ### STEP 2.1: INITIALIZE LIVE DATA USING MAPPING CLAUSES AND CONVERSION TO MEMORY REGIONS
         live_device_variables = populate_live_data(self, pet, ignore_update_instructions=True)
         print("LIVE DEVICE VARIABLES:", file=sys.stderr)
         print(live_device_variables, file=sys.stderr)
         print(file=sys.stderr)
 
         # extend device liveness with memory regions
-        device_liveness_plus_memory_regions: Dict[
-            VarName, List[Tuple[NodeID, Set[MemoryRegion]]]
-        ] = add_memory_regions_to_device_liveness(live_device_variables, cu_and_variable_to_memory_regions)
+        device_liveness_plus_memory_regions: Dict[VarName, List[Tuple[NodeID, Set[MemoryRegion]]]] = (
+            add_memory_regions_to_device_liveness(live_device_variables, cu_and_variable_to_memory_regions)
+        )
 
         # ### STEP 2.2: CALCULATE LIVE DATA BY PROPAGATING MEMORY REGIONS AND EXTENDING LIFESPAN
 
         # propagate memory regions
         device_liveness_plus_memory_regions = propagate_memory_regions(device_liveness_plus_memory_regions)
 
         print("PROPAGATED DEVICE VARIABLES + MEMORY:", file=sys.stderr)
@@ -248,17 +248,17 @@
 
         # remove dummy marks from CU ID's created during loop unrolling
         for update in issued_updates:
             update.remove_dummy_marks()
 
         # ### STEP 5: CONVERT MEMORY REGIONS IN UPDATES TO VARIABLE NAMES
         # propagate memory region to variable name associations within function body
-        memory_regions_to_functions_and_variables: Dict[
-            MemoryRegion, Dict[NodeID, Set[VarName]]
-        ] = propagate_variable_name_associations(pet, memory_regions_to_cus_and_variables)
+        memory_regions_to_functions_and_variables: Dict[MemoryRegion, Dict[NodeID, Set[VarName]]] = (
+            propagate_variable_name_associations(pet, memory_regions_to_cus_and_variables)
+        )
         print("MEMORY REGIONS TO FUNCTIONS AND VARIABLES:", file=sys.stderr)
         print(memory_regions_to_functions_and_variables, file=sys.stderr)
         print(file=sys.stderr)
 
         # determine variable name for memory regions in update instructions
         for update in issued_updates:
             update.convert_memory_regions_to_variable_names(pet, memory_regions_to_functions_and_variables)
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Dependency.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Dependency.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/EntryPoint.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/EntryPoint.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Enums.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Enums.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/ExitPoint.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/ExitPoint.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Update.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/classes/Update.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/combined_gpu_pattern_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/combined_gpu_pattern_detector.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/prepare_metadata.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/prepare_metadata.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 from typing import Set, List, Tuple
 
 from discopop_explorer.PEGraphX import PEGraphX, NodeID
 from discopop_explorer.pattern_detectors.combined_gpu_patterns.classes.Aliases import VarName
 from discopop_explorer.pattern_detectors.combined_gpu_patterns.classes.Dependency import Dependency
 
 
-def get_dependencies_as_metadata(
-    pet: PEGraphX, all_dependencies: Set[Dependency]
-) -> Tuple[List[Tuple[VarName, NodeID, str]], List[Tuple[VarName, NodeID, str]],]:
+def get_dependencies_as_metadata(pet: PEGraphX, all_dependencies: Set[Dependency]) -> Tuple[
+    List[Tuple[VarName, NodeID, str]],
+    List[Tuple[VarName, NodeID, str]],
+]:
     in_deps_metadata: Set[Tuple[VarName, NodeID, str]] = set()
     out_deps_metadata: Set[Tuple[VarName, NodeID, str]] = set()
 
     for dependency in all_dependencies:
         # create out dependency metadata
         for var_name in dependency.var_names:
             out_deps_metadata.add(
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_1.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_1.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_2.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_2.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_3.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_3.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_4.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_4.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_5.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_5.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_6.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/step_6.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/combined_gpu_patterns/utilities.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/combined_gpu_patterns/utilities.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/device_updates.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/device_updates.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/do_all_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/do_all_detector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
+import sys
 from multiprocessing import Pool
 from typing import List, Dict, Set, Tuple, cast
+import warnings
 
 from alive_progress import alive_bar  # type: ignore
 
 from .PatternInfo import PatternInfo
+from .reduction_detector import ReductionInfo
 from ..PEGraphX import (
     CUNode,
     LoopNode,
     PEGraphX,
     Node,
     NodeType,
     EdgeType,
     LineID,
     MemoryRegion,
     DepType,
+    NodeID,
 )
-from ..utils import classify_loop_variables
+from ..utils import classify_loop_variables, filter_for_hotspots
 from ..variable import Variable
 
 
 class DoAllInfo(PatternInfo):
     """Class, that contains do-all detection result"""
 
     def __init__(self, pet: PEGraphX, node: Node):
@@ -62,33 +66,42 @@
             f"scheduling clause: {self.scheduling_clause}"
         )
 
 
 global_pet = None
 
 
-def run_detection(pet: PEGraphX) -> List[DoAllInfo]:
+def run_detection(pet: PEGraphX, hotspots, reduction_info: List[ReductionInfo]) -> List[DoAllInfo]:
     """Search for do-all loop pattern
 
     :param pet: PET graph
     :return: List of detected pattern info
     """
     import tqdm  # type: ignore
 
     global global_pet
     global_pet = pet
     result: List[DoAllInfo] = []
     nodes = pet.all_nodes(LoopNode)
 
+    # remove reduction loops
+    print("ASDF: ", [r.node_id for r in reduction_info])
+    print("Nodes: ", [n.start_position() for n in nodes])
+    print("pre:", len(nodes))
+    nodes = [n for n in nodes if n.id not in [r.node_id for r in reduction_info]]
+    print("post:", len(nodes))
+
+    nodes = cast(List[LoopNode], filter_for_hotspots(pet, cast(List[Node], nodes), hotspots))
+
     param_list = [(node) for node in nodes]
     with Pool(initializer=__initialize_worker, initargs=(pet,)) as pool:
         tmp_result = list(tqdm.tqdm(pool.imap_unordered(__check_node, param_list), total=len(param_list)))
     for local_result in tmp_result:
         result += local_result
-    print("GLOBAL RES: ", result)
+    print("GLOBAL RES: ", [r.start_line for r in result])
 
     for pattern in result:
         pattern.get_workload(pet)
         pattern.get_per_iteration_workload(pet)
 
     # remove reduction operations from shared variables to prevent issues / incorrect results in the exported JSON file
     for idx, _ in enumerate(result):
@@ -133,22 +146,29 @@
     for v in root_children_loops:
         loop_start_lines.append(v.start_position())
     fp, p, lp, s, r = classify_loop_variables(pet, root_loop)
     # get variables which are defined inside the loop
     defined_inside_loop: List[Tuple[Variable, Set[MemoryRegion]]] = []
     tmp_loop_variables = pet.get_variables(root_children_cus)
     for var in tmp_loop_variables:
-        if var.defLine >= root_loop.start_position() and var.defLine <= root_loop.end_position():
-            defined_inside_loop.append((var, tmp_loop_variables[var]))
+        if ":" in var.defLine:
+            file_id = int(var.defLine.split(":")[0])
+            def_line_num = int(var.defLine.split(":")[1])
+            for rc_cu in root_children_cus:
+                if file_id == rc_cu.file_id and def_line_num >= rc_cu.start_line and def_line_num <= rc_cu.end_line:
+                    defined_inside_loop.append((var, tmp_loop_variables[var]))
 
     # check if all subnodes are parallelizable
+    file_io_warnings = []
     for node in pet.subtree_of_type(root_loop, CUNode):
         if node.performs_file_io:
             # node is not reliably parallelizable as some kind of file-io is performed.
-            return False
+            file_io_warnings.append(node)
+            # return False  # too pessimistic
+            # todo: issue critical around file_io
 
     for i in range(0, len(subnodes)):
         children_cache: Dict[Node, List[Node]] = dict()
         dependency_cache: Dict[Tuple[Node, Node], Set[Node]] = dict()
         for j in range(i, len(subnodes)):
             if __check_loop_dependencies(
                 pet,
@@ -162,14 +182,17 @@
                 p,
                 lp,
                 defined_inside_loop,
             ):
                 # if pet.depends_ignore_readonly(subnodes[i], subnodes[j], root_loop):
                 return False
 
+    for fio in file_io_warnings:
+        warnings.warn("FileIO performed inside DoAll @ " + str(node.start_position()))
+
     return True
 
 
 def __check_loop_dependencies(
     pet: PEGraphX,
     node_1: Node,
     node_2: Node,
@@ -200,14 +223,21 @@
 
     # get memory regions which are defined inside the loop
     memory_regions_defined_in_loop = set()
     for var, mem_regs in defined_inside_loop:
         memory_regions_defined_in_loop.update(mem_regs)
 
     for source, target, dep in deps:
+
+        # todo: move this calculation to the innermost point possible to reduce computation costs
+        # get metadata for dependency
+        dep_source_nesting_level = __calculate_nesting_level(pet, root_loop, source)
+        dep_target_nesting_level = __calculate_nesting_level(pet, root_loop, target)
+        max_considered_intra_iteration_dep_level = max(dep_source_nesting_level, dep_target_nesting_level)
+
         # check if targeted variable is readonly inside loop
         if pet.is_readonly_inside_loop_body(
             dep,
             root_loop,
             root_children_cus,
             root_children_loops,
             loops_start_lines=loop_start_lines,
@@ -215,37 +245,60 @@
             # variable is readonly -> no problem
             continue
 
         # check if targeted variable is loop index
         if pet.is_loop_index(dep.var_name, loop_start_lines, root_children_cus):
             continue
 
-        # check if variable is defined inside loop
-        if dep.memory_region in memory_regions_defined_in_loop:
-            continue
-
         # targeted variable is not read-only
         if dep.dtype == DepType.INIT:
             continue
         elif dep.dtype == DepType.RAW:
             # check RAW dependencies
             # RAW problematic, if it is not an intra-iteration RAW
             if not dep.intra_iteration:
                 return True
             # if it is an intra iteration dependency, it is problematic if it belongs to a parent loop
-            elif dep.intra_iteration_level > root_loop.get_nesting_level(pet):
-                tmp = root_loop.get_nesting_level(pet)
-                return True
+            else:
+                if dep.intra_iteration_level <= max_considered_intra_iteration_dep_level:
+                    if pet.node_at(source) in root_children_cus and pet.node_at(target) in root_children_cus:
+                        pass
+                    else:
+                        return True
+
+        #                    # dep within the loop. not problematic, if intra_iteration_level == 0
+        #                    if dep.intra_iteration_level == 0:
+        #                        pass
+        #                    else:
+        #                        # might be problematic
+        #                        # check if source and target in children loops
+        #                        contained_in_nested_loop = False
+        #                        for nested_loop in [l for l in root_children_loops if l != root_loop]:
+        #                            nested_children = pet.subtree_of_type(nested_loop, (CUNode, LoopNode))
+        #                            nested_children_cus = [cast(CUNode, cu) for cu in nested_children if cu.type == NodeType.CU]
+        #                            if pet.node_at(source) in nested_children_cus and pet.node_at(target) in nested_children_cus:
+        #                                contained_in_nested_loop = True
+        #                        if not contained_in_nested_loop:
+        #                            # problematic
+        #                            return True
+
+        #                else:
+        #                    # dep could belong to a parent loop
+        #                    if root_loop.get_nesting_level(pet) > 1 and dep.intra_iteration_level > 0:
+        #                        # dep belongs to parent loop. Can not be ignored for the inner loop
+        #                        return True
 
         elif dep.dtype == DepType.WAR:
             # check WAR dependencies
             # WAR problematic, if it is not an intra-iteration WAR and the variable is not private or firstprivate
             if not dep.intra_iteration:
                 if dep.var_name not in [v.name for v in first_privates + privates + last_privates]:
-                    return True
+                    # check if variable is defined inside loop
+                    if dep.memory_region not in memory_regions_defined_in_loop:
+                        return True
             # if it is an intra iteration dependency, it is problematic if it belongs to a parent loop
             elif dep.intra_iteration_level > root_loop.get_nesting_level(pet):
                 tmp = root_loop.get_nesting_level(pet)
                 return True
         elif dep.dtype == DepType.WAW:
             # check WAW dependencies
             # handled by variable classification
@@ -276,7 +329,22 @@
         children_cache: Dict[CUNode, List[CUNode]] = dict()
         dependency_cache: Dict[Tuple[CUNode, CUNode], Set[CUNode]] = dict()
         for j in range(i, len(subnodes)):
             if pet.depends_ignore_readonly(subnodes[i], subnodes[j], root_loop):
                 return False
 
     return True
+
+
+def __calculate_nesting_level(pet: PEGraphX, root_loop: LoopNode, cu_node_id: str):
+    potential_parents = [(cu_node_id, -1)]  # -1 to offset the initialization with cu_node_id
+    while True:
+        if len(potential_parents) == 0:
+            # warnings.warn("root_loop: " + str(root_loop) + " not a parent of cu_node_id: " + str(cu_node_id))
+            return sys.maxsize
+        current_node_id, nesting_level = potential_parents.pop()
+        if current_node_id == root_loop.id:
+            # found
+            return nesting_level
+        # add new parents to the queue
+        for in_child_edge in pet.in_edges(cast(NodeID, current_node_id), EdgeType.CHILD):
+            potential_parents.append((in_child_edge[0], nesting_level + 1))
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/geometric_decomposition_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/geometric_decomposition_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 
 import math
-from typing import Dict, List, Tuple, Optional
+from typing import Dict, List, Tuple, Optional, cast
 
 from alive_progress import alive_bar  # type: ignore
 
 from .PatternInfo import PatternInfo
 from ..PEGraphX import FunctionNode, LoopNode, NodeID, PEGraphX, Node, EdgeType
-from ..utils import classify_task_vars, get_child_loops
+from ..utils import classify_task_vars, filter_for_hotspots, get_child_loops
 from ..variable import Variable
 
 __loop_iterations: Dict[NodeID, int] = {}
 
 
 class GDInfo(PatternInfo):
     """Class, that contains geometric decomposition detection result"""
@@ -74,15 +74,15 @@
             f"\tlast private: {[v.name for v in self.last_private]}"
         )
 
 
 global_pet = None
 
 
-def run_detection(pet: PEGraphX) -> List[GDInfo]:
+def run_detection(pet: PEGraphX, hotspots) -> List[GDInfo]:
     """Detects geometric decomposition
 
     :param pet: PET graph
     :return: List of detected pattern info
     """
     import tqdm  # type: ignore
     from multiprocessing import Pool
@@ -91,14 +91,16 @@
     global_pet = pet
 
     result: List[GDInfo] = []
     global __loop_iterations
     __loop_iterations = {}
     nodes = pet.all_nodes(FunctionNode)
 
+    nodes = cast(List[FunctionNode], filter_for_hotspots(pet, cast(List[Node], nodes), hotspots))
+
     param_list = [(node) for node in nodes]
     with Pool(initializer=__initialize_worker, initargs=(pet,)) as pool:
         tmp_result = list(tqdm.tqdm(pool.imap_unordered(__check_node, param_list), total=len(param_list)))
     for local_result in tmp_result:
         result += local_result
     print("GLOBAL RES: ", result)
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/pipeline_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/pipeline_detector.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 
-from typing import List, Tuple, Dict, Set
+from typing import List, Tuple, Dict, Set, cast
 
 from alive_progress import alive_bar  # type: ignore
 
 from .PatternInfo import PatternInfo
 from ..PEGraphX import (
     CUNode,
     LineID,
@@ -19,15 +19,15 @@
     NodeID,
     PEGraphX,
     Node,
     EdgeType,
     DepType,
     Dependency,
 )
-from ..utils import correlation_coefficient, classify_task_vars
+from ..utils import correlation_coefficient, classify_task_vars, filter_for_hotspots
 
 __pipeline_threshold = 0.9
 
 
 class PipelineStage(object):
     def __init__(self, pet: PEGraphX, node: Node, in_dep, out_dep):
         self.node = node.id
@@ -144,15 +144,15 @@
         and c_start in children_start_lines
     )
 
 
 global_pet = None
 
 
-def run_detection(pet: PEGraphX) -> List[PipelineInfo]:
+def run_detection(pet: PEGraphX, hotspots) -> List[PipelineInfo]:
     """Search for pipeline pattern on all the loops in the graph
     except for doall loops
 
     :param pet: PET graph
     :return: List of detected pattern info
     """
     import tqdm  # type: ignore
@@ -162,14 +162,16 @@
     global_pet = pet
 
     result: List[PipelineInfo] = []
     children_cache: Dict[Node, List[Node]] = dict()
     dependency_cache: Dict[Tuple[Node, Node], Set[Node]] = dict()
     nodes = pet.all_nodes(LoopNode)
 
+    nodes = cast(List[LoopNode], filter_for_hotspots(pet, cast(List[Node], nodes), hotspots))
+
     param_list = [(node) for node in nodes]
     with Pool(initializer=__initialize_worker, initargs=(pet,)) as pool:
         tmp_result = list(tqdm.tqdm(pool.imap_unordered(__check_node, param_list), total=len(param_list)))
     for local_result in tmp_result:
         result += local_result
     print("GLOBAL RES: ", result)
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/reduction_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/reduction_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     PEGraphX,
     NodeType,
     Node,
     LineID,
     DepType,
     EdgeType,
 )
-from ..utils import is_reduction_var, classify_loop_variables
+from ..utils import filter_for_hotspots, is_reduction_var, classify_loop_variables
 from ..variable import Variable
 
 
 class ReductionInfo(PatternInfo):
     """Class, that contains reduction detection result"""
 
     def __init__(self, pet: PEGraphX, node: Node):
@@ -58,33 +58,35 @@
             f"last private: {[v.name for v in self.last_private]}"
         )
 
 
 global_pet = None
 
 
-def run_detection(pet: PEGraphX) -> List[ReductionInfo]:
+def run_detection(pet: PEGraphX, hotspots) -> List[ReductionInfo]:
     """Search for reduction pattern
 
     :param pet: PET graph
     :return: List of detected pattern info
     """
     import tqdm  # type: ignore
 
     global global_pet
     global_pet = pet
     result: List[ReductionInfo] = []
     nodes = pet.all_nodes(LoopNode)
 
+    nodes = cast(List[LoopNode], filter_for_hotspots(pet, cast(List[Node], nodes), hotspots))
+
     param_list = [(node) for node in nodes]
     with Pool(initializer=__initialize_worker, initargs=(pet,)) as pool:
         tmp_result = list(tqdm.tqdm(pool.imap_unordered(__check_node, param_list), total=len(param_list)))
     for local_result in tmp_result:
         result += local_result
-    print("GLOBAL RES: ", result)
+    print("GLOBAL RES: ", [r.start_line for r in result])
 
     for pattern in result:
         pattern.get_workload(pet)
         pattern.get_per_iteration_workload(pet)
 
     return result
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPULoop.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPULoop.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPUMemory.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPUMemory.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPURegions.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/GPURegions.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/gpu_pattern_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/gpu_pattern_detector.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/simple_gpu_patterns/utils.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/simple_gpu_patterns/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/alias_detection.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/alias_detection.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/classes.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/classes.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/filter.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/filter.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/postprocessor.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/postprocessor.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/preprocessor.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/preprocessor.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/auxiliary.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/auxiliary.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/barriers.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/barriers.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/data_sharing_clauses.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/data_sharing_clauses.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/dependency_clauses.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/dependency_clauses.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/suggesters/tasks.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/suggesters/tasks.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/task_parallelism_detector.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/task_parallelism_detector.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from typing import List, Optional, cast
 
 from discopop_explorer.PEGraphX import DummyNode, PEGraphX, MWType
 from discopop_explorer.parser import parse_inputs
 from discopop_explorer.pattern_detectors.PatternInfo import PatternInfo
 from discopop_explorer.pattern_detectors.do_all_detector import run_detection as detect_do_all
-from discopop_explorer.pattern_detectors.reduction_detector import run_detection as detect_reduction
+from discopop_explorer.pattern_detectors.reduction_detector import ReductionInfo, run_detection as detect_reduction
 from discopop_explorer.pattern_detectors.task_parallelism.classes import (
     TaskParallelismInfo,
     TPIType,
 )
 from discopop_explorer.pattern_detectors.task_parallelism.filter import (
     filter_data_sharing_clauses,
     remove_useless_barrier_suggestions,
@@ -70,14 +70,16 @@
     cu_xml: str,
     dep_file: str,
     reduction_file: str,
     file_mapping: str,
     cu_inst_result_file: str,
     llvm_cxxfilt_path: Optional[str],
     discopop_build_path: Optional[str],
+    hotspots,
+    reduction_info: List[ReductionInfo],
 ) -> List[PatternInfo]:
     """execute preprocessing of given cu xml file and construct a new cu graph.
     execute run_detection on newly constructed graph afterwards.
     :param cu_xml: Path (string) to the CU xml file to be used
     :param dep_file: Path (string) to the dependence file to be used
     :param loop_counter_file: Path (string) to the loop counter file file to be used
     :param reduction_file: Path (string) to the reduction file to be used
@@ -97,16 +99,16 @@
     set_global_llvm_cxxfilt_path(__global_llvm_cxxfilt_path)
     preprocessed_cu_xml = cu_xml_preprocessing(cu_xml)
     preprocessed_graph = PEGraphX.from_parsed_input(
         *parse_inputs(preprocessed_cu_xml, dep_file, reduction_file, file_mapping)
     )
 
     # execute reduction detector to enable taskloop-reduction-detection
-    detect_reduction(preprocessed_graph)
-    detect_do_all(preprocessed_graph)
+    detect_reduction(preprocessed_graph, hotspots)
+    detect_do_all(preprocessed_graph, hotspots, reduction_info)
 
     suggestions = run_detection(
         preprocessed_graph,
         preprocessed_cu_xml,
         file_mapping,
         dep_file,
         cu_inst_result_file,
```

### Comparing `discopop-3.1.1/discopop_explorer/pattern_detectors/task_parallelism/tp_utils.py` & `discopop-3.2.0/discopop_explorer/pattern_detectors/task_parallelism/tp_utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/plugins/pipeline.py` & `discopop-3.2.0/discopop_explorer/plugins/pipeline.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_explorer/utils.py` & `discopop-3.2.0/discopop_explorer/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,21 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import itertools
-from typing import List, Sequence, Set, Dict, Tuple, cast
+from typing import List, Optional, Sequence, Set, Dict, Tuple, cast
 
 import numpy as np
 import warnings
+from discopop_library.HostpotLoader.HotspotNodeType import HotspotNodeType
+
+from discopop_library.HostpotLoader.HotspotType import HotspotType
 
 from .PEGraphX import (
     CUNode,
     FunctionNode,
     LineID,
     LoopNode,
     NodeID,
@@ -724,15 +727,23 @@
 def classify_task_vars(
     pet: PEGraphX,
     task: Node,
     type: str,
     in_deps: List[Tuple[NodeID, NodeID, Dependency]],
     out_deps: List[Tuple[NodeID, NodeID, Dependency]],
     used_in_task_parallelism_detection=False,
-) -> Tuple[List[Variable], List[Variable], List[Variable], List[Variable], List[Variable], List[Variable], List[str],]:
+) -> Tuple[
+    List[Variable],
+    List[Variable],
+    List[Variable],
+    List[Variable],
+    List[Variable],
+    List[Variable],
+    List[str],
+]:
     """Classify task variables
 
     :param pet: CU graph
     :param task: node
     :param type: type of task
     :param in_deps: in dependencies
     :param out_deps: out dependencies
@@ -915,7 +926,51 @@
     for out_dep in pet.out_edges(task.id, EdgeType.DATA):
         if out_dep[2].dtype != DepType.RAW:
             continue
         # check if out_dep.source in predecessors
         if pet.node_at(out_dep[0]) in predecessors:
             return True
     return False
+
+
+def filter_for_hotspots(
+    pet: PEGraphX,
+    nodes: List[Node],
+    hotspot_information: Optional[Dict[HotspotType, List[Tuple[int, int, HotspotNodeType, str]]]],
+) -> List[Node]:
+    """Removes such nodes from the list which are not identified as hotspots"""
+    if hotspot_information is None:
+        return nodes
+    if len(hotspot_information) == 0:
+        return nodes
+    # collect hotspot information
+    all_hotspot_descriptions: List[Tuple[int, int, HotspotNodeType, str]] = []
+    for key in hotspot_information:
+        for entry in hotspot_information[key]:
+            all_hotspot_descriptions.append(entry)
+
+    result_set: Set[Node] = set()
+    # check for direct matches
+    for node in nodes:
+        for hotspot in all_hotspot_descriptions:
+            # check if file matches
+            if hotspot[0] == node.file_id:
+                # check if location matches
+                if hotspot[1] == node.start_line:
+                    # check if type matches
+                    if node.type == NodeType.LOOP and hotspot[2] == HotspotNodeType.LOOP:
+                        result_set.add(node)
+                    if node.type == NodeType.FUNC and hotspot[2] == HotspotNodeType.FUNCTION:
+                        result_set.add(node)
+
+    #    # check for matches from hotspot functions
+    #    for node in nodes:
+    #        for hotspot in all_hotspot_descriptions:
+    #            if hotspot[2] == HotspotNodeType.FUNCTION:
+    #                if hotspot[0] == node.file_id:
+    #                    try:
+    #                        if pet.get_parent_function(node).name == hotspot[3]:
+    #                            print("HOTSPOT FUNCTION MATCH FROM NODE: ", node.id)
+    #                    except AssertionError:
+    #                        continue
+
+    return list(result_set)
```

### Comparing `discopop-3.1.1/discopop_explorer/variable.py` & `discopop-3.2.0/discopop_explorer/variable.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,15 +27,18 @@
     def __hash__(self):
         return hash(self.name)
 
     def __eq__(self, other):
         return isinstance(other, Variable) and self.name == other.name
 
     def __lt__(self, other):
-        return self.name < other.name
+        try:
+            return self.name < other.name
+        except:
+            return True
 
     def __str__(self):
         return self.name
 
     def toJSON(self):
         if self.operation is None:
             return self.name
```

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/CodeGenerator.py` & `discopop-3.2.0/discopop_library/CodeGenerator/CodeGenerator.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/CodeGeneratorArguments.py` & `discopop-3.2.0/discopop_library/CodeGenerator/CodeGeneratorArguments.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/classes/ContentBuffer.py` & `discopop-3.2.0/discopop_library/CodeGenerator/classes/ContentBuffer.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/classes/Enums.py` & `discopop-3.2.0/discopop_library/CodeGenerator/classes/Enums.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/classes/Line.py` & `discopop-3.2.0/discopop_library/CodeGenerator/classes/Line.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/classes/Pragma.py` & `discopop-3.2.0/discopop_library/CodeGenerator/classes/Pragma.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/CodeGenerator/classes/UnpackedSuggestion.py` & `discopop-3.2.0/discopop_library/CodeGenerator/classes/UnpackedSuggestion.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
-from typing import Dict, List, Any, Optional
+from typing import Dict, List, Any, Optional, Tuple
 
 from discopop_explorer.pattern_detectors.combined_gpu_patterns.classes.Enums import (
     EntryPointType,
     EntryPointPositioning,
     UpdateType,
     ExitPointType,
     ExitPointPositioning,
@@ -60,43 +60,52 @@
 
         source_device_id = int(self.values["source_device_id"])
         target_device_id = int(self.values["target_device_id"])
         var_name = self.values["var_name"]
         is_first_data_occurrence: bool = self.values["is_first_data_occurrence"]
         openmp_source_device_id = self.values["openmp_source_device_id"]
         openmp_target_device_id = self.values["openmp_target_device_id"]
-        print("IS FIRST DATA OCCURRENCE?: ", is_first_data_occurrence)
+        range: Optional[Tuple[int, int]] = self.values["range"]
+        delete_data: bool = self.values["delete_data"]
+        copy_delete_data: bool = self.values["copy_delete_data"]
+
+        def get_range_str(r):
+            return "" if r is None else "[" + str(r[0]) + ":" + str(r[1]) + "]"
 
         if source_device_id == self.host_device_id and target_device_id == self.host_device_id:
             # no update required
             pass
         elif source_device_id == self.host_device_id and target_device_id != self.host_device_id:
             # update type to
             if is_first_data_occurrence:
                 pragma.pragma_str = "#pragma omp target enter data map(to:"
             else:
                 pragma.pragma_str = "#pragma omp target update to("
             pragma.pragma_str += (
                 var_name
+                + get_range_str(range)
                 + ") device("
                 # + str(openmp_source_device_id)
                 # + " -> "
                 + str(openmp_target_device_id)
                 + ")"
             )
 
         elif source_device_id != self.host_device_id and target_device_id == self.host_device_id:
             # update type from
-            if is_first_data_occurrence:
+            if delete_data:
+                pragma.pragma_str = "#pragma omp target exit data map(delete:"
+            elif copy_delete_data:
                 pragma.pragma_str = "#pragma omp target exit data map(from:"
             else:
                 pragma.pragma_str = "#pragma omp target update from("
 
             pragma.pragma_str += (
                 var_name
+                + get_range_str(range)
                 + ") device("
                 + str(openmp_source_device_id)
                 # + " -> "
                 # + str(openmp_target_device_id)
                 + ")"
             )
 
@@ -111,14 +120,15 @@
                 + str(source_device_id)
                 + ") --> Device("
                 + str(openmp_source_device_id)
                 + " -> "
                 + str(openmp_target_device_id)
                 + ") Var("
                 + var_name
+                + get_range_str(range)
                 + ")"
             )
 
         #            #  map to host
         #            pragma.pragma_str = (
         #                # "#pragma omp target map(from:"
         #                    "#pragma omp target enter data map(to:"
@@ -159,21 +169,21 @@
             pragma.pragma_str += "device(" + str(device_id) + ") "
         else:
             pragma.pragma_str = "#pragma omp parallel for "
         if "collapse_level" in self.values:
             if self.values["collapse_level"] > 1:
                 pragma.pragma_str += "collapse(" + str(self.values["collapse_level"]) + ") "
         if len(self.values["first_private"]) > 0:
-            pragma.pragma_str += "firstprivate(" + ",".join(self.values["first_private"]) + ") "
+            pragma.pragma_str += "firstprivate(" + ",".join([str(s) for s in self.values["first_private"]]) + ") "
         if len(self.values["private"]) > 0:
-            pragma.pragma_str += "private(" + ",".join(self.values["private"]) + ") "
+            pragma.pragma_str += "private(" + ",".join([str(s) for s in self.values["private"]]) + ") "
         if len(self.values["last_private"]) > 0:
-            pragma.pragma_str += "lastprivate(" + ",".join(self.values["last_private"]) + ") "
+            pragma.pragma_str += "lastprivate(" + ",".join([str(s) for s in self.values["last_private"]]) + ") "
         if len(self.values["shared"]) > 0:
-            pragma.pragma_str += "shared(" + ",".join(self.values["shared"]) + ") "
+            pragma.pragma_str += "shared(" + ",".join([str(s) for s in self.values["shared"]]) + ") "
         if len(self.values["reduction"]) > 0:
             reductions_dict: Dict[str, List[str]] = dict()
             for entry in self.values["reduction"]:
                 red_type: str = entry.split(":")[0]
                 var: str = entry.split(":")[1]
                 if red_type not in reductions_dict:
                     reductions_dict[red_type] = []
```

### Comparing `discopop-3.1.1/discopop_library/ConfigProvider/ConfigProviderArguments.py` & `discopop-3.2.0/discopop_library/ConfigProvider/ConfigProviderArguments.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 @dataclass
 class ConfigProviderArguments(object):
     """Container Class for the arguments passed to the discopop_config_provider"""
 
     return_dp_build_dir: bool
     return_dp_source_dir: bool
     return_llvm_bin_dir: bool
+    return_version_string: bool
 
     def __post_init__(self):
         self.__validate()
 
     def __validate(self):
         pass
```

### Comparing `discopop-3.1.1/discopop_library/ConfigProvider/__main__.py` & `discopop-3.2.0/discopop_library/ConfigProvider/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,40 +10,39 @@
 from discopop_library.ConfigProvider.ConfigProviderArguments import ConfigProviderArguments
 from discopop_library.ConfigProvider.config_provider import run
 
 
 def parse_args() -> ConfigProviderArguments:
     """Parse the arguments passed to the discopop_config_provider"""
     parser = ArgumentParser(description="DiscoPoP Config Provider")
-    # all flags that are not considered stable should be added to the experimental_parser
-    experimental_parser = parser.add_argument_group(
-        "EXPERIMENTAL",
-        "Arguments for experimental features. Experimental arguments may or may not be removed or changed in the future.",
-    )
 
     # fmt: off
-    parser.add_argument("-b", "--dp-build-dir", action="store_true",
+    mutually_exclusive = parser.add_mutually_exclusive_group()
+    mutually_exclusive.add_argument("-b", "--dp-build-dir", action="store_true",
                         help="Return the path to the DiscoPoP build directory")
-    parser.add_argument("-s", "--dp-source-dir", action="store_true",
+    mutually_exclusive.add_argument("-s", "--dp-source-dir", action="store_true",
                         help="Return the path to the DiscoPoP source directory")
-    parser.add_argument("--llvm-bin-dir", action="store_true",
+    mutually_exclusive.add_argument("--llvm-bin-dir", action="store_true",
                         help="Return the path to the LLVM bin directory")
+    mutually_exclusive.add_argument("-v", "--version", action="store_true",
+                        help="Return the version string of the DiscoPoP library")
     # EXPERIMENTAL FLAGS:
     # fmt: on
 
     arguments = parser.parse_args()
 
     return ConfigProviderArguments(
         return_dp_build_dir=arguments.dp_build_dir,
         return_dp_source_dir=arguments.dp_source_dir,
         return_llvm_bin_dir=arguments.llvm_bin_dir,
+        return_version_string=arguments.version,
     )
 
 
-def main() -> str:
+def main() -> None:
     arguments = parse_args()
     retval = run(arguments)
-    return retval
+    print(retval)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `discopop-3.1.1/discopop_library/ConfigProvider/config_provider.py` & `discopop-3.2.0/discopop_library/ConfigProvider/config_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,23 +2,25 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
-from typing import cast
 from discopop_library.ConfigProvider.ConfigProviderArguments import ConfigProviderArguments
 from discopop_library.ConfigProvider.assets.build_config import DP_BUILD, DP_SOURCE, LLVM_BIN_DIR  # type: ignore
+from discopop_library.global_data.version.utils import get_version
 
 
 def run(arguments: ConfigProviderArguments) -> str:
     """Returns the contents of the written build_config.txt"""
 
     if arguments.return_dp_build_dir:
-        return cast(str, DP_BUILD)  # type: ignore
+        return DP_BUILD  # type: ignore
     elif arguments.return_dp_source_dir:
-        return cast(str, DP_SOURCE)  # type: ignore
+        return DP_SOURCE  # type: ignore
     elif arguments.return_llvm_bin_dir:
-        return cast(str, LLVM_BIN_DIR)  # type: ignore
+        return LLVM_BIN_DIR  # type: ignore
+    elif arguments.return_version_string:
+        return get_version()
     else:
         raise ValueError("No valid operation for execution configuration: \n" + str(arguments))
```

### Comparing `discopop-3.1.1/discopop_library/JSONHandler/JSONHandler.py` & `discopop-3.2.0/discopop_library/JSONHandler/JSONHandler.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/LineMapping/diff_modifications.py` & `discopop-3.2.0/discopop_library/LineMapping/diff_modifications.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/LineMapping/initialize.py` & `discopop-3.2.0/discopop_library/LineMapping/initialize.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/LineMapping/load.py` & `discopop-3.2.0/discopop_library/LineMapping/load.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/LineMapping/save.py` & `discopop-3.2.0/discopop_library/LineMapping/save.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/MemoryRegions/utils.py` & `discopop-3.2.0/discopop_library/MemoryRegions/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/PatchApplicatorArguments.py` & `discopop-3.2.0/discopop_library/PatchApplicator/PatchApplicatorArguments.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import json
 import sys
 from dataclasses import dataclass
 from typing import List
 
+from discopop_library.ArgumentClasses.GeneralArguments import GeneralArguments
+
 
 @dataclass
-class PatchApplicatorArguments(object):
+class PatchApplicatorArguments(GeneralArguments):
     """Container Class for the arguments passed to the discopop_patch_applicator"""
 
     verbose: bool
     apply: List[str]
     rollback: List[str]
     clear: bool
     load: bool
```

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/__main__.py` & `discopop-3.2.0/discopop_library/PatchApplicator/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 from argparse import ArgumentParser
+from discopop_library.GlobalLogger.setup import setup_logger
 
 from discopop_library.PatchApplicator.PatchApplicatorArguments import PatchApplicatorArguments
 from discopop_library.PatchApplicator.patch_applicator import run
 
 
 def parse_args() -> PatchApplicatorArguments:
     """Parse the arguments passed to the discopop_explorer"""
@@ -33,36 +34,42 @@
                                                                    "the list of applied suggestion for loading."
                                                                    "Old saves will be overwritten!")
     # todo: in the long run, saving configurations to different locations could be easily implemented.
 
     parser.add_argument('-L', '--load', action="store_true", help="Load a previous state after clearing.")
     parser.add_argument('-l', '--list', action="store_true", help="Show the list of applied suggestions."
                                                                   "If set, nothing else will be done.")
+    
+    parser.add_argument("--log", type=str, default="WARNING", help="Specify log level: DEBUG, INFO, WARNING, ERROR, CRITICAL")
+    parser.add_argument("--write-log", action="store_true", help="Create Logfile.")
     # EXPERIMENTAL FLAGS:
     # fmt: on
 
     arguments = parser.parse_args()
 
     return PatchApplicatorArguments(
         verbose=arguments.verbose,
         apply=arguments.apply,
         rollback=arguments.rollback,
         clear=arguments.clear,
         load=arguments.load,
         list=arguments.list,
+        log_level=arguments.log.upper(),
+        write_log=arguments.write_log,
     )
 
 
 def main() -> int:
     """Return values:"
     "0: Applied successfully"
     "1: Nothing applied"
     "2: Some changes applied successfully
     """
     retval = 0
     arguments = parse_args()
+    setup_logger(arguments)
     retval = run(arguments)
     return retval
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/apply.py` & `discopop-3.2.0/discopop_library/PatchApplicator/apply.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/clear.py` & `discopop-3.2.0/discopop_library/PatchApplicator/clear.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/list.py` & `discopop-3.2.0/discopop_library/PatchApplicator/list.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/load.py` & `discopop-3.2.0/discopop_library/PatchApplicator/load.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/patch_applicator.py` & `discopop-3.2.0/discopop_library/PatchApplicator/patch_applicator.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchApplicator/rollback.py` & `discopop-3.2.0/discopop_library/PatchApplicator/rollback.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchGenerator/PatchGeneratorArguments.py` & `discopop-3.2.0/discopop_library/PatchGenerator/PatchGeneratorArguments.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,24 +4,29 @@
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import os.path
 from dataclasses import dataclass
 
+from discopop_library.ArgumentClasses.GeneralArguments import GeneralArguments
+
 
 @dataclass
-class PatchGeneratorArguments(object):
+class PatchGeneratorArguments(GeneralArguments):
     """Container Class for the arguments passed to the discopop_patch_generator"""
 
     verbose: bool
     discopop_build_path: str
     CC: str
     CXX: str
     add_from_json: str
+    # Benchmarking flags
+    only_optimizer_output_patterns: bool
+    only_maximum_id_pattern: bool
 
     def __post_init__(self):
         self.__validate()
 
     def __validate(self):
         """Validate the arguments passed to the discopop_explorer, e.g check if given files exist"""
         if self.verbose:
```

### Comparing `discopop-3.1.1/discopop_library/PatchGenerator/__main__.py` & `discopop-3.2.0/discopop_library/PatchGenerator/__main__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import os.path
 from argparse import ArgumentParser
 from pathlib import Path
+from discopop_library.GlobalLogger.setup import setup_logger
 
 from discopop_library.PatchGenerator.PatchGeneratorArguments import PatchGeneratorArguments
 from discopop_library.PatchGenerator.patch_generator import run
 from discopop_library.ConfigProvider.config_provider import run as run_config_provider
 from discopop_library.ConfigProvider.ConfigProviderArguments import ConfigProviderArguments
 
 
@@ -19,35 +20,48 @@
     """Parse the arguments passed to the discopop_explorer"""
     parser = ArgumentParser(description="DiscoPoP Patch Generator")
     # all flags that are not considered stable should be added to the experimental_parser
     experimental_parser = parser.add_argument_group(
         "EXPERIMENTAL",
         "Arguments marked as experimental features. These flags may or may not be removed or changed in the future.",
     )
+    benchmarking_parser = parser.add_argument_group(
+        "BENCHMARKING",
+        "Arguments marked as benchmarking features. These flags may or may not be removed or changed in the future.",
+    )
 
     # fmt: off
     parser.add_argument("-v", "--verbose", action="store_true",
         help="Enable verbose output.")
     parser.add_argument(
         "-a", "--add-from-json", type=str, default="None",
         help="Add additional patches specified in the given patterns.json file."
     )
+    parser.add_argument("--log", type=str, default="WARNING", help="Specify log level: DEBUG, INFO, WARNING, ERROR, CRITICAL")
+    parser.add_argument("--write-log", action="store_true", help="Create Logfile.")
     # EXPERIMENTAL FLAGS:
+    # BENCHMARKING FLAGS:
+    benchmarking_parser.add_argument("--only-optimizer-output-patterns", action="store_true", help="Only generate code for optimizer_output patterns.")
+    benchmarking_parser.add_argument("--only-maximum-id-pattern", action="store_true", help="Only generate code for the pattern with the highest id.")
     # fmt: on
 
     arguments = parser.parse_args()
 
     # determine DP build path
     arguments.dp_build_path = run_config_provider(
-        ConfigProviderArguments(return_dp_build_dir=True, return_dp_source_dir=False, return_llvm_bin_dir=False)
+        ConfigProviderArguments(
+            return_dp_build_dir=True, return_dp_source_dir=False, return_llvm_bin_dir=False, return_version_string=False
+        )
     )
 
     # determine LLVM_BIN_DIR
     llvm_bin_dir = run_config_provider(
-        ConfigProviderArguments(return_dp_build_dir=False, return_dp_source_dir=False, return_llvm_bin_dir=True)
+        ConfigProviderArguments(
+            return_dp_build_dir=False, return_dp_source_dir=False, return_llvm_bin_dir=True, return_version_string=False
+        )
     )
     # determine CC
     if os.path.exists(os.path.join(llvm_bin_dir, "clang")):
         arguments.cc = os.path.join(llvm_bin_dir, "clang")
     elif os.path.exists(os.path.join(llvm_bin_dir, "clang-11")):
         arguments.cc = os.path.join(llvm_bin_dir, "clang-11")
     else:
@@ -63,17 +77,22 @@
 
     return PatchGeneratorArguments(
         verbose=arguments.verbose,
         discopop_build_path=arguments.dp_build_path,
         CC=arguments.cc,
         CXX=arguments.cxx,
         add_from_json=arguments.add_from_json,
+        only_optimizer_output_patterns=arguments.only_optimizer_output_patterns,
+        log_level=arguments.log.upper(),
+        write_log=arguments.write_log,
+        only_maximum_id_pattern=arguments.only_maximum_id_pattern,
     )
 
 
 def main():
     arguments = parse_args()
+    setup_logger(arguments)
     run(arguments)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `discopop-3.1.1/discopop_library/PatchGenerator/diffs.py` & `discopop-3.2.0/discopop_library/PatchGenerator/diffs.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchGenerator/from_json_patterns.py` & `discopop-3.2.0/discopop_library/PatchGenerator/from_json_patterns.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,41 +3,71 @@
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 import json
+import logging
 import os.path
 from pathlib import Path
 import shutil
 from typing import Dict, List
 from discopop_library.CodeGenerator.CodeGenerator import from_json_strings
 from discopop_library.PatchGenerator.PatchGeneratorArguments import PatchGeneratorArguments
 from discopop_library.PatchGenerator.diffs import get_diffs_from_modified_code
 from discopop_library.PatchGenerator.from_optimizer_output import from_optimizer_output
 
+logger = logging.getLogger("PatchGenerator")
+
 
 def from_json_patterns(
     arguments: PatchGeneratorArguments,
     patterns_by_type: Dict[str, List[str]],
     file_mapping: Dict[int, Path],
     patch_generator_dir: str,
 ):
+    # collect metadata
+    max_pattern_id = 0
+    for suggestion_type in patterns_by_type:
+        for suggestion in patterns_by_type[suggestion_type]:
+            suggestion_dict = json.loads(suggestion)
+            suggestion_id = suggestion_dict["pattern_id"]
+            if max_pattern_id < suggestion_id:
+                max_pattern_id = suggestion_id
+    logger.debug("max_pattern_id = " + str(max_pattern_id))
+
     # generate code modifications from each suggestion, create a patch and store the patch
     # using the suggestions unique id
     if arguments.verbose:
         print("Generating modified code...")
     for suggestion_type in patterns_by_type:
         if suggestion_type == "version":
             continue
         for suggestion in patterns_by_type[suggestion_type]:
-            if suggestion_type == "optimizer_output":
+            # parse benchmarking flags
+            if arguments.only_optimizer_output_patterns and suggestion_type != "optimizer_output":
+                # ignore all other pattern types
+                logger.debug("Ignoring pattern of type: " + suggestion_type)
+                continue
+
+            suggestion_dict = json.loads(suggestion)
+            if not suggestion_dict["applicable_pattern"]:
+                continue
+
+            # parse benchmarking flags
+            if arguments.only_maximum_id_pattern:
+                if suggestion_dict["pattern_id"] != max_pattern_id:
+                    logger.debug("Skipping pattern: " + str(suggestion_dict["pattern_id"]))
+                    continue
+
+            if suggestion_type in ["optimizer_output", "merged_pattern"]:
                 from_optimizer_output(file_mapping, patterns_by_type, suggestion, arguments, patch_generator_dir)
                 continue
+
             if arguments.verbose:
                 print("Suggestion: ", suggestion)
             file_id_to_modified_code: Dict[int, str] = from_json_strings(
                 file_mapping,
                 {suggestion_type: [suggestion]},
                 CC=arguments.CC,
                 CXX=arguments.CXX,
```

### Comparing `discopop-3.1.1/discopop_library/PatchGenerator/from_optimizer_output.py` & `discopop-3.2.0/discopop_library/PatchGenerator/from_optimizer_output.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatchGenerator/patch_generator.py` & `discopop-3.2.0/discopop_library/PatchGenerator/patch_generator.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,28 +2,31 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import json
+import logging
 import os.path
 import shutil
 from typing import Dict
 
 from discopop_library.CodeGenerator.CodeGenerator import from_json_strings
 from discopop_library.JSONHandler.JSONHandler import read_patterns_from_json_to_json
 from discopop_library.PatchGenerator.PatchGeneratorArguments import PatchGeneratorArguments
 from discopop_library.PatchGenerator.from_optimizer_output import from_optimizer_output
 from discopop_library.PatchGenerator.diffs import get_diffs_from_modified_code
 from discopop_library.PatchGenerator.from_json_patterns import from_json_patterns
 from discopop_library.PathManagement.PathManagement import load_file_mapping
 
 
 def run(arguments: PatchGeneratorArguments):
+    logger = logging.getLogger("PatchGenerator")
+
     if arguments.verbose:
         print("Started DiscoPoP Patch Generator...")
     if arguments.verbose:
         print("Creating patch_generator directory...")
     patch_generator_dir = os.path.join(os.getcwd(), "patch_generator")
     if not os.path.exists(patch_generator_dir):
         os.mkdir(patch_generator_dir)
```

### Comparing `discopop-3.1.1/discopop_library/PathManagement/PathManagement.py` & `discopop-3.2.0/discopop_library/PathManagement/PathManagement.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/PatternIdManagement/unique_pattern_id.py` & `discopop-3.2.0/discopop_library/PatternIdManagement/unique_pattern_id.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/CostModel.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/CostModel.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/DataTransfer/DataTransferCosts.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/DataTransfer/DataTransferCosts.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/CostModels/utilities.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/CostModels/utilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import copy
 import random
 from typing import List, Dict, cast, Set, Optional
+import warnings
 
 import networkx as nx  # type: ignore
 import sympy  # type: ignore
 from sympy import Integer, Expr, Symbol  # type: ignore
 
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
@@ -44,36 +45,65 @@
     ]
 
     for node_id in graph.nodes:
         node_data = graph.nodes[node_id]["data"]
         node_data.node_id = node_id  # fix potential mismatches due to node copying
 
         if isinstance(node_data, FunctionRoot):
-            # start the collection at the first child of the function
-            for child_id in get_children(graph, node_id):
-                performance_models[node_data] = get_node_performance_models(
-                    experiment, graph, child_id, set(), all_function_nodes, restrict_to_decisions=restrict_to_decisions
-                )
+            try:
+                # ignore non-hotspot functions in the calculateion to save analysis time
+                if (
+                    node_id not in experiment.hotspot_function_node_ids
+                    and len(experiment.hotspot_function_node_ids) > 0
+                ):
+                    print("SKIPPING NON-HOTPSOT FUNCTION: ", node_data.name, "ID: ", node_id, " SET COSTS TO 1")
+                    performance_models[node_data] = [CostModel(Integer(0), Integer(1))]
+                    continue
 
-            # At this point, decisions are restricted to the specified parallelization or the sequential version.
-            # Restrict them to the exact case specified in restrict_to_decisions
-            if restrict_to_decisions is not None:
-                to_be_removed: List[int] = []
-                for idx, cost_model in enumerate(performance_models[node_data]):
-                    for decision in cost_model.path_decisions:
-                        if decision not in restrict_to_decisions:
-                            to_be_removed.append(idx)
-                            break
-                for idx in sorted(to_be_removed, reverse=True):
-                    del performance_models[node_data][idx]
+                # start the collection at the first child of the function
+                for child_id in get_children(graph, node_id):
+                    performance_models[node_data] = get_node_performance_models(
+                        experiment,
+                        graph,
+                        child_id,
+                        set(),
+                        all_function_nodes,
+                        restrict_to_decisions=restrict_to_decisions,
+                        allow_sequential=True,
+                    )
+
+                # At this point, decisions are restricted to the specified parallelization or the sequential version.
+                # Restrict them to the exact case specified in restrict_to_decisions
+                if restrict_to_decisions is not None:
+                    to_be_removed: List[int] = []
+                    for idx, cost_model in enumerate(performance_models[node_data]):
+                        for decision in cost_model.path_decisions:
+                            if decision not in restrict_to_decisions:
+                                # check if the decision to be removed is a sequential execution. If so, ignore it
+                                if data_at(graph, decision).represents_sequential_version():
+                                    continue
+                                # decision represents a not-allowes, parallel execution. Remove it.
+                                to_be_removed.append(idx)
+                                break
+                    for idx in sorted(to_be_removed, reverse=True):
+                        del performance_models[node_data][idx]
 
-            # filter out NaN - Models
-            performance_models[node_data] = [
-                model for model in performance_models[node_data] if model.parallelizable_costs != sympy.nan
-            ]
+                # filter out NaN - Models
+                performance_models[node_data] = [
+                    model for model in performance_models[node_data] if model.parallelizable_costs != sympy.nan
+                ]
+            except KeyError as ke:
+                performance_models[node_data] = [CostModel(Integer(0), Integer(1))]
+                warnings.warn(
+                    "No performance model for "
+                    + node_data.name
+                    + "found due to the following error: "
+                    + str(ke)
+                    + ". Model set to Fallback (0,1)"
+                )
 
     return performance_models
 
 
 def get_node_performance_models(
     experiment: Experiment,
     graph: nx.DiGraph,
@@ -81,224 +111,239 @@
     visited_nodes: Set[int],
     all_function_nodes: List[FunctionRoot],
     restrict_to_decisions: Optional[Set[int]] = None,
     do_not_allow_decisions: Optional[Set[int]] = None,
     get_single_random_model: bool = False,
     ignore_node_costs: Optional[List[int]] = None,
     current_device_id=None,
+    allow_sequential: bool = False,
 ) -> List[CostModel]:
     """Returns the performance models for the given node.
     If a set of decision is specified for restrict_to_decisions, only those non-sequential decisions will be allowed.
     Caution: List might be empty!
     """
-    result_list: List[CostModel] = []
-    successors = get_successors(graph, node_id)
-    successor_count = len(successors)
-    node_data = data_at(graph, node_id)
-    if node_data.execute_in_parallel:
-        current_device_id = node_data.device_id
-    visited_nodes.add(node_id)
-
-    # consider performance models of children
-    children_models = get_performance_models_for_children(
-        experiment,
-        graph,
-        node_id,
-        copy.deepcopy(visited_nodes),
-        all_function_nodes,
-        restrict_to_decisions=restrict_to_decisions,
-        do_not_allow_decisions=do_not_allow_decisions,
-        get_single_random_model=get_single_random_model,
-    )
-
-    if len(children_models) == 0:
-        if ignore_node_costs is not None:
-            if node_data.node_id in ignore_node_costs:
-                children_models = [CostModel(Integer(0), Integer(0))]
+    try:
+        result_list: List[CostModel] = []
+        successors = get_successors(graph, node_id)
+        successor_count = len(successors)
+        node_data = data_at(graph, node_id)
+        if node_data.execute_in_parallel:
+            current_device_id = node_data.device_id
+        visited_nodes.add(node_id)
+
+        # consider performance models of children
+        children_models = get_performance_models_for_children(
+            experiment,
+            graph,
+            node_id,
+            copy.deepcopy(visited_nodes),
+            all_function_nodes,
+            restrict_to_decisions=restrict_to_decisions,
+            do_not_allow_decisions=do_not_allow_decisions,
+            get_single_random_model=get_single_random_model,
+        )
+
+        if len(children_models) == 0:
+            if ignore_node_costs is not None:
+                if node_data.node_id in ignore_node_costs:
+                    children_models = [CostModel(Integer(0), Integer(0))]
+            else:
+                children_models = [
+                    node_data.get_cost_model(
+                        experiment,
+                        all_function_nodes,
+                        experiment.get_system().get_device(current_device_id),
+                    )
+                ]
+
         else:
-            children_models = [
-                node_data.get_cost_model(
+            if ignore_node_costs is not None:
+                if node_data.node_id in ignore_node_costs:
+                    tmp_node_cost_model = CostModel(Integer(0), Integer(0))
+            else:
+                tmp_node_cost_model = node_data.get_cost_model(
                     experiment,
                     all_function_nodes,
                     experiment.get_system().get_device(current_device_id),
                 )
-            ]
 
-    else:
-        if ignore_node_costs is not None:
-            if node_data.node_id in ignore_node_costs:
-                tmp_node_cost_model = CostModel(Integer(0), Integer(0))
-        else:
-            tmp_node_cost_model = node_data.get_cost_model(
-                experiment,
-                all_function_nodes,
-                experiment.get_system().get_device(current_device_id),
-            )
-
-        for idx, child_model in enumerate(children_models):
-            if ignore_node_costs is not None:
-                if node_data.node_id not in ignore_node_costs:
+            for idx, child_model in enumerate(children_models):
+                if ignore_node_costs is not None:
+                    if node_data.node_id not in ignore_node_costs:
+                        children_models[idx] = tmp_node_cost_model.register_child(
+                            child_model,
+                            node_data,
+                            experiment,
+                            all_function_nodes,
+                            experiment.get_system().get_device(current_device_id),
+                        )
+                else:
                     children_models[idx] = tmp_node_cost_model.register_child(
                         child_model,
                         node_data,
                         experiment,
                         all_function_nodes,
                         experiment.get_system().get_device(current_device_id),
                     )
-            else:
-                children_models[idx] = tmp_node_cost_model.register_child(
-                    child_model,
-                    node_data,
-                    experiment,
-                    all_function_nodes,
-                    experiment.get_system().get_device(current_device_id),
-                )
 
-    # construct the performance models
-    if successor_count >= 1:
-        removed_successors = False
-        if get_single_random_model and successor_count > 1:
-            # pick only a single successor
-            successors = [random.choice(successors)]
-            removed_successors = True
-
-        for children_model in children_models:
-            for successor in successors:
-                # ## CHECK REQUIREMENTS ##
-                # check if successor validates a requirements edge to restrain the created combinations
-                # 1.1. check if optionEdge between any node in visited_nodes and successor exists
-                # 1.2. if so, check if option edge to other node in visited nodes exists
-                # 1.3. if so, check if a requirements edge between both option exists.
-                # 1.4. if not, the path is not valid since two options for the same
-                #      source code location would be selected
-                path_invalid = False
-                # 1.1
-                #               if successor in [109, 110, 111, 112, 113, 114]:
-                #                      print("VISITED NODES: ", visited_nodes)
-                for visited_node_id in visited_nodes:
-                    options = get_out_mutex_edges(graph, visited_node_id)
-                    if successor in options:
-                        # 1.2
-                        visited_options = [opt for opt in options if opt in visited_nodes]
-                        if len(visited_options) > 0:
-                            # 1.3
-                            for vo in visited_options:
-                                # 1.4
-                                if successor not in get_requirements(graph, vo):
-                                    path_invalid = True
-                                    break
+        # construct the performance models
+        if successor_count >= 1:
+            removed_successors = False
+            if get_single_random_model and successor_count > 1:
+                # pick only a single successor
+                successors = [random.choice(successors)]
+                removed_successors = True
+
+            for children_model in children_models:
+                for successor in successors:
+                    # ## CHECK REQUIREMENTS ##
+                    # check if successor validates a requirements edge to restrain the created combinations
+                    # 1.1. check if optionEdge between any node in visited_nodes and successor exists
+                    # 1.2. if so, check if option edge to other node in visited nodes exists
+                    # 1.3. if so, check if a requirements edge between both option exists.
+                    # 1.4. if not, the path is not valid since two options for the same
+                    #      source code location would be selected
+                    path_invalid = False
+                    # 1.1
+                    #               if successor in [109, 110, 111, 112, 113, 114]:
+                    #                      print("VISITED NODES: ", visited_nodes)
+                    for visited_node_id in visited_nodes:
+                        options = get_out_mutex_edges(graph, visited_node_id)
+                        if successor in options:
+                            # 1.2
+                            visited_options = [opt for opt in options if opt in visited_nodes]
+                            if len(visited_options) > 0:
+                                # 1.3
+                                for vo in visited_options:
+                                    # 1.4
+                                    if successor not in get_requirements(graph, vo):
+                                        path_invalid = True
+                                        break
+                        if path_invalid:
+                            break
                     if path_invalid:
-                        break
-                if path_invalid:
-                    continue
+                        continue
 
-                # 2 check if a sibling of successor exists which has a requirements edge to a visited node
-                # 2.1 check if an incoming or outgoing option edge exists, get the node id for the sequential version
-                # 2.2 for all parallelization options
-                # 2.3 check if a requirements edge to a visited node exists
-                # 2.4 if so, stop if successor is NOT the parallelization option with the requirements edge
-                # 2.1
-                for sibling in successors:
-                    sequential_version_ids = []
-                    if len(get_out_mutex_edges(graph, sibling)) > 0:
-                        sequential_version_ids = [sibling]
-                    else:
-                        for seq in get_in_mutex_edges(graph, sibling):
-                            sequential_version_ids.append(seq)
-                    # 2.2
-                    for seq in sequential_version_ids:
-                        for option in get_out_mutex_edges(graph, seq):
-                            if option == successor:
-                                continue
-                            # 2.3
-                            for visited_req in [req for req in get_requirements(graph, option) if req in visited_nodes]:
-                                # 2.4
-                                if visited_req != successor:
+                    # 2 check if a sibling of successor exists which has a requirements edge to a visited node
+                    # 2.1 check if an incoming or outgoing option edge exists, get the node id for the sequential version
+                    # 2.2 for all parallelization options
+                    # 2.3 check if a requirements edge to a visited node exists
+                    # 2.4 if so, stop if successor is NOT the parallelization option with the requirements edge
+                    # 2.1
+                    for sibling in successors:
+                        sequential_version_ids = []
+                        if len(get_out_mutex_edges(graph, sibling)) > 0:
+                            sequential_version_ids = [sibling]
+                        else:
+                            for seq in get_in_mutex_edges(graph, sibling):
+                                sequential_version_ids.append(seq)
+                        # 2.2
+                        for seq in sequential_version_ids:
+                            for option in get_out_mutex_edges(graph, seq):
+                                if option == successor:
+                                    continue
+                                # 2.3
+                                for visited_req in [
+                                    req for req in get_requirements(graph, option) if req in visited_nodes
+                                ]:
+                                    # 2.4
+                                    if visited_req != successor:
+                                        path_invalid = True
+                                        break
+                                if path_invalid:
+                                    break
+                        if path_invalid:
+                            break
+
+                    # do not allow nested parallelization suggestions on devices of type GPU
+                    if True:  # option to disable this check
+                        combined_visited_nodes = copy.deepcopy(visited_nodes)
+                        combined_visited_nodes.add(successor)
+                        gpu_suggestions = [
+                            node_id
+                            for node_id in combined_visited_nodes
+                            if isinstance(
+                                experiment.get_system().get_device(data_at(graph, node_id).device_id),
+                                GPU,
+                            )
+                        ]
+                        # check if two suggestions are in a contained-in relation
+                        for suggestion_1 in gpu_suggestions:
+                            all_parents = get_all_parents(graph, suggestion_1)
+                            for suggestion_2 in gpu_suggestions:
+                                if suggestion_1 == suggestion_2:
+                                    continue
+                                if suggestion_2 in all_parents:
                                     path_invalid = True
                                     break
                             if path_invalid:
                                 break
-                    if path_invalid:
-                        break
 
-                # do not allow nested parallelization suggestions on devices of type GPU
-                if True:  # option to disable this check
-                    combined_visited_nodes = copy.deepcopy(visited_nodes)
-                    combined_visited_nodes.add(successor)
-                    gpu_suggestions = [
-                        node_id
-                        for node_id in combined_visited_nodes
-                        if isinstance(
-                            experiment.get_system().get_device(data_at(graph, node_id).device_id),
-                            GPU,
-                        )
-                    ]
-                    # check if two suggestions are in a contained-in relation
-                    for suggestion_1 in gpu_suggestions:
-                        all_parents = get_all_parents(graph, suggestion_1)
-                        for suggestion_2 in gpu_suggestions:
-                            if suggestion_1 == suggestion_2:
-                                continue
-                            if suggestion_2 in all_parents:
-                                path_invalid = True
-                                break
-                        if path_invalid:
-                            break
+                    # check if the current decision invalidates decision requirements, if some are specified
+                    if restrict_to_decisions is not None:
+                        if not (successor in restrict_to_decisions or data_at(graph, successor).suggestion is None):
+                            path_invalid = True
+                        if not path_invalid:
+                            if data_at(graph, successor).suggestion is None:
+                                # if the sequential "fallback" has been used, check if a different option is specifically
+                                # mentioned in restrict_to_decisions. If so, the sequential fallback shall be ignored.
+                                options = get_out_mutex_edges(graph, successor)
+                                restricted_options = [opt for opt in options if opt in restrict_to_decisions]
+                                if len(restricted_options) != 0:
+                                    # do not use he sequential fallback since a required option exists
+                                    path_invalid = True
 
-                # check if the current decision invalidates decision requirements, if some are specified
-                if restrict_to_decisions is not None:
-                    if not (successor in restrict_to_decisions or data_at(graph, successor).suggestion is None):
-                        path_invalid = True
-                    if not path_invalid:
-                        if data_at(graph, successor).suggestion is None:
-                            # if the sequential "fallback" has been used, check if a different option is specifically
-                            # mentioned in restrict_to_decisions. If so, the sequential fallback shall be ignored.
-                            options = get_out_mutex_edges(graph, successor)
-                            restricted_options = [opt for opt in options if opt in restrict_to_decisions]
-                            if len(restricted_options) != 0:
-                                # do not use he sequential fallback since a required option exists
-                                path_invalid = True
-
-                if do_not_allow_decisions is not None:
-                    if successor in do_not_allow_decisions:
-                        path_invalid = True
+                    if do_not_allow_decisions is not None:
+                        if successor in do_not_allow_decisions:
+                            path_invalid = True
 
-                if path_invalid:
-                    continue
+                    if path_invalid:
+                        continue
 
-                # ## END OF REQUIREMENTS CHECK ##
+                    # ## END OF REQUIREMENTS CHECK ##
 
-                combined_model = children_model
-                # add transfer costs
-                transfer_costs_model = get_edge_data(graph, node_id, successor).get_cost_model()
-                combined_model = combined_model.parallelizable_plus_combine(transfer_costs_model)
-
-                # if the successor is "determined" by a path decision, add path decision to the combined model
-                if len(successors) > 1 or removed_successors:
-                    combined_model.path_decisions.append(successor)
-                # append the model of the successor
-                for model in get_node_performance_models(
-                    experiment,
-                    graph,
-                    successor,
-                    copy.deepcopy(visited_nodes),
-                    all_function_nodes,
-                    restrict_to_decisions=restrict_to_decisions,
-                    do_not_allow_decisions=do_not_allow_decisions,
-                    get_single_random_model=get_single_random_model,
-                    ignore_node_costs=ignore_node_costs,
-                ):
-                    tmp = combined_model.parallelizable_plus_combine(model)
-                    tmp.path_decisions += [d for d in model.path_decisions if d not in tmp.path_decisions]
-                    result_list.append(tmp)
-        if len(result_list) >= 1:
-            return result_list
-
-    # successor count == 0 or successor count > 1
-    return children_models
+                    combined_model = children_model
+                    # add transfer costs
+                    transfer_costs_model = get_edge_data(graph, node_id, successor).get_cost_model()
+                    combined_model = combined_model.parallelizable_plus_combine(transfer_costs_model)
+
+                    # if the successor is "determined" by a path decision, add path decision to the combined model
+                    if len(successors) > 1 or removed_successors:
+                        combined_model.path_decisions.append(successor)
+                    # append the model of the successor
+                    for model in get_node_performance_models(
+                        experiment,
+                        graph,
+                        successor,
+                        copy.deepcopy(visited_nodes),
+                        all_function_nodes,
+                        restrict_to_decisions=restrict_to_decisions,
+                        do_not_allow_decisions=do_not_allow_decisions,
+                        get_single_random_model=get_single_random_model,
+                        ignore_node_costs=ignore_node_costs,
+                    ):
+                        tmp = combined_model.parallelizable_plus_combine(model)
+                        tmp.path_decisions += [d for d in model.path_decisions if d not in tmp.path_decisions]
+                        result_list.append(tmp)
+            if len(result_list) >= 1:
+                return result_list
+
+        # successor count == 0 or successor count > 1
+        return children_models
+
+    except RecursionError:
+        warnings.warn("Allowed recursion depth exceeded at node " + str(node_id) + " . Results may be inaccurate.")
+        node_data = data_at(graph, node_id)
+        return [
+            node_data.get_cost_model(
+                experiment,
+                all_function_nodes,
+                experiment.get_system().get_device(current_device_id),
+            )
+        ]
 
 
 def get_performance_models_for_children(
     experiment: Experiment,
     graph: nx.DiGraph,
     node_id: int,
     visited_nodes: Set[int],
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/DataTransfers/DataTransfers.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/DataTransfers/DataTransfers.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
-from typing import Dict, List, Optional, Tuple, cast
+from typing import Dict, List, Optional, Set, Tuple, cast
 
 import networkx as nx  # type: ignore
+from discopop_explorer.PEGraphX import EdgeType, MemoryRegion
 
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.classes.context.ContextObject import ContextObject
 from discopop_library.discopop_optimizer.classes.nodes.ContextNode import ContextNode
+from discopop_library.discopop_optimizer.classes.nodes.DeviceSwitch import DeviceSwitch
 from discopop_library.discopop_optimizer.classes.nodes.FunctionRoot import FunctionRoot
+from discopop_library.discopop_optimizer.classes.nodes.SynchronizationTrigger import SynchronizationTrigger
+from discopop_library.discopop_optimizer.classes.types.DataAccessType import ReadDataAccess, WriteDataAccess
 from discopop_library.discopop_optimizer.utilities.MOGUtilities import (
+    get_all_nodes_in_function,
+    get_function_return_node,
+    get_predecessors,
     get_requirements,
     get_successors,
     get_children,
     show,
 )
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 
@@ -28,21 +35,28 @@
     """Calculate data transfers for each performance model and append the respective ContextObject to the result."""
     result_dict: Dict[FunctionRoot, List[Tuple[CostModel, ContextObject]]] = dict()
     for function in function_performance_models:
         result_dict[function] = []
         for model in function_performance_models[function]:
             # create a ContextObject for the current path
             context = ContextObject(function.node_id, [function.device_id])
-            context = get_path_context_iterative(function.node_id, graph, model, context, experiment)
+            context = get_path_context_iterative(
+                function.node_id, graph, model, context, experiment, top_level_call=False
+            )
             result_dict[function].append((model, context))
     return result_dict
 
 
 def get_path_context_iterative(
-    root_node_id: int, graph: nx.DiGraph, model: CostModel, context: ContextObject, experiment
+    root_node_id: int,
+    graph: nx.DiGraph,
+    model: CostModel,
+    context: ContextObject,
+    experiment,
+    top_level_call: bool = False,
 ) -> ContextObject:
     """passes the context Object along the path and returns the context once the end has been reached"""
     node_id = None
     next_node_id: Optional[int] = root_node_id
 
     while next_node_id is not None:
         node_id = next_node_id
@@ -121,14 +135,64 @@
                         model.path_decisions,
                         "successors:",
                         successors,
                     )
             # suitable successor identified.
             # pass the current context to the successor
             next_node_id = suitable_successors[0]
+
+    # force update to host device of the function (not system host device, to allow offloading functions to devices)
+    # TODO CURRENTLY UNUSED, REACTIVATE?
+    if top_level_call:
+        # force synchronization with executing device
+
+        # create a filter for the data accesses to be synchronized
+        # only consider such memory regions which are used outside the function
+        filter: Set[MemoryRegion] = set()
+        nodes_in_function = get_all_nodes_in_function(graph, root_node_id)
+        cu_nodes_in_function = set([data_at(graph, n).original_cu_id for n in nodes_in_function])
+        for node in nodes_in_function:
+            node_data = data_at(graph, node)
+            if node_data.original_cu_id is None:
+                continue
+            for out_dep_edge in experiment.detection_result.pet.out_edges(
+                node_data.original_cu_id, etype=EdgeType.DATA
+            ):
+                target = out_dep_edge[1]
+                if target in cu_nodes_in_function:
+                    continue
+                # target outside the function. MemoryRegions qualifies for synchronization at the end of the function
+                filter.add(out_dep_edge[2].memory_region)
+
+        # collect all write data accesses which might need synchronization
+        seen_writes: Set[WriteDataAccess] = set()
+        for device_id in context.seen_writes_by_device:
+            for mem_reg in context.seen_writes_by_device[device_id]:
+                for wda in context.seen_writes_by_device[device_id][mem_reg]:
+                    # check wda against filter
+                    if wda.memory_region in filter:
+                        seen_writes.add(wda)
+
+        reading_device_id = data_at(graph, root_node_id).device_id
+        reading_device_id = (
+            experiment.get_system().get_host_device_id() if reading_device_id is None else reading_device_id
+        )
+        forced_sync_context = context.calculate_and_perform_necessary_updates(
+            cast(Set[ReadDataAccess], seen_writes),
+            reading_device_id,
+            get_function_return_node(graph, root_node_id),
+            graph,
+            experiment,
+        )
+
+        # add the writes performed by the given node to the context
+        forced_sync_context = forced_sync_context.add_writes(
+            node_data.written_memory_regions, cast(int, context.last_seen_device_ids[-1])
+        )
+
     return context
 
 
 def get_path_context(
     node_id: int, graph: nx.DiGraph, model: CostModel, context: ContextObject, experiment
 ) -> ContextObject:
     """passes the context Object along the path and returns the context once the end has been reached"""
@@ -222,29 +286,60 @@
         # apply modifications according to encountered context node
         updated_context = cast(ContextNode, data_at(graph, node_id)).get_modified_context(
             node_id, graph, model, context
         )
         return updated_context
 
     # only allow updates on device switches
-    device_switch = False
+
+    device_switch_occured = False
     if data_at(graph, node_id).device_id is None:
         if context.last_seen_device_ids[-1] != context.last_visited_device_id:
-            device_switch = True
+            device_switch_occured = True
     elif context.last_visited_device_id != data_at(graph, node_id).device_id:
-        device_switch = True
+        device_switch_occured = True
 
-    if device_switch:
+    # TODO: if a device switch is encountered, collect read / written data unitl next device switch
+
+    #    if device_switch or type(node_data) == SynchronizationTrigger or True:
+
+    if type(node_data) == SynchronizationTrigger or type(node_data) == DeviceSwitch:
+        # identify updates at a designated synchronization point
         context = context.calculate_and_perform_necessary_updates(
             node_data.read_memory_regions,
             cast(int, context.last_seen_device_ids[-1]),
             node_data.node_id,
             graph,
             experiment,
         )
+    elif device_switch_occured:
+        # identify updates due to suggestion entries
+        # attribute the updates to the last visited DeviceSwitch if necessary
+        last_seen_device_switch_node = None
+        queue = [node_id]
+        while len(queue) > 0:
+            current = queue.pop()
+            current_data = data_at(graph, current)
+            if type(current_data) == DeviceSwitch:
+                last_seen_device_switch_node = current
+                break
+            queue += [p for p in get_predecessors(graph, current) if p not in queue]
+
+        if last_seen_device_switch_node is not None:
+            context = context.calculate_and_perform_necessary_updates(
+                node_data.read_memory_regions,
+                cast(int, context.last_seen_device_ids[-1]),
+                last_seen_device_switch_node,
+                graph,
+                experiment,
+                updates_originated_from=node_id,
+            )
+        else:
+            # this can be the case for function nodes and similar
+            pass
 
     # add the writes performed by the given node to the context
     context = context.add_writes(node_data.written_memory_regions, cast(int, context.last_seen_device_ids[-1]))
 
     return context
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/DelaunayInterpolatedMicrobench.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/DelaunayInterpolatedMicrobench.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/ExtrapInterpolatedMicrobench.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/ExtrapInterpolatedMicrobench.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/Microbench.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/Microbench.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,18 @@
     iterations: int
 
 
 class Microbench(ABC):
     @abstractmethod
     def getMeasurements(
         self,
-    ) -> Dict[MicrobenchType, Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],]:
+    ) -> Dict[
+        MicrobenchType,
+        Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],
+    ]:
         raise TypeError("Pure virtual method called")
 
     @abstractmethod
     def toJSON(self) -> str:
         raise TypeError("Pure virtual method called")
 
     @abstractmethod
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/MicrobenchParser.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/MicrobenchParser.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/MixedMicrobench.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/MixedMicrobench.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,27 +22,36 @@
     def __init__(self, inner: Microbench, outer: Microbench, threshold: MicrobenchCoordinate):
         self.inner = inner
         self.outer = outer
         self.threshold = threshold
 
     def getMeasurements(
         self,
-    ) -> Dict[MicrobenchType, Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],]:
+    ) -> Dict[
+        MicrobenchType,
+        Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],
+    ]:
         raise TypeError(
             "This MixedMicrobench might be based on two different sets of measurements. Use getInnerMeasurements() or getOuterMeasurements() instead."
         )
 
     def getInnerMeasurements(
         self,
-    ) -> Dict[MicrobenchType, Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],]:
+    ) -> Dict[
+        MicrobenchType,
+        Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],
+    ]:
         return self.inner.getMeasurements()
 
     def getOuterMeasurements(
         self,
-    ) -> Dict[MicrobenchType, Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],]:
+    ) -> Dict[
+        MicrobenchType,
+        Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],
+    ]:
         return self.outer.getMeasurements()
 
     def toJSON(self) -> str:
         raise TypeError("This class does not support JSON serialization.")
 
     def evaluateInterpolation(
         self,
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/PureDataMicrobench.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/PureDataMicrobench.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,24 +48,25 @@
 class PureDataMicrobench(Microbench):
     measurements: Dict[
         MicrobenchType,
         Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],
     ]
 
     @overload
-    def __getitem__(self, key: MicrobenchType) -> Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]]:
-        ...
+    def __getitem__(
+        self, key: MicrobenchType
+    ) -> Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]]: ...
 
     @overload
-    def __getitem__(self, key: Tuple[MicrobenchType, MicrobenchDimension]) -> Dict[MicrobenchCoordinate, List[float]]:
-        ...
+    def __getitem__(
+        self, key: Tuple[MicrobenchType, MicrobenchDimension]
+    ) -> Dict[MicrobenchCoordinate, List[float]]: ...
 
     @overload
-    def __getitem__(self, key: Tuple[MicrobenchType, MicrobenchDimension, MicrobenchCoordinate]) -> List[float]:
-        ...
+    def __getitem__(self, key: Tuple[MicrobenchType, MicrobenchDimension, MicrobenchCoordinate]) -> List[float]: ...
 
     # allow to use this class like a dictionary
     def __getitem__(self, key):
         if isinstance(key, MicrobenchType):
             return self.measurements[key]
         elif (
             (isinstance(key, tuple) or isinstance(key, List))
@@ -177,15 +178,18 @@
     def mergeAll(self, others: List[PureDataMicrobench]):
         for other in others:
             self.merge(other)
 
     # inherited from Microbench
     def getMeasurements(
         self,
-    ) -> Dict[MicrobenchType, Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],]:
+    ) -> Dict[
+        MicrobenchType,
+        Dict[MicrobenchDimension, Dict[MicrobenchCoordinate, List[float]]],
+    ]:
         return self.measurements
 
     # inherited from Microbench
     def toJSON(self) -> str:
         return json.dumps(
             {
                 "measurements": {
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Microbench/utils.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Microbench/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/OptimizationGraph.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/OptimizationGraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,17 +121,17 @@
         # add function symbols to list of substitutions
         # collect substitutions
         for function in experiment.selected_paths_per_function:
             # register substitution
             experiment.substitutions[cast(Symbol, function.sequential_costs)] = experiment.selected_paths_per_function[
                 function
             ][0].sequential_costs
-            experiment.substitutions[
-                cast(Symbol, function.parallelizable_costs)
-            ] = experiment.selected_paths_per_function[function][0].parallelizable_costs
+            experiment.substitutions[cast(Symbol, function.parallelizable_costs)] = (
+                experiment.selected_paths_per_function[function][0].parallelizable_costs
+            )
 
         # TODO END OF DUMMY
 
         # set free symbol ranges and distributions for comparisons
         #        for idx, function in enumerate(complete_performance_models):
         #            for pair in complete_performance_models[function]:
         #                model, context = pair
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/OptimizerArguments.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/OptimizerArguments.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,42 +5,51 @@
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import os.path
 from dataclasses import dataclass
 from typing import List, Optional
 
+from discopop_library.ArgumentClasses.GeneralArguments import GeneralArguments
+
 
 @dataclass
-class OptimizerArguments(object):
+class OptimizerArguments(GeneralArguments):
     """Container Class for the arguments passed to the discopop_optimizer"""
 
     verbose: bool
     interactive: bool
-    exhaustive: bool
-    evolutionary: Optional[List[str]]
+    interactive_export: str
     doall_microbench_file: str
     reduction_microbench_file: str
     allow_nested_parallelism: bool
     plot: bool
     system_configuration_path: str
     check_called_function_for_nested_parallelism: bool
+    profiling: bool
+    pruning_level: int
+    optimization_level: int
+    optimization_level_2_parameters: str
+    single_suggestions: bool
+    pin_function_calls_to_host: bool
 
     def __post_init__(self):
-        # fix correct optimization method
-        if not self.exhaustive:
-            if self.evolutionary == None:
-                self.evolutionary = [str(50), str(5)]
-        elif self.evolutionary != None:
-            self.evolutionary = None
-
         self.__validate()
 
     def __validate(self):
         """Validate the arguments passed to the discopop_optimizer, e.g check if given files exist"""
-        if self.doall_microbench_file is not "None":
+        if self.doall_microbench_file != "None":
             if not os.path.isfile(self.doall_microbench_file):
                 raise FileNotFoundError(f"Microbenchmark file not found: {self.doall_microbench_file}")
-        if self.reduction_microbench_file is not "None":
+        if self.reduction_microbench_file != "None":
             if not os.path.isfile(self.reduction_microbench_file):
                 raise FileNotFoundError(f"Microbenchmark file not found: {self.reduction_microbench_file}")
+
+        # check pruning level values
+        if self.pruning_level not in [0, 1, 2]:
+            raise ValueError("Unsupported pruning level: ", self.pruning_level)
+
+        # check optimization level
+        if self.optimization_level not in [0, 1, 2, 3]:
+            raise ValueError("Unknown optimization level requested: ", self.optimization_level)
+
         pass
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/PETParser/DataAccesses/FromCUs.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/PETParser/DataAccesses/FromCUs.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/LoopInitializationUpdates.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/LoopInitializationUpdates.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/RemoveLoopIndexUpdates.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/RemoveSameDeviceUpdates.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,52 +2,35 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
-from typing import List, cast
-from discopop_explorer.PEGraphX import LoopNode
+from typing import List
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.classes.context.Update import Update
-from discopop_library.discopop_optimizer.classes.nodes.Loop import Loop
-from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 from discopop_library.result_classes.OptimizerOutputPattern import OptimizerOutputPattern
 
 
-def remove_loop_index_updates(
-    experiment: Experiment, best_configuration: OptimizerOutputPattern, arguments: OptimizerArguments
+def remove_same_device_updates(
+    experiment: Experiment, configuration: OptimizerOutputPattern, arguments: OptimizerArguments
 ) -> OptimizerOutputPattern:
-    to_be_removed: List[Update] = []
-    for update in best_configuration.data_movement:
-        # check for loop nodes as update targets
-        if type(data_at(experiment.optimization_graph, update.target_node_id)) == Loop:
-            # get loop indices from PEGraph
-            loop_cu_id = data_at(experiment.optimization_graph, update.target_node_id).original_cu_id
-            if loop_cu_id is None:
-                continue
-            loop_indices = cast(LoopNode, experiment.detection_result.pet.node_at(loop_cu_id)).loop_indices
-            # check for loop indices as targeted varbiables
-            if update.write_data_access.var_name in loop_indices:
-                # found update to loop index
-                if arguments.verbose:
-                    print("ignoring update: ", str(update), " , since it targets a loop index.")
-                to_be_removed.append(update)
-    # remove identified loop index updates
-    for tbr in to_be_removed:
-        if tbr in best_configuration.data_movement:
-            best_configuration.data_movement.remove(tbr)
+    """Remove updates where source and device id are equal. These are artifacts from initializing device memory states during the data movement calculation."""
+    cleaned_updates: List[Update] = []
+    for update in configuration.data_movement:
+        if (
+            update.source_device_id == update.target_device_id and not update.delete_data
+        ):  # delete updates can be issued with the same source and target device and need to be kept
+            # ignore this update
+            continue
+        else:
+            cleaned_updates.append(update)
+    configuration.data_movement = cleaned_updates
 
-    # ensure correct formatting
     if arguments.verbose:
-        if len(to_be_removed) > 0:
-            print()
-
-    if arguments.verbose:
-        print("Removed loop index updates")
-        for update in best_configuration.data_movement:
+        print("Removed same device updates")
+        for update in configuration.data_movement:
             print("# ", update)
         print()
-
-    return best_configuration
+    return configuration
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/UpdateOptimization/main.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/UpdateOptimization/main.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,58 +2,69 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
+import logging
 import os
 
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
+from discopop_library.discopop_optimizer.UpdateOptimization.AddRangesToUpdates import add_ranges_to_updates
 from discopop_library.discopop_optimizer.UpdateOptimization.LoopInitializationUpdates import (
     fix_loop_initialization_updates,
 )
 from discopop_library.discopop_optimizer.UpdateOptimization.RemoveDuplicatedUpdates import remove_duplicated_updates
 from discopop_library.discopop_optimizer.UpdateOptimization.RemoveLoopIndexUpdates import remove_loop_index_updates
+from discopop_library.discopop_optimizer.UpdateOptimization.RemoveSameDeviceUpdates import remove_same_device_updates
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.utilities.visualization.update_graph import show_update_graph
 from discopop_library.result_classes.OptimizerOutputPattern import OptimizerOutputPattern
 
 
 def optimize_updates(
-    experiment: Experiment, best_configuration: OptimizerOutputPattern, arguments: OptimizerArguments
+    experiment: Experiment, configuration: OptimizerOutputPattern, arguments: OptimizerArguments
 ) -> OptimizerOutputPattern:
+    logger = logging.getLogger("Optimizer").getChild("UpdateOptimization")
+    logger.setLevel(arguments.log_level)
     # plot raw update graph
     # show_update_graph(experiment.optimization_graph, best_configuration, experiment)
 
     # print original updates
     if arguments.verbose:
         print("Original updates")
-        for update in best_configuration.data_movement:
+        for update in configuration.data_movement:
             print("# ", update)
         print()
 
+    # remove same-device updates
+    configuration = remove_same_device_updates(experiment, configuration, arguments)
+
     # optimize updates
-    best_configuration = fix_loop_initialization_updates(experiment, best_configuration, arguments)
+    configuration = fix_loop_initialization_updates(experiment, configuration, arguments)
 
     # remove duplicated updates
-    best_configuration = remove_duplicated_updates(best_configuration, arguments)
+    configuration = remove_duplicated_updates(configuration, arguments)
 
     # remove loop index updates
-    best_configuration = remove_loop_index_updates(experiment, best_configuration, arguments)
+    # configuration = remove_loop_index_updates(experiment, configuration, arguments)
+
+    # add ranges to be transferred to the updates
+    configuration = add_ranges_to_updates(experiment, configuration, arguments)
 
     # plt optimized update graph
     # show_update_graph(experiment.optimization_graph, best_configuration, experiment)
 
     # print optimized updates
-    if arguments.verbose:
-        print("Optimized updates")
-        for update in best_configuration.data_movement:
-            print("# ", update)
-        print()
 
-    return best_configuration
+    logger.debug("Optimized updates")
+    for update in configuration.data_movement:
+        logger.debug("# " + str(update))
+    logger.debug("")
+
+    return configuration
 
 
 #    # export the updated configuration to the disk
 #    updated_configuration_path = os.path.join("optimizer", "updated_configuration.json")
 #    best_configuration.dump_to_file(updated_configuration_path)
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Variables/Experiment.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Variables/Experiment.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 from pathlib import Path
 from typing import Dict, Tuple, Set, Optional, List, Any
 
 import networkx as nx  # type: ignore
 from sympy import Integer, Symbol, Expr, Float  # type: ignore
 
 from discopop_explorer.PEGraphX import MemoryRegion
+from discopop_library.HostpotLoader.HotspotNodeType import HotspotNodeType
+from discopop_library.HostpotLoader.HotspotType import HotspotType
 from discopop_library.MemoryRegions.utils import get_sizes_of_memory_regions
 from discopop_library.PathManagement.PathManagement import load_file_mapping
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
 from discopop_library.discopop_optimizer.classes.context.ContextObject import ContextObject
 from discopop_library.discopop_optimizer.classes.enums.Distributions import FreeSymbolDistribution
 from discopop_library.discopop_optimizer.classes.nodes.FunctionRoot import FunctionRoot
@@ -68,22 +70,27 @@
     function_models: Dict[FunctionRoot, List[Tuple[CostModel, ContextObject, str]]]
     selected_paths_per_function: Dict[FunctionRoot, Tuple[CostModel, ContextObject]]
 
     optimization_graph: nx.DiGraph
     next_free_node_id: int
     suggestion_to_node_ids_dict: Dict[int, List[int]]
     node_id_to_suggestion_dict: Dict[int, int]
+    pattern_id_to_decisions_dict: Dict[int, List[int]]
+
+    hotspot_functions: Dict[HotspotType, List[Tuple[int, int, HotspotNodeType, str]]]
+    hotspot_function_node_ids: List[int]
 
     def __init__(
         self,
         file_mapping: Dict[int, Path],
         system: System,
         detection_result: DetectionResult,
         profiler_dir: str,
         arguments: OptimizerArguments,
+        hotspot_functions: Dict[HotspotType, List[Tuple[int, int, HotspotNodeType, str]]],
     ):
         self.__system = system
         self.detection_result = detection_result
         self.arguments = arguments
 
         self.__memory_region_sizes = get_sizes_of_memory_regions(
             set(),
@@ -92,14 +99,17 @@
         )
 
         self.file_mapping = file_mapping
         self.function_models = dict()
         self.selected_paths_per_function = dict()
         self.suggestion_to_node_ids_dict = dict()
         self.node_id_to_suggestion_dict = dict()
+        self.pattern_id_to_decisions_dict = dict()
+        self.hotspot_functions = hotspot_functions
+        self.hotspot_function_node_ids = []
 
         # collect free symbols from system
         for free_symbol, value_suggestion in system.get_free_symbols():
             self.register_free_symbol(free_symbol, value_suggestion)
 
     def get_memory_region_size(
         self, memory_region: MemoryRegion, use_symbolic_value: bool = False
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/Variables/ExperimentUtils.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/Variables/ExperimentUtils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/__main__.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/__main__.py`

 * *Files 27% similar despite different names*

```diff
@@ -2,76 +2,103 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 from argparse import ArgumentParser
+import logging
+from discopop_library.GlobalLogger.setup import setup_logger
 
 from discopop_library.discopop_optimizer.optimizer import run
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
 
 
 def parse_args() -> OptimizerArguments:
     """Parse the arguments passed to the discopop_optimizer"""
     parser = ArgumentParser(description="DiscoPoP Optimizer")
+    # all flags that belong to the interactive optimizer for pattern merging
+    interactive_parser = parser.add_argument_group(
+        "Interactive (Pattern merging)", "Arguments related to pattern merging."
+    )
     # all flags that are not considered stable should be added to the experimental_parser
     experimental_parser = parser.add_argument_group(
         "EXPERIMENTAL",
         "Arguments marked as experimental features. These flags may or may not be removed or changed in the future.",
     )
 
     # fmt: off
     parser.add_argument("-v", "--verbose", action="store_true",
         help="Enable verbose output.")
-    parser.add_argument("-x", "--exhaustive", action="store_true",
-        help="Enable exhaustive search. By default, an evolutionary search with a population size of 50 and 5 generations is performed.")
-    parser.add_argument("-e", "--evolutionary", type=str, default=None, nargs=2, metavar=("population_size", "generations"),
-        help="Enable evolutionary search. By default, an evolutionary search with a population size of 50 and 5 generations is performed.")
+    parser.add_argument("-p", type=int, default=0,
+        help="Program path pruning aggressiveness. 0: no pruning. 1: prune to paths that cover 80%% of observed decisions per path split. 2: prune to most likely path.")
+    parser.add_argument("-o", type=int, default=0, help="Optimization level: 0 -> no optimization. 1 -> greedy. 2 -> evolutionary. 3 -> exhaustive")
+
+    parser.add_argument("-opt-2-params", type=str, default=None, nargs=2, metavar=("population_size", "generations"), help="Configure parameters of the evolutionary optimization (-o2). Default: 50 5")
+    parser.add_argument("-s", "--single-suggestions", action="store_true", help="Enable the generation of individual suggestions for device mappings.")
+
     parser.add_argument(
         "--doall-microbench-file", type=str, default="None",
         help="Do-All microbenchmark results"
     )
     parser.add_argument(
         "--reduction-microbench-file", type=str, default="None",
         help="Reduction microbenchmark results"
     )
     parser.add_argument(
         "--system-configuration", type=str, default="optimizer/system_configuration.json",
         help="System configuration file"
     )
+    parser.add_argument("--profiling", action="store_true",
+        help="Enable profiling.")
+    parser.add_argument("--pin-function-calls-to-host", action="store_true", help="Force functions calls on the host system. Prevent offloading of entire functions.")
+    parser.add_argument("--log", type=str, default="WARNING", help="Specify log level: DEBUG, INFO, WARNING, ERROR, CRITICAL")
+    parser.add_argument("--write-log", action="store_true", help="Create Logfile.")
+    # INTERACTIVE (Merge) flags
+    interactive_parser.add_argument("-i", "--interactive", action="store_true",
+        help="Enable interactive pattern merge tool.")
+    interactive_parser.add_argument("--interactive-export", metavar="suggestion_ids", type=str, default="None", help="Merge and export the result for the comma-separated list of suggestion ids. Requires '-i' .")
     # EXPERIMENTAL FLAGS:
     experimental_parser.add_argument("--allow-nested-parallelism", action="store_true",
         help="Allow the creation of nested parallelism suggestions. "
         + "WARNING: Cost estimations may not be accurrate due to potentially"
         + "high overhead introduced by entering nested parallelism!")
     experimental_parser.add_argument("--check-called-function-for-nested-parallelism", action="store_true", help="Extend the check for nested parallelism to called functions."
         + "WARNING: Execution time may increase significantly!")
-    experimental_parser.add_argument("-i", "--interactive", action="store_true",
-        help="Enable interactive execution.")
+    
     experimental_parser.add_argument("--plot", action="store_true",
         help="Plot the internal graph.")
     # fmt: on
 
     arguments = parser.parse_args()
 
     return OptimizerArguments(
         verbose=arguments.verbose,
         interactive=arguments.interactive,
-        exhaustive=arguments.exhaustive,
-        evolutionary=arguments.evolutionary,
+        interactive_export=arguments.interactive_export,
         doall_microbench_file=arguments.doall_microbench_file,
         reduction_microbench_file=arguments.reduction_microbench_file,
         allow_nested_parallelism=arguments.allow_nested_parallelism,
         plot=arguments.plot,
         system_configuration_path=arguments.system_configuration,
         check_called_function_for_nested_parallelism=arguments.check_called_function_for_nested_parallelism,
+        profiling=arguments.profiling,
+        pruning_level=arguments.p,
+        optimization_level=arguments.o,
+        optimization_level_2_parameters=arguments.opt_2_params,
+        single_suggestions=arguments.single_suggestions,
+        log_level=arguments.log.upper(),
+        write_log=arguments.write_log,
+        pin_function_calls_to_host=arguments.pin_function_calls_to_host,
     )
 
 
 def main():
     arguments = parse_args()
+
+    setup_logger(arguments)
+
     run(arguments)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/bindings/utilities.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/bindings/utilities.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/ContextObject.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/ContextObject.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     def calculate_and_perform_necessary_updates(
         self,
         node_reads: Set[ReadDataAccess],
         reading_device_id: int,
         reading_node_id: int,
         graph: nx.DiGraph,
         experiment,
+        updates_originated_from: Optional[int] = None,
     ):
         """checks if the specified list of ReadDataAccesses performed by the specified device id makes updates
         necessary. If so, the updates will get append to the list of updates of the current ContextObject.
         The list of seen writes by device of the ContextObject will be updated to reflect the identified data transfers.
         A reference to the object is returned."""
         required_updates: Set[Update] = set()
         for read in node_reads:
@@ -61,14 +62,15 @@
 
                 if device_id == reading_device_id:
                     continue
 
                 if read.memory_region not in self.get_seen_writes_by_device(device_id):
                     # read memory region is currently "unknown" to the device, thus is can be skipped
                     continue
+
                 other_devices_known_writes = self.get_seen_writes_by_device(device_id)[read.memory_region]
 
                 is_first_data_occurrence = False
                 if read.memory_region not in self.get_seen_writes_by_device(reading_device_id):
                     # reading device does not currently "know" about the read memory region. create a new entry.
                     self.initialize_seen_writes_by_device(reading_device_id, read.memory_region)
                     is_first_data_occurrence = True
@@ -117,14 +119,15 @@
                                     target_node_id=reading_node_id,
                                     source_device_id=device_id,
                                     target_device_id=experiment.get_system().get_host_device_id(),  # reading_device_id,
                                     write_data_access=data_write,
                                     is_first_data_occurrence=is_first_data_occurrence,
                                     source_cu_id=data_at(graph, self.last_visited_node_id).original_cu_id,
                                     target_cu_id=data_at(graph, reading_node_id).original_cu_id,
+                                    originated_from_node=updates_originated_from,
                                 )
                             )
                         #                        else:
                         #                            print(
                         #                                "SKIPPED KNOWN WRITE: ",
                         #                                str(
                         #                                    Update(
@@ -145,14 +148,15 @@
                                 target_node_id=reading_node_id,
                                 source_device_id=0,  # device_id,
                                 target_device_id=reading_device_id,
                                 write_data_access=data_write,
                                 is_first_data_occurrence=is_first_data_occurrence,
                                 source_cu_id=data_at(graph, self.last_visited_node_id).original_cu_id,
                                 target_cu_id=data_at(graph, reading_node_id).original_cu_id,
+                                originated_from_node=updates_originated_from,
                             )
                         )
 
                     else:
                         # Host -> Device or Device -> Host update
                         required_updates.add(
                             Update(
@@ -160,14 +164,15 @@
                                 target_node_id=reading_node_id,
                                 source_device_id=device_id,
                                 target_device_id=reading_device_id,
                                 write_data_access=data_write,
                                 is_first_data_occurrence=is_first_data_occurrence,
                                 source_cu_id=data_at(graph, self.last_visited_node_id).original_cu_id,
                                 target_cu_id=data_at(graph, reading_node_id).original_cu_id,
+                                originated_from_node=updates_originated_from,
                             )
                         )
 
                 # todo: check if this is sufficient
                 for update in required_updates:
                     if update.write_data_access.memory_region not in self.get_seen_writes_by_device(
                         update.target_device_id
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/ContextObjectUtils.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/ContextObjectUtils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/context/Update.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/context/Update.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,55 +2,71 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import json
-from typing import Any, Dict, Optional, cast
+from typing import Any, Dict, Optional, Tuple, cast
 from discopop_explorer.PEGraphX import NodeID, PEGraphX
 from discopop_library.discopop_optimizer.classes.types.Aliases import DeviceID
 from discopop_library.discopop_optimizer.classes.types.DataAccessType import (
+    ReadDataAccess,
     WriteDataAccess,
     write_data_access_from_dict,
 )
 
 
 class Update(object):
     source_node_id: int
     target_node_id: int
+    originated_from_node: Optional[int]  # used in case the update is moved to the nearest DeviceSwitch node
     source_device_id: DeviceID
     target_device_id: DeviceID
     write_data_access: WriteDataAccess
     is_first_data_occurrence: bool
     source_cu_id: Optional[NodeID]
     target_cu_id: Optional[NodeID]
+    range: Optional[Tuple[int, int]]
+    delete_data: bool  # i.e. exit data map(delete: a)
+    copy_delete_data: bool  # i.e. exit data map(from: a)
 
     def __init__(
         self,
         source_node_id: int,
         target_node_id: int,
         source_device_id: DeviceID,
         target_device_id: DeviceID,
         write_data_access: WriteDataAccess,
         is_first_data_occurrence: bool,
         source_cu_id: Optional[NodeID],
         target_cu_id: Optional[NodeID],
+        originated_from_node: Optional[int] = None,
+        range: Optional[Tuple[int, int]] = None,
+        delete_data: bool = False,
+        copy_delete_data: bool = False,
     ):
         self.source_node_id = source_node_id
         self.target_node_id = target_node_id
         self.source_device_id = source_device_id
         self.target_device_id = target_device_id
         self.write_data_access = write_data_access
         self.is_first_data_occurrence = is_first_data_occurrence
         self.source_cu_id = source_cu_id
         self.target_cu_id = target_cu_id
+        self.originated_from_node = originated_from_node
+        self.range = range
+        self.delete_data = delete_data
+        self.copy_delete_data = copy_delete_data
 
     def __str__(self):
-        result_str = "First" if self.is_first_data_occurrence else ""
+        result_str = ""
+        result_str += "IssueCopyDelete " if self.copy_delete_data else ""
+        result_str += "IssueDelete " if self.delete_data else ""
+        result_str += "First" if self.is_first_data_occurrence else ""
         return (
             result_str
             + "Update("
             + str(self.source_node_id)
             + "@"
             + str(self.source_device_id)
             + ", "
@@ -71,34 +87,43 @@
         result_dict["target_device_id"] = self.target_device_id
         result_dict["openmp_source_device_id"] = self.source_device_id
         result_dict["openmp_target_device_id"] = self.target_device_id
         result_dict["is_first_data_occurrence"] = self.is_first_data_occurrence
         result_dict["var_name"] = self.write_data_access.var_name
         result_dict["start_line"] = pet.node_at(cast(NodeID, self.source_cu_id)).start_position()
         result_dict["end_line"] = pet.node_at(cast(NodeID, self.target_cu_id)).start_position()
+        result_dict["range"] = self.range
+        result_dict["delete_data"] = self.delete_data
+        result_dict["copy_delete_data"] = self.copy_delete_data
         return json.dumps(result_dict)
 
     def toDict(self) -> Dict[str, Any]:
         result_dict: Dict[str, Any] = {}
         result_dict["source_node_id"] = self.source_node_id
         result_dict["target_node_id"] = self.target_node_id
         result_dict["source_device_id"] = self.source_device_id
         result_dict["target_device_id"] = self.target_device_id
         result_dict["is_first_data_occurrence"] = self.is_first_data_occurrence
         result_dict["write_data_access"] = self.write_data_access.toDict()
         result_dict["source_cu_id"] = self.source_cu_id
         result_dict["target_cu_id"] = self.target_cu_id
+        result_dict["range"] = self.range
+        result_dict["delete_data"] = self.delete_data
+        result_dict["copy_delete_data"] = self.copy_delete_data
         return result_dict
 
 
 def construct_update_from_dict(values: Dict[str, Any]) -> Update:
     update = Update(
         values["source_node_id"],
         values["target_node_id"],
         values["source_device_id"],
         values["target_device_id"],
         write_data_access_from_dict(values["write_data_access"]),
         values["is_first_data_occurrence"],
         values["source_cu_id"],
         values["target_cu_id"],
+        range=values["range"],
+        delete_data=values["delete_data"],
+        copy_delete_data=values["copy_delete_data"],
     )
     return update
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/DataFlowEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/DataFlowEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/GenericEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/GenericEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/MutuallyExclusiveEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/MutuallyExclusiveEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/OptionEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/OptionEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/RequirementEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/RequirementEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/SuccessorEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/SuccessorEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/edges/TemporaryEdge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/edges/TemporaryEdge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextMerge.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextMerge.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextNode.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextNode.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextRestore.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextRestore.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextSave.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextSave.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshot.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshot.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshotPop.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/ContextSnapshotPop.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/FunctionRoot.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/FunctionRoot.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/GenericNode.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/GenericNode.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/Loop.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/Loop.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/nodes/Workload.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/nodes/Workload.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/Network.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/Network.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,23 +26,27 @@
     def add_connection(self, source: Device, target: Device, transfer_speed: Expr, initialization_delay: Expr):
         if source == target:
             transfer_speed = Integer(10000 * 1000)  # 10000 GB/s = 10000 * 1000 MB/s
         self.__transfer_speeds[(source, target)] = transfer_speed
         self.__transfer_initialization_costs[(source, target)] = initialization_delay
 
     def get_transfer_speed(self, source: Device, target: Device):
+        if source == target:
+            return Integer(1000000)  # 1000 GB/s
         if (source, target) not in self.__transfer_speeds:
             if self.__host_device is None:
                 raise ValueError("Host device of network unspecified!")
             S_to_H_speed = self.__transfer_speeds[(source, self.__host_device)]
             H_to_T_speed = self.__transfer_speeds[(self.__host_device, target)]
             return min(S_to_H_speed, H_to_T_speed)
         return self.__transfer_speeds[(source, target)]
 
     def get_transfer_initialization_costs(self, source: Device, target: Device):
+        if source == target:
+            return Integer(0)
         if (source, target) not in self.__transfer_speeds:
             if self.__host_device is None:
                 raise ValueError("Host device of network unspecified!")
             S_to_H_init_costs = self.__transfer_initialization_costs[(source, self.__host_device)]
             H_to_T_init_costs = self.__transfer_initialization_costs[(self.__host_device, target)]
             return S_to_H_init_costs + H_to_T_init_costs
         return self.__transfer_initialization_costs[(source, target)]
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/System.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/System.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 class System(object):
     __devices: Dict[int, Device]
     __host_device_id: int
     __network: Network
     __device_do_all_overhead_models: Dict[Device, Expr]
+    __device_do_all_shared_overhead_models: Dict[Device, Expr]
     __device_reduction_overhead_models: Dict[Device, Expr]
     __symbol_substitutions: List[
         Tuple[
             Symbol,
             Optional[float],
             Optional[float],
             Optional[float],
@@ -39,14 +40,15 @@
     ]
 
     def __init__(self, arguments: OptimizerArguments):
         self.__devices = dict()
         self.__host_device_id = -1
         self.__network = Network()
         self.__device_do_all_overhead_models = dict()
+        self.__device_do_all_shared_overhead_models = dict()
         self.__device_reduction_overhead_models = dict()
         self.__symbol_substitutions = []
 
         self.__build_from_configuration_file(arguments)
 
     # todo: support the replication of device ids (e.g. CPU-0 and GPU-0)
 
@@ -87,43 +89,59 @@
 
     def __build_CPU(self, device_configuration: Dict[str, Any]):
         cpu = CPU(
             frequency=Integer(device_configuration["frequency"]),
             thread_count=Integer(device_configuration["threads"]),
             openmp_device_id=device_configuration["device_id"],
             device_specific_compiler_flags="",
+            speedup=device_configuration["speedup"],
+            compute_init_delays=device_configuration["compute_init_delays[us]"],
         )
         self.add_device(cpu, device_configuration["device_id"])
 
     def __build_GPU(self, device_configuration: Dict[str, Any]):
         gpu = GPU(
             frequency=Integer(device_configuration["frequency"]),
             thread_count=Integer(device_configuration["threads"]),
             openmp_device_id=device_configuration["device_id"],
             device_specific_compiler_flags="",
+            speedup=device_configuration["speedup"],
+            compute_init_delays=device_configuration["compute_init_delays[us]"],
         )
         self.add_device(gpu, device_configuration["device_id"])
 
     def set_device_doall_overhead_model(self, device: Device, model: Expr, arguments: OptimizerArguments):
         if arguments.verbose:
             print("System: Set DOALL overhead model: ", model)
         self.__device_do_all_overhead_models[device] = model
 
+    def set_device_doall_shared_overhead_model(self, device: Device, model: Expr, arguments: OptimizerArguments):
+        if arguments.verbose:
+            print("System: Set DOALL SHARED overhead model: ", model)
+        self.__device_do_all_shared_overhead_models[device] = model
+
     def set_reduction_overhead_model(self, device: Device, model: Expr, arguments: OptimizerArguments):
         if arguments.verbose:
             print("System: Set REDUCTION overhead model: ", model)
         self.__device_reduction_overhead_models[device] = model
 
     def get_device_doall_overhead_model(self, device: Device, arguments: OptimizerArguments) -> Expr:
         if device not in self.__device_do_all_overhead_models:
             if arguments.verbose:
                 warnings.warn("No DOALL overhead model, assuming 0 for device: " + str(device))
             return Expr(Integer(0))
         return self.__device_do_all_overhead_models[device]
 
+    def get_device_doall_shared_overhead_model(self, device: Device, arguments: OptimizerArguments) -> Expr:
+        if device not in self.__device_do_all_shared_overhead_models:
+            if arguments.verbose:
+                warnings.warn("No DOALL SHARED overhead model, assuming 0 for device: " + str(device))
+            return Expr(Integer(0))
+        return self.__device_do_all_shared_overhead_models[device]
+
     def get_device_reduction_overhead_model(self, device: Device, arguments: OptimizerArguments) -> Expr:
         if device not in self.__device_reduction_overhead_models:
             if arguments.verbose:
                 warnings.warn("No REDUCTION overhead model, assuming 0 for device: " + str(device))
             return Expr(Integer(0))
         return self.__device_reduction_overhead_models[device]
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/CPU.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/CPU.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
+from typing import Dict
 from discopop_library.discopop_optimizer.classes.system.devices.Device import Device
 from discopop_library.discopop_optimizer.classes.system.devices.DeviceTypeEnum import DeviceTypeEnum
 
 
 class CPU(Device):
     def __init__(
         self,
         frequency,
         thread_count,
         openmp_device_id: int,
         device_specific_compiler_flags: str,
+        speedup: float,
+        compute_init_delays: Dict[str, float],
     ):
-        super().__init__(frequency, thread_count, openmp_device_id, device_specific_compiler_flags)
+        super().__init__(
+            frequency, thread_count, openmp_device_id, device_specific_compiler_flags, speedup, compute_init_delays
+        )
 
     def get_device_type(self) -> DeviceTypeEnum:
         return DeviceTypeEnum.CPU
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/Device.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/Device.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,57 +1,69 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
-from typing import Tuple, List, Optional, cast
+from typing import Dict, Tuple, List, Optional, cast
 
-from sympy import Expr, Symbol
+from sympy import Expr, Float, Symbol
 from sympy import Integer
 
 from discopop_explorer.pattern_detectors.PatternInfo import PatternInfo
 from discopop_library.discopop_optimizer.classes.system.devices.DeviceTypeEnum import DeviceTypeEnum
 
 
 class Device(object):
     __frequency: Expr
     __thread_count: Expr
     openmp_device_id: int
+    __speedup: float  # comapred to sequential execution
+    __compute_init_delays: Dict[str, float]
 
     def __init__(
         self,
         frequency: Expr,  # GHz
         thread_count: Expr,
         openmp_device_id: int,
         device_specific_compiler_flags: str,
+        speedup: float,
+        compute_init_delays: Dict[str, float],
     ):
         self.__frequency = frequency
         self.__thread_count = thread_count
         self.openmp_device_id = openmp_device_id
         self.device_specific_compiler_flags: str = device_specific_compiler_flags
+        self.__speedup = speedup
+        self.__compute_init_delays = compute_init_delays
 
     def get_device_specific_pattern_info(
         self, suggestion: PatternInfo, suggestion_type: str
     ) -> Tuple[PatternInfo, str]:
         return suggestion, suggestion_type
 
+    def get_compute_init_delays(self) -> Dict[str, float]:
+        return self.__compute_init_delays
+
     def get_compute_capability(self) -> Expr:
         return self.__frequency
 
     def get_thread_count(self) -> Expr:
         return self.__thread_count
 
     def get_free_symbols(self) -> List[Tuple[Symbol, Optional[Expr]]]:
         result_list: List[Tuple[Symbol, Optional[Expr]]] = []
         result_list += [(cast(Symbol, s), None) for s in self.__frequency.free_symbols]
         result_list += [(cast(Symbol, s), None) for s in self.__thread_count.free_symbols]
         return result_list
 
+    def get_measured_speedup(self) -> Expr:
+        return Float(self.__speedup)
+
     def get_estimated_execution_time_in_micro_seconds(self, workload: Expr, is_sequential: bool):
         """execution time is estimated by:
         - convert workload to estimated amount of CPU instructions using a extra-p model
         - NOTE: use "perf stat ./<cmd" to get the amount of instructions and instructions per cycle
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/devices/GPU.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/devices/GPU.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,34 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
-from typing import Tuple
+from typing import Dict, Tuple
 
 from discopop_explorer.pattern_detectors.PatternInfo import PatternInfo
 from discopop_library.discopop_optimizer.classes.system.devices.Device import Device
 from discopop_library.discopop_optimizer.classes.system.devices.DeviceTypeEnum import DeviceTypeEnum
 
 
 class GPU(Device):
-    def __init__(self, frequency, thread_count, openmp_device_id, device_specific_compiler_flags):
-        super().__init__(frequency, thread_count, openmp_device_id, device_specific_compiler_flags)
+    def __init__(
+        self,
+        frequency,
+        thread_count,
+        openmp_device_id,
+        device_specific_compiler_flags,
+        speedup: float,
+        compute_init_delays: Dict[str, float],
+    ):
+        super().__init__(
+            frequency, thread_count, openmp_device_id, device_specific_compiler_flags, speedup, compute_init_delays
+        )
 
     def get_device_specific_pattern_info(
         self, suggestion: PatternInfo, suggestion_type: str
     ) -> Tuple[PatternInfo, str]:
         return suggestion, "gpu_" + suggestion_type
 
     def get_device_type(self) -> DeviceTypeEnum:
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/system/system_utils.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/system/system_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,48 +27,52 @@
     # configure host device
     host_device: Dict[str, Union[float, int, Dict[str, float]]] = {
         "device_id": 0,
         "device_type": DeviceTypeEnum.CPU,
         "frequency": 3000000000,
         "processors": 16,
         "threads": 16,
+        "speedup": 9.5,
+        "compute_init_delays[us]": {"doall": 300},
     }
     # configure gpu_1
     gpu_1: Dict[str, Union[float, int, Dict[str, float]]] = {
-        "compute_init_delays": {"target_teams_distribute_parallel_for": 0.01},
+        "compute_init_delays[us]": {"target_teams_distribute_parallel_for": 1000},
         "device_id": 1,
         "device_type": DeviceTypeEnum.GPU,
         "frequency": 256000000,
         "processors": 128,
         "teams": 3200,
         "threads": 3200,
         "transfer_init_delays[us]": {
             "target_data_update": 350,
             "target_enter_data": 900,
             "target_exit_data": 40,
             "average": 730,
         },
         "transfer_speeds": {"D2H_MB/s": 1800, "H2D_MB/s": 3600},  # MB/s
+        "speedup": 160.32,
     }
     # configure gpu_2
     gpu_2: Dict[str, Union[float, int, Dict[str, float]]] = {
-        "compute_init_delays": {"target_teams_distribute_parallel_for": 0.005},
+        "compute_init_delays[us]": {"target_teams_distribute_parallel_for": 5000},
         "device_id": 2,
         "device_type": DeviceTypeEnum.GPU,
-        "frequency": 256000000,
+        "frequency": 128000000,
         "processors": 128,
         "teams": 3200,
         "threads": 3200,
         "transfer_init_delays[us]": {
             "target_data_update": 710,
             "target_enter_data": 900,
             "target_exit_data": 50,
             "average": 810,
         },
         "transfer_speeds": {"D2H_MB/s": 1900, "H2D_MB/s": 4200},  # MB/s
+        "speedup": 105.58,
     }
     # assemble system_configuration
     devices = [host_device, gpu_1, gpu_2]
     system_configuration["devices"] = devices
     system_configuration["host_device"] = host_device["device_id"]
 
     # output to file
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/classes/types/DataAccessType.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/classes/types/DataAccessType.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,42 +9,53 @@
 
 from discopop_explorer.PEGraphX import MemoryRegion
 
 
 class ReadDataAccess(object):
     memory_region: MemoryRegion
     var_name: Optional[str]
+    from_call: bool
 
-    def __init__(self, memory_region: MemoryRegion, var_name: Optional[str]):
+    def __init__(self, memory_region: MemoryRegion, var_name: Optional[str], from_call: bool = False):
         self.memory_region = memory_region
         self.var_name = var_name
+        self.from_call = from_call
 
     def __str__(self):
-        return "R(" + self.memory_region + ")"
+        return_str = ""
+        return_str += "C" if self.from_call else ""
+        return_str += "R(" + self.memory_region + ")"
+        return return_str
 
 
 class WriteDataAccess(object):
     memory_region: MemoryRegion
     unique_id: int
     var_name: Optional[str]
+    from_call: bool
 
-    def __init__(self, memory_region: MemoryRegion, unique_id: int, var_name: Optional[str]):
+    def __init__(self, memory_region: MemoryRegion, unique_id: int, var_name: Optional[str], from_call: bool = False):
         self.memory_region = memory_region
         self.unique_id = unique_id
         self.var_name = var_name
+        self.from_call = from_call
 
     def __str__(self):
-        return "W(" + self.memory_region + "-" + str(self.unique_id) + ", --> " + self.var_name + ")"
+        return_str = ""
+        return_str += "C" if self.from_call else ""
+        return_str += "W(" + self.memory_region + "-" + str(self.unique_id) + ", --> " + self.var_name + ")"
+        return return_str
 
     def __hash__(self):
         return self.unique_id
 
     def toDict(self):
         result_dict = {}
         result_dict["memory_region"] = self.memory_region
         result_dict["unique_id"] = self.unique_id
         result_dict["var_name"] = self.var_name
+        result_dict["from_call"] = self.from_call
         return result_dict
 
 
 def write_data_access_from_dict(values: Dict[str, Any]) -> WriteDataAccess:
-    return WriteDataAccess(values["memory_region"], values["unique_id"], values["var_name"])
+    return WriteDataAccess(values["memory_region"], values["unique_id"], values["var_name"], values["from_call"])
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/gui/plotting/CostModels.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/gui/plotting/CostModels.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/gui/presentation/ChoiceDetails.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/gui/presentation/ChoiceDetails.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/gui/presentation/OptionTable.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/gui/presentation/OptionTable.py`

 * *Files 2% similar despite different names*

```diff
@@ -208,20 +208,20 @@
                 pet, graph, experiment, opt, ctx, opt_name, function_root
             ),
         )
         export_code_button.grid(row=0, column=2)
 
         def __update_selection(cm, ctx):
             experiment.selected_paths_per_function[function_root] = (cm, ctx)
-            experiment.substitutions[
-                cast(Symbol, function_root.sequential_costs)
-            ] = experiment.selected_paths_per_function[function_root][0].sequential_costs
-            experiment.substitutions[
-                cast(Symbol, function_root.parallelizable_costs)
-            ] = experiment.selected_paths_per_function[function_root][0].parallelizable_costs
+            experiment.substitutions[cast(Symbol, function_root.sequential_costs)] = (
+                experiment.selected_paths_per_function[function_root][0].sequential_costs
+            )
+            experiment.substitutions[cast(Symbol, function_root.parallelizable_costs)] = (
+                experiment.selected_paths_per_function[function_root][0].parallelizable_costs
+            )
             # update displayed value
             label2.configure(state=NORMAL)
             label2.delete(0, END)
             label2.insert(0, str(cm.path_decisions))
             label2.configure(state=DISABLED)
 
         update_selection_button = Button(
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/gui/queries/ValueTableQuery.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/gui/queries/ValueTableQuery.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/gui/widgets/ScrollableFrame.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/gui/widgets/ScrollableFrame.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/optimization/evaluate.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/optimization/evaluate.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.CostModels.DataTransfer.DataTransferCosts import add_data_transfer_costs
 from discopop_library.discopop_optimizer.CostModels.utilities import (
     get_node_performance_models,
     get_performance_models_for_functions,
 )
 from discopop_library.discopop_optimizer.DataTransfers.DataTransfers import calculate_data_transfers
+from discopop_library.discopop_optimizer.DataTransfers.NewDataTransfers import calculate_data_transfers_by_models
 
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.classes.context.ContextObject import ContextObject
 from discopop_library.discopop_optimizer.classes.nodes.FunctionRoot import FunctionRoot
 from discopop_library.discopop_optimizer.utilities.MOGUtilities import get_all_function_nodes, show
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
@@ -47,16 +48,15 @@
             main_function = cast(FunctionRoot, data_at(experiment.optimization_graph, function_id))
     if main_function is None:
         raise ValueError("No main function found!")
 
     function_performance_models_without_context = get_performance_models_for_functions(
         experiment, experiment.optimization_graph, restrict_to_decisions=set(decisions)
     )
-
-    function_performance_models = calculate_data_transfers(
+    function_performance_models = calculate_data_transfers_by_models(
         experiment.optimization_graph, function_performance_models_without_context, experiment
     )
     function_performance_models = add_data_transfer_costs(
         experiment.optimization_graph,
         function_performance_models,
         experiment,
     )
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/optimization/evaluate_all_decision_combinations.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/optimization/evaluate_all_decision_combinations.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,15 @@
                     if best_configuration is None:
                         best_configuration = OptimizerOutputPattern(
                             experiment.detection_result.pet.node_at(
                                 cast(NodeID, data_at(experiment.optimization_graph, node_id).original_cu_id)
                             ),
                             [],
                             experiment.get_system().get_host_device_id(),
+                            experiment,
                         )
                     best_configuration.add_pattern(
                         pattern_id, device_id, experiment.get_system().get_device(device_id).get_device_type()
                     )
         if best_configuration is None:
             return None
         # collect data movement information
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/optimization/evolutionary_algorithm.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/optimization/evolutionary_algorithm.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,19 +38,19 @@
 
 def perform_evolutionary_search(
     experiment: Experiment,
     available_decisions: Dict[FunctionRoot, List[List[int]]],
     arguments: OptimizerArguments,
     optimizer_dir: str,
 ) -> Optional[OptimizerOutputPattern]:
-    if arguments.evolutionary is None:
-        raise ValueError("Invalid arguments for evolutionary search: " + str(arguments.evolutionary))
+    if arguments.optimization_level_2_parameters is None:
+        arguments.optimization_level_2_parameters = ["50", "5"]
     ### SETTINGS
-    population_size = int(arguments.evolutionary[0])
-    generations = int(arguments.evolutionary[1])
+    population_size = int(arguments.optimization_level_2_parameters[0])
+    generations = int(arguments.optimization_level_2_parameters[1])
     selection_strength = 0.85  # 0.8 --> 80% of the population will be selected for the next generation
     crossovers = int(population_size / 10)
     mutations = int(population_size / 10)
     ### END SETTINGS
 
     population: List[List[int]] = __initialize(experiment, population_size, available_decisions, arguments)
     population, fitness, _ = __calculate_fitness(experiment, population, arguments)
@@ -315,14 +315,17 @@
 
     for i in range(0, 1000):
         # select two random elements
         element_1 = random.choice(global_population)
         element_2 = random.choice(global_population)
         # select crossover point
         max_crossover_idx = min(len(element_1), len(element_2))
+        if max_crossover_idx == 0:
+            # prevent index errors
+            continue
         crossover_idx = random.choice(range(0, max_crossover_idx))
 
         new_element_1 = element_1[:crossover_idx] + element_2[crossover_idx:]
         new_element_2 = element_2[:crossover_idx] + element_1[crossover_idx:]
 
         # validate elements
         if not check_configuration_validity(global_experiment, global_arguments, new_element_1):
@@ -377,14 +380,17 @@
     global global_population
 
     for i in range(0, 1000):
         # select random mutation target from population
         mutation_target = random.choice(global_population)
 
         # select random mutation within the target
+        if len(mutation_target) == 0:
+            # prevent index errors
+            continue
         mutation_index = random.choice(range(0, len(mutation_target)))
 
         # perform mutation if possible
         options = get_out_mutex_edges(global_experiment.optimization_graph, mutation_target[mutation_index])
         if len(options) > 0:
             index_mutant = random.choice(options)
             mutant = copy.deepcopy(mutation_target)
@@ -438,14 +444,15 @@
                     if best_configuration is None:
                         best_configuration = OptimizerOutputPattern(
                             experiment.detection_result.pet.node_at(
                                 cast(NodeID, data_at(experiment.optimization_graph, node_id).original_cu_id)
                             ),
                             [],
                             experiment.get_system().get_host_device_id(),
+                            experiment,
                         )
                     best_configuration.add_pattern(
                         pattern_id, device_id, experiment.get_system().get_device(device_id).get_device_type()
                     )
         if best_configuration is None:
             return None
         # collect data movement information
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/optimization/validation.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/optimization/validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 
 
 def check_configuration_validity(
     experiment: Experiment, arguments: OptimizerArguments, configuration: List[int]
 ) -> bool:
     """Returns True if the given configuration is valid. Returns False otherwise."""
-
     # check requirements edges
     for node_id in configuration:
         requirements = get_requirements(experiment.optimization_graph, node_id)
         for r in requirements:
             if r not in configuration:
                 # requirement not satisfied
                 return False
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/optimizer.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/optimizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,42 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
+import cProfile
 import json
+import logging
 import os.path
+import pstats
 import shutil
 from typing import Dict, List, Tuple, cast
 import warnings
 
 import jsonpickle  # type: ignore
 from sympy import Float, Symbol  # type: ignore
 
 from discopop_library.CodeGenerator.CodeGenerator import from_json_strings
+from discopop_library.HostpotLoader.HotspotLoaderArguments import HotspotLoaderArguments
 from discopop_library.JSONHandler.JSONHandler import read_patterns_from_json_to_json
 from discopop_library.PatchGenerator.PatchGeneratorArguments import PatchGeneratorArguments
 from discopop_library.PatchGenerator.diffs import get_diffs_from_modified_code
 from discopop_library.PathManagement.PathManagement import load_file_mapping
 from discopop_library.discopop_optimizer.CostModels.DataTransfer.DataTransferCosts import add_data_transfer_costs
 from discopop_library.discopop_optimizer.CostModels.utilities import get_performance_models_for_functions
-from discopop_library.discopop_optimizer.DataTransfers.DataTransfers import calculate_data_transfers
+from discopop_library.discopop_optimizer.DataTransfers.NewDataTransfers import new_calculate_data_transfers
+from discopop_library.discopop_optimizer.DataTransfers.calculate_configuration_data_movement import (
+    calculate_data_movement,
+)
+from discopop_library.discopop_optimizer.DataTransfers.prepare_force_branch_end_data_movement import (
+    prepare_force_branch_end_data_movement,
+)
+from discopop_library.discopop_optimizer.DataTransfers.prepare_forced_data_movement import prepare_forced_data_movement
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
 from discopop_library.discopop_optimizer.PETParser.PETParser import PETParser
 from discopop_library.discopop_optimizer.UpdateOptimization.main import optimize_updates
 from discopop_library.discopop_optimizer.Variables.ExperimentUtils import (
     create_optimization_graph,
     export_detection_result_to_json,
     export_patterns_to_json,
@@ -33,20 +44,23 @@
     get_sequential_cost_model,
     initialize_free_symbol_ranges_and_distributions,
 )
 from discopop_library.discopop_optimizer.classes.enums.Distributions import FreeSymbolDistribution
 from discopop_library.discopop_optimizer.classes.nodes.FunctionRoot import FunctionRoot
 from discopop_library.discopop_optimizer.classes.system.system_utils import generate_default_system_configuration
 from discopop_library.discopop_optimizer.gui.queries.ValueTableQuery import query_user_for_symbol_values
+from discopop_library.discopop_optimizer.interactive.interactive_optimizer import run_interactive_optimizer
 from discopop_library.discopop_optimizer.optimization.evaluate import evaluate_configuration
 from discopop_library.discopop_optimizer.optimization.evaluate_all_decision_combinations import (
     evaluate_all_decision_combinations,
 )
 from discopop_library.discopop_optimizer.optimization.evolutionary_algorithm import perform_evolutionary_search
+from discopop_library.discopop_optimizer.optimization.greedy import greedy_search
 from discopop_library.discopop_optimizer.suggestions.optimizers.main import optimize_suggestions
+from discopop_library.discopop_optimizer.utilities.insert_device_switch_nodes import insert_device_switch_nodes
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 from discopop_library.discopop_optimizer.utilities.visualization.update_graph import show_update_graph
 from discopop_library.global_data.version.utils import get_version
 from discopop_library.result_classes.DetectionResult import DetectionResult
 from discopop_library.discopop_optimizer.classes.system.System import System
 from discopop_library.discopop_optimizer.Microbench.ExtrapInterpolatedMicrobench import (
     ExtrapInterpolatedMicrobench,
@@ -55,16 +69,27 @@
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.utilities.MOGUtilities import (
     get_available_decisions_for_functions,
     show,
 )
 from discopop_library.discopop_optimizer.suggestions.importers.main import import_suggestions
 
+from ..HostpotLoader.hostpot_loader import run as load_hotspots
+
 
 def run(arguments: OptimizerArguments):
+    if arguments.interactive:
+        run_interactive_optimizer(arguments)
+    else:
+        run_passive_optimizer(arguments)
+
+
+def run_passive_optimizer(arguments: OptimizerArguments):
+    logger = logging.getLogger("Optimizer")
+
     # check prerequisites and setup folder structure
     if arguments.verbose:
         print("Started DiscoPoP Optimizer...")
         print("Creating optimizer directory...")
     optimizer_dir = os.path.join(os.getcwd(), "optimizer")
     if not os.path.exists(optimizer_dir):
         os.mkdir(optimizer_dir)
@@ -92,14 +117,32 @@
     if arguments.verbose:
         print("Loading file mapping...", end="")
     file_mapping = load_file_mapping(file_mapping_path)
     if arguments.verbose:
         print("Done.")
 
     if arguments.verbose:
+        print("Loading Hotspots...")
+    hotspot_functions = load_hotspots(
+        HotspotLoaderArguments(
+            verbose=arguments.verbose,
+            get_loops=False,
+            get_functions=True,
+            get_YES=True,
+            get_MAYBE=False,
+            get_NO=False,
+            log_level=arguments.log_level,
+            write_log=arguments.write_log,
+        )
+    )
+
+    if arguments.verbose:
+        print("Done.")
+
+    if arguments.verbose:
         print("Loading patterns...", end="")
     patterns_by_type = read_patterns_from_json_to_json(pattern_file_path, [])
     if arguments.verbose:
         print("Done.")
 
     if arguments.verbose:
         print("Loading detection result and PET...", end="")
@@ -131,44 +174,65 @@
     # todo check if OpenMP allows direct data transfers between devices
 
     # load overhead measurements into system if existent
     if arguments.doall_microbench_file != "None":
         # construct and set overhead model for doall suggestions
         system.set_device_doall_overhead_model(
             system.get_device(system.get_host_device_id()),
-            ExtrapInterpolatedMicrobench(arguments.doall_microbench_file).getFunctionSympy(),
+            ExtrapInterpolatedMicrobench(arguments.doall_microbench_file).getFunctionSympy(
+                benchType=MicrobenchType.DOALL
+            ),
             arguments,
         )
+        # construct and set overhead model for doall suggestions with shaed clause
+        system.set_device_doall_shared_overhead_model(
+            system.get_device(system.get_host_device_id()),
+            ExtrapInterpolatedMicrobench(arguments.doall_microbench_file).getFunctionSympy(
+                benchType=MicrobenchType.SHARED
+            ),
+            arguments,
+        )
+
     if arguments.reduction_microbench_file != "None":
         # construct and set overhead model for reduction suggestions
         system.set_reduction_overhead_model(
             system.get_device(system.get_host_device_id()),
             ExtrapInterpolatedMicrobench(arguments.reduction_microbench_file).getFunctionSympy(
                 benchType=MicrobenchType.FOR
             ),
             arguments,
         )
 
     # define Experiment
-    experiment = Experiment(file_mapping, system, detection_result, profiler_dir, arguments)
+    experiment = Experiment(file_mapping, system, detection_result, profiler_dir, arguments, hotspot_functions)
+
+    if arguments.profiling:
+        experiment.profile = cProfile.Profile()  # type: ignore
+        experiment.profile.enable()  # type: ignore
 
     # build optimization graph
     if arguments.verbose:
         print("Creating optimization graph...")
     create_optimization_graph(experiment, arguments)
 
+    # prepare forcing of data movement at branch end
+    experiment.optimization_graph = prepare_forced_data_movement(experiment)
+
     if arguments.verbose:
         print("Done.")
     # import parallelization suggestions
     experiment.optimization_graph = import_suggestions(experiment)
     # optimize parallelization suggestions
     experiment.optimization_graph = optimize_suggestions(experiment)
 
+    # insert device switch nodes
+    # experiment.optimization_graph = insert_device_switch_nodes(experiment)
+
     if arguments.plot:
-        show(experiment.optimization_graph, show_dataflow=False, show_mutex_edges=False)
+        show(experiment.optimization_graph, show_dataflow=True, show_mutex_edges=False)
 
     if arguments.verbose:
         print("# SUGGESTION ID -> NODE ID MAPPING")
         for suggestion_id in experiment.suggestion_to_node_ids_dict:
             print("#", suggestion_id, "->", experiment.suggestion_to_node_ids_dict[suggestion_id])
         print()
 
@@ -183,37 +247,65 @@
 
     if arguments.verbose:
         print("# SUBSTITUTIONS:")
         for key in experiment.substitutions:
             print("#", key, " ->", experiment.substitutions[key])
         print()
 
-    # calculate options for easy access
-    available_decisions = get_available_decisions_for_functions(experiment.optimization_graph, arguments)
+    # calculate necessary updates for all created (i.e. mapped or collapsed) suggestions
+    # this can get quite expensive for large software, so it should only be calculated upon request
+    if arguments.single_suggestions:
+        calculate_data_movement(experiment)
+
+    # apply optimization steps if requested
+    best_configuration = None
+    if arguments.optimization_level != 0:
+        # calculate options for easy access
+        available_decisions = get_available_decisions_for_functions(experiment.optimization_graph, arguments)
+
+        if arguments.optimization_level == 1:
+            best_configuration = greedy_search(experiment, available_decisions, arguments, optimizer_dir)
+        elif arguments.optimization_level == 2:
+            # perform evolutionary search
+            best_configuration = perform_evolutionary_search(
+                experiment,
+                available_decisions,
+                arguments,
+                optimizer_dir,
+            )
+        # calculate costs for all combinations of decisions
+        elif arguments.optimization_level == 3:
+            best_configuration = evaluate_all_decision_combinations(
+                experiment, available_decisions, arguments, optimizer_dir
+            )
+        else:
+            raise ValueError("No valid optimization method specified: " + str(arguments.optimization_level))
 
-    # calculate costs for all combinations of decisions
-    if arguments.exhaustive:
-        best_configuration = evaluate_all_decision_combinations(
-            experiment, available_decisions, arguments, optimizer_dir
-        )
-    elif arguments.evolutionary != None:
-        # perform evolutionary search
-        best_configuration = perform_evolutionary_search(
-            experiment,
-            available_decisions,
-            arguments,
-            optimizer_dir,
-        )
-    else:
-        raise ValueError("No optimization method specified!")
+        print("BEST CONFIGURATION: ", best_configuration)
 
     if best_configuration is not None:
+        # calculate updates for best_configuration
+        updates = new_calculate_data_transfers(experiment.optimization_graph, best_configuration.decisions, experiment)
+        # register updates
+        best_configuration.data_movement = []
+        for u in updates:
+            best_configuration.add_data_movement(u)
+
         best_configuration = optimize_updates(experiment, best_configuration, arguments)
         # append the configuration to the list of patterns
         experiment.detection_result.patterns.optimizer_output.append(best_configuration)
 
+    if arguments.profiling:
+        experiment.profile.disable()  # type: ignore
+        if os.path.exists("optimizer_profile.txt"):
+            os.remove("optimizer_profile.txt")
+        with open("optimizer_profile.txt", "w+") as f:
+            stats = pstats.Stats(experiment.profile, stream=f).sort_stats("time").reverse_order()  # type: ignore
+            stats.print_stats()
+        del experiment.profile  # type: ignore
+
     # save full experiment to disk
     export_to_json(experiment, optimizer_dir)
     # save updated patterns.json to disk
     export_patterns_to_json(experiment, os.path.join(optimizer_dir, "patterns.json"))
     # save updated detection_result to disk
     export_detection_result_to_json(experiment, os.path.join(optimizer_dir, "detection_result_dump.json"))
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/scheduling/workload_delta.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/scheduling/workload_delta.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/do_all.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/reduction.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.Microbench.utils import (
     convert_discopop_to_microbench_workload,
 )
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.classes.edges.MutuallyExclusiveEdge import MutuallyExclusiveEdge
 from discopop_library.discopop_optimizer.classes.edges.OptionEdge import OptionEdge
-from discopop_library.discopop_optimizer.classes.edges.RequirementEdge import RequirementEdge
 from discopop_library.discopop_optimizer.classes.nodes.Loop import Loop
 from discopop_library.discopop_optimizer.classes.nodes.Workload import Workload
 from discopop_library.discopop_optimizer.classes.system.devices.CPU import CPU
 from discopop_library.discopop_optimizer.classes.system.devices.GPU import GPU
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 
 suggestion_device_types = [CPU, GPU]
@@ -36,18 +35,18 @@
     # get all devices which can be used to execute the suggestion
     suggestion_device_ids = []
     for device_type in suggestion_device_types:
         suggestion_device_ids += environment.get_system().get_device_ids_by_type(device_type)
 
     for node in buffer:
         introduced_options: Set[int] = set()
-        if suggestion.node_id == data_at(graph, node).cu_id:
+        if suggestion.node_id == data_at(graph, node).cu_id and type(data_at(graph, node)) == Loop:
             # save node in introduced_options to mark as mutually exclusive
             introduced_options.add(node)
-            # todo: This implementation for the device id is temporary and MUST be replaced
+            environment.pattern_id_to_decisions_dict[suggestion.pattern_id] = [node]
             for device_id in suggestion_device_ids:
                 # reserve a node id for the new parallelization option
                 new_node_id = get_next_free_node_id_function()
                 # copy data from existing node
                 node_data_copy = copy.deepcopy(data_at(graph, node))
                 node_data_copy.node_id = new_node_id
                 # register new node_id for pattern
@@ -58,20 +57,19 @@
 
                 # set the device id for the suggestion
                 node_data_copy.device_id = device_id
                 # remove cu_id to prevent using parallelization options as basis for new versions
                 node_data_copy.cu_id = None
                 # mark node for parallel execution
                 node_data_copy.execute_in_parallel = True
-
                 # copy loop iteration variable
                 cast(Loop, node_data_copy).iterations_symbol = cast(Loop, node_data_copy).iterations_symbol
                 # add suggestion to node data
                 node_data_copy.suggestion = suggestion
-                node_data_copy.suggestion_type = "do_all"
+                node_data_copy.suggestion_type = "reduction"
                 # add the cost multiplier to represent the effects of the suggestion
                 (
                     cast(Workload, node_data_copy).cost_multiplier,
                     introduced_symbols,
                 ) = get_cost_multiplier(new_node_id, environment, device_id)
                 # add the overhead term to represent the overhead incurred by the suggestion
                 cast(Workload, node_data_copy).overhead, tmp_introduced_symbols = get_overhead_term(
@@ -81,76 +79,72 @@
 
                 node_data_copy.introduced_symbols += introduced_symbols
 
                 # create a new node for the option
                 graph.add_node(new_node_id, data=node_data_copy)
                 # mark the newly created option
                 # graph.add_edge(node, new_node_id, data=OptionEdge())
-                # print("ADDED OPTION EDGE: ", node, new_node_id)
 
                 # save the id of the introduced parallelization option to connect them afterwards
                 introduced_options.add(new_node_id)
 
                 # connect the newly created node to the parent and successor of node
                 for edge in graph.in_edges(node):
                     edge_data = copy.deepcopy(graph.edges[edge]["data"])
                     graph.add_edge(edge[0], new_node_id, data=edge_data)
                 for edge in graph.out_edges(node):
                     edge_data = copy.deepcopy(graph.edges[edge]["data"])
                     graph.add_edge(new_node_id, edge[1], data=edge_data)
-                    # if a successor has no device id already,
+                    # if the successor has no device id already,
                     # set it to 0 to simulate "leaving" the device after the suggestion
                     # todo: this should not happen here, but be considered when calculating the updates in order to
                     #  prevent suggestions from influencing each other by "mapping" workloads to certain devices.
                     # todo re-enable?
-                    # if (
-                    #    type(edge_data) == SuccessorEdge
-                    #    and data_at(graph, edge[1]).device_id is None
-                    # ):
-                    #   data_at(graph, edge[1]).device_id = 0
+                    # if data_at(graph, edge[1]).device_id is None:
+                    #     data_at(graph, edge[1]).device_id = 0
 
         # connect introduced parallelization options to support path restraining
         for node_id_1 in introduced_options:
             for node_id_2 in introduced_options:
                 if node_id_1 == node_id_2:
                     continue
                 graph.add_edge(node_id_1, node_id_2, data=MutuallyExclusiveEdge())
     return graph
 
 
 def get_cost_multiplier(node_id: int, environment: Experiment, device_id: int) -> Tuple[CostModel, List[Symbol]]:
     """Creates and returns the multiplier to represent the effects of the given suggestion on the cost model.
     A CostModel object is used to store the information on the path selection.
     Returns the multiplier and the list of introduces symbols
-    Multiplier for Do-All:
-        1 / Thread_count"""
+    Multiplier for Reduction:
+        1 / Compute_capa"""
     # get device specifications
-
-    thread_count = environment.get_system().get_device(device_id).get_thread_count()
-
-    multiplier = Integer(1) / thread_count
+    # todo: add reduction speedup measurement to the OpenMP Microbenchmark suite
+    speedup = environment.get_system().get_device(device_id).get_measured_speedup()
+    multiplier = Integer(1) / speedup
     cm = CostModel(multiplier, Integer(1))
 
     # return cm, [thread_count]
     return cm, []
 
 
 def get_overhead_term(node_data: Loop, environment: Experiment, device_id: int) -> Tuple[CostModel, List[Symbol]]:
     """Creates and returns the Expression which represents the Overhead incurred by the given suggestion.
     For testing purposes, the following function is used to represent the overhead incurred by a do-all loop.
     The function has been created using Extra-P.
-    unit of the overhead term are micro seconds."""
-    # retrieve DoAll overhead model
-    overhead_model = environment.get_system().get_device_doall_overhead_model(
+    Unit of the overhead term are micro seconds."""
+
+    # retrieve Reduction overhead model
+    overhead_model = environment.get_system().get_device_reduction_overhead_model(
         environment.get_system().get_device(device_id), environment.arguments
     )
     # substitute workload, iterations and threads
     thread_count = environment.get_system().get_device(device_id).get_thread_count()
     iterations = node_data.iterations_symbol
-    # since node_data is of type Loop, parallelizable_workload must be set
+    # since node_data is of type Loop, parallelizable_workload has to exist
     per_iteration_workload = cast(Expr, node_data.parallelizable_workload)
     # convert DiscoPoP workload to Microbench workload
     converted_per_iteration_workload = convert_discopop_to_microbench_workload(per_iteration_workload, iterations)
 
     substitutions: Dict[Symbol, Expr] = {}
 
     for symbol in cast(List[Symbol], overhead_model.free_symbols):
@@ -161,16 +155,13 @@
         elif symbol.name == "threads":
             substitutions[symbol] = thread_count
         else:
             raise ValueError("Unknown symbol: ", symbol)
 
     substituted_overhead_model = overhead_model.xreplace(substitutions)
 
-    # register symbol for overhead
-    doall_overhead_symbol = Symbol("doall_" + str(node_data.node_id) + "_pos_" + str(node_data.position) + "_overhead")
+    cm = CostModel(Integer(0), substituted_overhead_model)
 
-    environment.substitutions[doall_overhead_symbol] = substituted_overhead_model
+    # todo: convert result (in s) to workload
 
-    # cm = CostModel(Integer(0), substituted_overhead_model)
-    cm = CostModel(Integer(0), doall_overhead_symbol)
     # add weight to overhead
     return cm, []
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/main.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This file is part of the DiscoPoP software (http://www.discopop.tu-darmstadt.de)
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
+import copy
 import networkx as nx  # type: ignore
 
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.suggestions.importers.do_all import (
     import_suggestion as import_doall,
 )
 from discopop_library.discopop_optimizer.suggestions.importers.reduction import (
@@ -16,15 +17,16 @@
 )
 
 
 def import_suggestions(experiment: Experiment) -> nx.DiGraph:
     """Imports the suggestions specified in res into the graph stored in the given experiment and returns the modified graph"""
 
     # import do-all
-    for do_all_suggestion in experiment.detection_result.patterns.do_all:
+    buffer = copy.deepcopy(experiment.detection_result.patterns.do_all)
+    for do_all_suggestion in buffer:
         experiment.optimization_graph = import_doall(
             experiment.optimization_graph, do_all_suggestion, experiment.get_next_free_node_id, experiment
         )
 
     # import reduction
     for reduction_suggestion in experiment.detection_result.patterns.reduction:
         experiment.optimization_graph = import_reduction(
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/importers/reduction.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/importers/do_all.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,50 +2,59 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import copy
+import logging
 from typing import Set, cast, Tuple, List, Dict
 
 import networkx as nx  # type: ignore
-from sympy import Expr, Integer, Symbol, log, Float, init_printing  # type: ignore
+from sympy import Expr, Integer, Symbol, log, Float, init_printing
+from discopop_explorer.PEGraphX import NodeID
+from discopop_explorer.pattern_detectors.do_all_detector import DoAllInfo  # type: ignore
 
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.Microbench.utils import (
     convert_discopop_to_microbench_workload,
 )
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.classes.edges.MutuallyExclusiveEdge import MutuallyExclusiveEdge
 from discopop_library.discopop_optimizer.classes.edges.OptionEdge import OptionEdge
+from discopop_library.discopop_optimizer.classes.edges.RequirementEdge import RequirementEdge
 from discopop_library.discopop_optimizer.classes.nodes.Loop import Loop
 from discopop_library.discopop_optimizer.classes.nodes.Workload import Workload
 from discopop_library.discopop_optimizer.classes.system.devices.CPU import CPU
+from discopop_library.discopop_optimizer.classes.system.devices.DeviceTypeEnum import DeviceTypeEnum
 from discopop_library.discopop_optimizer.classes.system.devices.GPU import GPU
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
+from discopop_library.result_classes.OptimizerOutputPattern import OptimizerOutputPattern
 
 suggestion_device_types = [CPU, GPU]
+logger = logging.getLogger("Optimizer")
 
 
 def import_suggestion(
     graph: nx.DiGraph, suggestion, get_next_free_node_id_function, environment: Experiment
 ) -> nx.DiGraph:
     # find a node which belongs to the suggestion
     buffer = [n for n in graph.nodes]
     # get all devices which can be used to execute the suggestion
     suggestion_device_ids = []
     for device_type in suggestion_device_types:
         suggestion_device_ids += environment.get_system().get_device_ids_by_type(device_type)
 
     for node in buffer:
         introduced_options: Set[int] = set()
-        if suggestion.node_id == data_at(graph, node).cu_id:
+        if suggestion.node_id == data_at(graph, node).cu_id and type(data_at(graph, node)) == Loop:
             # save node in introduced_options to mark as mutually exclusive
             introduced_options.add(node)
+            environment.pattern_id_to_decisions_dict[suggestion.pattern_id] = [node]
+            # todo: This implementation for the device id is temporary and MUST be replaced
             for device_id in suggestion_device_ids:
                 # reserve a node id for the new parallelization option
                 new_node_id = get_next_free_node_id_function()
                 # copy data from existing node
                 node_data_copy = copy.deepcopy(data_at(graph, node))
                 node_data_copy.node_id = new_node_id
                 # register new node_id for pattern
@@ -56,19 +65,20 @@
 
                 # set the device id for the suggestion
                 node_data_copy.device_id = device_id
                 # remove cu_id to prevent using parallelization options as basis for new versions
                 node_data_copy.cu_id = None
                 # mark node for parallel execution
                 node_data_copy.execute_in_parallel = True
+
                 # copy loop iteration variable
                 cast(Loop, node_data_copy).iterations_symbol = cast(Loop, node_data_copy).iterations_symbol
                 # add suggestion to node data
                 node_data_copy.suggestion = suggestion
-                node_data_copy.suggestion_type = "reduction"
+                node_data_copy.suggestion_type = "do_all"
                 # add the cost multiplier to represent the effects of the suggestion
                 (
                     cast(Workload, node_data_copy).cost_multiplier,
                     introduced_symbols,
                 ) = get_cost_multiplier(new_node_id, environment, device_id)
                 # add the overhead term to represent the overhead incurred by the suggestion
                 cast(Workload, node_data_copy).overhead, tmp_introduced_symbols = get_overhead_term(
@@ -78,72 +88,137 @@
 
                 node_data_copy.introduced_symbols += introduced_symbols
 
                 # create a new node for the option
                 graph.add_node(new_node_id, data=node_data_copy)
                 # mark the newly created option
                 # graph.add_edge(node, new_node_id, data=OptionEdge())
+                # print("ADDED OPTION EDGE: ", node, new_node_id)
 
                 # save the id of the introduced parallelization option to connect them afterwards
                 introduced_options.add(new_node_id)
 
                 # connect the newly created node to the parent and successor of node
                 for edge in graph.in_edges(node):
                     edge_data = copy.deepcopy(graph.edges[edge]["data"])
                     graph.add_edge(edge[0], new_node_id, data=edge_data)
                 for edge in graph.out_edges(node):
                     edge_data = copy.deepcopy(graph.edges[edge]["data"])
                     graph.add_edge(new_node_id, edge[1], data=edge_data)
-                    # if the successor has no device id already,
+                    # if a successor has no device id already,
                     # set it to 0 to simulate "leaving" the device after the suggestion
                     # todo: this should not happen here, but be considered when calculating the updates in order to
                     #  prevent suggestions from influencing each other by "mapping" workloads to certain devices.
                     # todo re-enable?
-                    # if data_at(graph, edge[1]).device_id is None:
-                    #     data_at(graph, edge[1]).device_id = 0
+                    # if (
+                    #    type(edge_data) == SuccessorEdge
+                    #    and data_at(graph, edge[1]).device_id is None
+                    # ):
+                    #   data_at(graph, edge[1]).device_id = 0
+
+                # register the device-mapped suggestion
+                if device_id != environment.get_system().get_host_device_id():
+                    pattern_info = DoAllInfo(
+                        environment.detection_result.pet,
+                        environment.detection_result.pet.node_at(cast(NodeID, node_data_copy.original_cu_id)),
+                    )
+                    pattern_info.collapse_level = suggestion.collapse_level
+                    pattern_info.device_id = device_id
+                    pattern_info.device_type = environment.get_system().get_device(device_id).get_device_type()
+                    pattern_info.applicable_pattern = False
+
+                    environment.detection_result.patterns.do_all.append(pattern_info)
+
+                    if environment.arguments.single_suggestions:
+                        # register the individual Pattern as a OutputPattern to reflect the device mapping of a regular suggestion
+                        optimizer_output_pattern = OptimizerOutputPattern(
+                            suggestion._node, [new_node_id], environment.get_system().get_host_device_id(), environment
+                        )
+                        logger.info("Created OptimizerOutputPattern: " + str(optimizer_output_pattern.pattern_id))
+
+                        optimizer_output_pattern.add_pattern(
+                            pattern_info.pattern_id, pattern_info.device_id, pattern_info.device_type
+                        )
+                        environment.detection_result.patterns.optimizer_output.append(optimizer_output_pattern)
 
         # connect introduced parallelization options to support path restraining
         for node_id_1 in introduced_options:
             for node_id_2 in introduced_options:
                 if node_id_1 == node_id_2:
                     continue
                 graph.add_edge(node_id_1, node_id_2, data=MutuallyExclusiveEdge())
     return graph
 
 
 def get_cost_multiplier(node_id: int, environment: Experiment, device_id: int) -> Tuple[CostModel, List[Symbol]]:
     """Creates and returns the multiplier to represent the effects of the given suggestion on the cost model.
     A CostModel object is used to store the information on the path selection.
     Returns the multiplier and the list of introduces symbols
-    Multiplier for Reduction:
-        1 / Compute_capa"""
+    Multiplier for Do-All:
+        1 / Thread_count"""
     # get device specifications
-    thread_count = environment.get_system().get_device(device_id).get_thread_count()
+    # thread_count = environment.get_system().get_device(device_id).get_thread_count()
+    speedup = environment.get_system().get_device(device_id).get_measured_speedup()
+    multiplier = Integer(1) / speedup
 
-    multiplier = Integer(1) / thread_count
     cm = CostModel(multiplier, Integer(1))
 
     # return cm, [thread_count]
     return cm, []
 
 
 def get_overhead_term(node_data: Loop, environment: Experiment, device_id: int) -> Tuple[CostModel, List[Symbol]]:
     """Creates and returns the Expression which represents the Overhead incurred by the given suggestion.
     For testing purposes, the following function is used to represent the overhead incurred by a do-all loop.
     The function has been created using Extra-P.
-    Unit of the overhead term are micro seconds."""
+    unit of the overhead term are micro seconds."""
+    ci_costs = environment.get_system().get_device(device_id).get_compute_init_delays()
+
+    # get overhead model
+    if environment.get_system().get_device(node_data.device_id).get_device_type() == DeviceTypeEnum.CPU:
+        # device is CPU
+        if len(cast(DoAllInfo, node_data.suggestion).shared) == 0:
+            # retrieve DoAll overhead model
+            overhead_model = environment.get_system().get_device_doall_overhead_model(
+                environment.get_system().get_device(device_id), environment.arguments
+            )
+            logger.info("Loop: " + str(node_data.node_id) + " is DOALL")
+        else:
+            # retrieve DoAll shared overhead model
+            overhead_model = environment.get_system().get_device_doall_shared_overhead_model(
+                environment.get_system().get_device(device_id), environment.arguments
+            )
+            logger.info("Loop: " + str(node_data.node_id) + " is DOALL SHARED")
+        # add computation initialization costs (technically duplicated, but required for low workloads)
+        if "doall" in ci_costs:
+            overhead_model += Float(ci_costs["doall"])
+            logger.debug(
+                "Added doall compute init delay: " + str(ci_costs["doall"]) + " to node: " + str(node_data.node_id)
+            )
+        else:
+            logger.debug("Could not find compute init delays for node: " + str(node_data.node_id))
+    else:
+        # device is GPU
+        overhead_model = Integer(0)
+        # add computation initialization costs (technically duplicated, but required for low workloads)
+        if "target_teams_distribute_parallel_for" in ci_costs:
+            overhead_model += Float(ci_costs["target_teams_distribute_parallel_for"])
+            logger.debug(
+                "Added ttdpf compute init delay: "
+                + str(ci_costs["target_teams_distribute_parallel_for"])
+                + " to node: "
+                + str(node_data.node_id)
+            )
+        else:
+            logger.debug("Could not find compute init delays for node: " + str(node_data.node_id))
 
-    # retrieve Reduction overhead model
-    overhead_model = environment.get_system().get_device_reduction_overhead_model(
-        environment.get_system().get_device(device_id), environment.arguments
-    )
     # substitute workload, iterations and threads
     thread_count = environment.get_system().get_device(device_id).get_thread_count()
     iterations = node_data.iterations_symbol
-    # since node_data is of type Loop, parallelizable_workload has to exist
+    # since node_data is of type Loop, parallelizable_workload must be set
     per_iteration_workload = cast(Expr, node_data.parallelizable_workload)
     # convert DiscoPoP workload to Microbench workload
     converted_per_iteration_workload = convert_discopop_to_microbench_workload(per_iteration_workload, iterations)
 
     substitutions: Dict[Symbol, Expr] = {}
 
     for symbol in cast(List[Symbol], overhead_model.free_symbols):
@@ -154,13 +229,16 @@
         elif symbol.name == "threads":
             substitutions[symbol] = thread_count
         else:
             raise ValueError("Unknown symbol: ", symbol)
 
     substituted_overhead_model = overhead_model.xreplace(substitutions)
 
-    cm = CostModel(Integer(0), substituted_overhead_model)
+    # register symbol for overhead
+    doall_overhead_symbol = Symbol("doall_" + str(node_data.node_id) + "_pos_" + str(node_data.position) + "_overhead")
 
-    # todo: convert result (in s) to workload
+    environment.substitutions[doall_overhead_symbol] = substituted_overhead_model
 
+    # cm = CostModel(Integer(0), substituted_overhead_model)
+    cm = CostModel(Integer(0), doall_overhead_symbol)
     # add weight to overhead
     return cm, []
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/optimizers/loop_collapse.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/optimizers/loop_collapse.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,21 +3,24 @@
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
 import copy
+import logging
 from multiprocessing import Pool
 from typing import Dict, List, Set, Tuple, cast
 from sympy import Integer, Symbol
 
 import networkx as nx  # type: ignore
 
 import tqdm  # type: ignore
+from discopop_library.discopop_optimizer.classes.nodes.ContextNode import ContextNode  # type: ignore
+from discopop_library.result_classes.OptimizerOutputPattern import OptimizerOutputPattern  # type: ignore
 from discopop_explorer.pattern_detectors.do_all_detector import DoAllInfo  # type: ignore
 from discopop_library.PatternIdManagement.unique_pattern_id import get_unique_pattern_id
 from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.classes.edges.MutuallyExclusiveEdge import MutuallyExclusiveEdge
 from discopop_library.discopop_optimizer.classes.edges.OptionEdge import OptionEdge
 from discopop_library.discopop_optimizer.classes.edges.RequirementEdge import RequirementEdge
 from discopop_library.discopop_optimizer.classes.nodes.Loop import Loop
@@ -25,19 +28,22 @@
 from discopop_library.discopop_optimizer.utilities.MOGUtilities import (
     get_all_function_nodes,
     get_all_loop_nodes,
     get_all_parents,
     get_children,
     get_out_mutex_edges,
     get_parents,
+    get_predecessors,
     get_successors,
     show,
 )
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 
+logger = logging.getLogger("Optimizer")
+
 global_graph = None
 global_experiment = None
 
 
 def collapse_loops(experiment: Experiment) -> nx.DiGraph:
     """identifies collapse loops and depicts them in the optimization graph"""
 
@@ -86,33 +92,60 @@
 
     while modifiation_found:
         modifiation_found = False
 
         #        # set of loops could change when modifications are applied, hence the copy
         #        loops = get_all_loop_nodes(global_graph)
         for loop in copy.deepcopy(relevant_loops):
+            logging.info("Checking loop collapse for @ " + str(loop))
             loop_data = data_at(global_graph, loop)
             #            if function_node_id not in get_all_parents(global_graph, loop):
             #                continue
             # loop contained in function
             # check for loop nesting
             queue: List[int] = get_parents(global_graph, loop)
             collapse_sources: Set[int] = set()
             while queue:
                 current = queue.pop()
+                logger.debug("\tCurrent: " + str(current))
                 current_data = data_at(global_graph, current)
 
                 if type(current_data) == Loop:
                     # parent is parallelizable loop -> collapse and end search
                     if current_data.suggestion_type == "do_all":
                         # if loops are located on the same device, collapse
                         if loop_data.device_id == current_data.device_id:
                             if loop not in visited_inner_loop:
-                                collapse_sources.add(current)
-                                visited_inner_loop.add(loop)
+                                # calculate distance of loop to parent to check for perfect nesting (distance <= 2 due to graph structure)
+                                distance_to_parent = 0
+                                inner_queue: List[Tuple[int, int]] = [(loop, 0)]
+                                while inner_queue:
+                                    logger.debug("\tInner queue: " + str(inner_queue))
+                                    inner_current, tmp_dist = inner_queue.pop()
+                                    preds = get_predecessors(global_graph, inner_current)
+                                    if len(preds) == 0:
+                                        if tmp_dist > distance_to_parent:
+                                            distance_to_parent = tmp_dist
+                                        continue
+                                    else:
+                                        inner_queue += [
+                                            (
+                                                p,
+                                                (
+                                                    tmp_dist
+                                                    if isinstance(data_at(global_graph, p), ContextNode)
+                                                    else tmp_dist + 1
+                                                ),
+                                            )
+                                            for p in preds
+                                        ]
+                                logger.debug("\t\tCollapse at distance: " + str(distance_to_parent))
+                                if distance_to_parent <= 2:
+                                    collapse_sources.add(current)
+                                    visited_inner_loop.add(loop)
                             continue
                     # parent is regular loop -> end search on this path
                     continue
 
                 # parent is empty node -> skip
                 if isinstance(current_data, Workload):
                     if cast(Workload, current_data).sequential_workload == Integer(0):
@@ -163,14 +196,15 @@
                 )
                 pattern_id = pattern_info.pattern_id
                 pattern_info.collapse_level = node_data_copy.collapse_level
                 pattern_info.device_id = node_data_copy.device_id
                 pattern_info.device_type = (
                     global_experiment.get_system().get_device(node_data_copy.device_id).get_device_type()
                 )
+                pattern_info.applicable_pattern = False  # patterns are only applicable via the optimizer output pattern interfaces due to potential data movement
                 global_experiment.suggestion_to_node_ids_dict[pattern_id] = [new_node_id]
                 global_experiment.node_id_to_suggestion_dict[new_node_id] = pattern_id
 
                 # create a new node
                 global_graph.add_node(new_node_id, data=node_data_copy)
 
                 # copy edges
@@ -236,13 +270,24 @@
                 # create a new requirements edge to the single-iteration sequential version of the inner loop
                 global_graph.add_edge(copy_seq_loop_option_id, new_node_id, data=RequirementEdge())
                 global_graph.add_edge(new_node_id, copy_seq_loop_option_id, data=RequirementEdge())
 
                 # register pattern for output
                 # todo: find a nicer solution to duplicating the patterns for each device mapping
                 global_experiment.detection_result.patterns.do_all.append(pattern_info)
+                # construct optimizer output pattern to represent the non-standalone pattern_info
+                optimizer_output_pattern = OptimizerOutputPattern(
+                    pattern_info._node,
+                    [new_node_id],
+                    global_experiment.get_system().get_host_device_id(),
+                    global_experiment,
+                )
+                optimizer_output_pattern.add_pattern(
+                    pattern_info.pattern_id, pattern_info.device_id, pattern_info.device_type
+                )
+                global_experiment.detection_result.patterns.optimizer_output.append(optimizer_output_pattern)
                 print("REGISTERED PATTERN INFO: ", pattern_id, " for Device: ", data_at(global_graph, csrc).device_id)
                 print(pattern_info)
                 print()
 
         return_value = return_value or modifiation_found
     return return_value
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/suggestions/optimizers/main.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/suggestions/optimizers/main.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/utilities/MOGUtilities.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/utilities/MOGUtilities.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,31 +5,34 @@
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import copy
 import itertools
 from multiprocessing import Pool
 from typing import Any, ClassVar, Dict, List, Optional, cast, Set, Tuple
+import warnings
 
 import matplotlib  # type: ignore
 import matplotlib.pyplot as plt  # type:ignore
 import networkx as nx  # type: ignore
 import tqdm  # type: ignore
 
 from discopop_explorer.PEGraphX import MemoryRegion, NodeID
 from discopop_library.discopop_optimizer.OptimizerArguments import OptimizerArguments
+from discopop_library.discopop_optimizer.classes.edges.CallEdge import CallEdge
 from discopop_library.discopop_optimizer.classes.edges.DataFlowEdge import DataFlowEdge
 from discopop_library.discopop_optimizer.classes.edges.MutuallyExclusiveEdge import MutuallyExclusiveEdge
 from discopop_library.discopop_optimizer.classes.edges.ChildEdge import ChildEdge
 from discopop_library.discopop_optimizer.classes.edges.GenericEdge import GenericEdge
 from discopop_library.discopop_optimizer.classes.edges.OptionEdge import OptionEdge
 from discopop_library.discopop_optimizer.classes.edges.RequirementEdge import RequirementEdge
 from discopop_library.discopop_optimizer.classes.edges.SuccessorEdge import SuccessorEdge
 from discopop_library.discopop_optimizer.classes.edges.TemporaryEdge import TemporaryEdge
 from discopop_library.discopop_optimizer.classes.nodes.ContextNode import ContextNode
+from discopop_library.discopop_optimizer.classes.nodes.FunctionReturn import FunctionReturn
 from discopop_library.discopop_optimizer.classes.nodes.FunctionRoot import FunctionRoot
 from discopop_library.discopop_optimizer.classes.nodes.GenericNode import GenericNode
 from discopop_library.discopop_optimizer.classes.nodes.Loop import Loop
 from discopop_library.discopop_optimizer.classes.nodes.Workload import Workload
 from discopop_library.discopop_optimizer.utilities.simple_utilities import data_at
 
 from networkx.drawing.nx_pydot import graphviz_layout  # type: ignore
@@ -88,25 +91,101 @@
 
 
 def get_out_mutex_edges(graph: nx.DiGraph, node_id: int) -> List[int]:
     """Returns a list of node ids which are mutually exclusive to the current node_id"""
     return [edge[1] for edge in graph.out_edges(node_id, data="data") if isinstance(edge[2], MutuallyExclusiveEdge)]
 
 
+def get_out_call_edges(graph: nx.DiGraph, node_id: int) -> List[int]:
+    """Returns a list of node ids which are called by current node_id"""
+    return [edge[1] for edge in graph.out_edges(node_id, data="data") if isinstance(edge[2], CallEdge)]
+
+
 def get_requirements(graph: nx.DiGraph, node_id: int) -> List[int]:
     """Returns a list of node ids for the requirements of the parallelization option in the given node"""
     return [edge[1] for edge in graph.out_edges(node_id, data="data") if isinstance(edge[2], RequirementEdge)]
 
 
 def has_temporary_successor(graph: nx.DiGraph, node_id: int) -> bool:
     """Checks whether the given node has outgoing temporary successor edges"""
     return len([edge for edge in graph.out_edges(node_id, data="data") if isinstance(edge[2], TemporaryEdge)]) > 0
 
 
-def show(graph, show_dataflow: bool = True, show_mutex_edges: bool = True):
+def get_function_return_node(graph: nx.DiGraph, function: int) -> int:
+    """Identify and return the FunctionReturn node belonging to function."""
+    queue = get_children(graph, function)
+    while len(queue) > 0:
+        current = queue.pop()
+        successors = get_successors(graph, current)
+        if len(successors) == 0 and type(data_at(graph, current)) == FunctionReturn:
+            return current
+        queue += [s for s in successors if s not in queue]
+    raise ValueError(
+        "No FunctionReturn found for function: "
+        + str(function)
+        + " "
+        + cast(FunctionRoot, data_at(graph, function)).name
+    )
+
+
+def show_decision_graph(
+    graph: nx.DiGraph, decisions: List[int], show_dataflow: bool = True, show_mutex_edges: bool = False
+):
+    print("Decisions: ", decisions)
+    contained_nodes: Set[int] = set()
+    for function in get_all_function_nodes(graph):
+        # get nodes in subtree of function, if they are reachable by the set of decisions
+        queue: List[int] = [data_at(graph, function).node_id]
+        while len(queue) > 0:
+            current = queue.pop()
+            contained_nodes.add(current)
+            queue += [c for c in get_children(graph, current) if c not in queue and c not in contained_nodes]
+            successors = get_successors(graph, current)
+
+            if len(successors) <= 1:
+                # no decision required
+                queue += [s for s in successors if s not in queue and s not in contained_nodes]
+            else:
+                # filter for successors in decisions
+                print("SUCCESSORS: ", successors)
+                valid_successors = [s for s in successors if s in decisions]
+                # check for requirements, if no valid successor was found
+                if len(valid_successors) == 0:
+                    requirements = []
+                    for dec in decisions:
+                        requirements += get_requirements(graph, dec)
+                    valid_successors = [s for s in successors if s in requirements]
+                    print("REQUIREMENT SUCCESSORS: ", valid_successors)
+                print("VALID SUCCESSORS: ", valid_successors)
+                # if no decision could be made, keep all sequential successors
+                if len(valid_successors) > 0:
+                    queue += [s for s in valid_successors if s not in queue and s not in contained_nodes]
+                else:
+                    # fallback
+                    queue += [s for s in successors if data_at(graph, s).represents_sequential_version()]
+
+    # show the subgraph
+    show(graph.subgraph(contained_nodes), show_dataflow=show_dataflow, show_mutex_edges=show_mutex_edges)
+
+
+def show_function(graph: nx.DiGraph, function: FunctionRoot, show_dataflow: bool = True, show_mutex_edges: bool = True):
+    # get nodes in subtree of function
+    contained_nodes: Set[int] = set()
+    queue: List[int] = [function.node_id]
+    while len(queue) > 0:
+        current = queue.pop()
+        contained_nodes.add(current)
+        queue += [c for c in get_children(graph, current) if c not in queue and c not in contained_nodes]
+        queue += [s for s in get_successors(graph, current) if s not in queue and s not in contained_nodes]
+
+    # show the subgraph
+    show(graph.subgraph(contained_nodes), show_dataflow=show_dataflow, show_mutex_edges=show_mutex_edges)
+
+
+def show(graph: nx.DiGraph, show_dataflow: bool = True, show_mutex_edges: bool = True):
     """Plots the graph
 
     :return:
     """
     matplotlib.use("TkAgg")
     fig, ax = plt.subplots()
     try:
@@ -218,14 +297,22 @@
         graph,
         pos,
         ax=ax,
         edge_color="yellow",
         edgelist=[e for e in graph.edges(data="data") if isinstance(e[2], RequirementEdge)],
     )
 
+    nx.draw_networkx_edges(
+        graph,
+        pos,
+        ax=ax,
+        edge_color="blue",
+        edgelist=[e for e in graph.edges(data="data") if isinstance(e[2], CallEdge)],
+    )
+
     if show_mutex_edges:
         nx.draw_networkx_edges(
             graph,
             pos,
             ax=ax,
             edge_color="orange",
             edgelist=[e for e in graph.edges(data="data") if isinstance(e[2], MutuallyExclusiveEdge)],
@@ -295,14 +382,19 @@
 
 
 def add_child_edge(graph: nx.DiGraph, source_id: int, target_id: int):
     edge_data = ChildEdge()
     graph.add_edge(source_id, target_id, data=edge_data)
 
 
+def add_call_edge(graph: nx.DiGraph, source_id: int, target_id: int):
+    edge_data = CallEdge()
+    graph.add_edge(source_id, target_id, data=edge_data)
+
+
 def add_temporary_edge(graph: nx.DiGraph, source_id: int, target_id: int):
     edge_data = TemporaryEdge()
     graph.add_edge(source_id, target_id, data=edge_data)
 
 
 def add_dataflow_edge(graph: nx.DiGraph, source_id: int, target_id: int):
     edge_data = DataFlowEdge()
@@ -356,17 +448,25 @@
         if type(graph.nodes[node_id]["data"]) == FunctionRoot:
             result_set.add(node_id)
     return list(result_set)
 
 
 def get_all_nodes_in_function(graph: nx.DiGraph, function_id: int) -> List[int]:
     result_list: List[int] = []
-    for node_id in graph.nodes:
-        if function_id in get_all_parents(graph, node_id):
-            result_list.append(node_id)
+    queue: List[int] = [function_id]
+    while len(queue) > 0:
+        current = queue.pop()
+        if current != function_id:
+            result_list.append(current)
+        queue += [c for c in get_children(graph, current) if c not in result_list and c not in queue]
+        queue += [s for s in get_successors(graph, current) if s not in result_list and s not in queue]
+
+    #    for node_id in graph.nodes:
+    #        if function_id in get_all_parents(graph, node_id):
+    #            result_list.append(node_id)
     return result_list
 
 
 def get_nodes_by_functions(graph: nx.DiGraph) -> Dict[int, List[int]]:
     result_dict: Dict[int, List[int]] = dict()
     function_nodes = set(get_all_function_nodes(graph))
     for node in graph.nodes:
@@ -390,21 +490,24 @@
 def get_read_and_written_data_from_subgraph(
     graph: nx.DiGraph, node_id: int, ignore_successors: bool = False
 ) -> Tuple[Set[MemoryRegion], Set[MemoryRegion]]:
     """Collect written and read memory regions for the node itself, it's successor and it's children. Used in the data flow calculation step."""
     read_memory_regions: Set[MemoryRegion] = set()
     written_memory_regions: Set[MemoryRegion] = set()
     # collect reads and writes from successors and children
-    subgraph = get_children(graph, node_id)
-    if not ignore_successors:
-        subgraph += get_successors(graph, node_id)
-    for successor in subgraph:
-        reads, writes = get_read_and_written_data_from_subgraph(graph, successor)
-        read_memory_regions.update(reads)
-        written_memory_regions.update(writes)
+    try:
+        subgraph = get_children(graph, node_id)
+        if not ignore_successors:
+            subgraph += get_successors(graph, node_id)
+        for successor in subgraph:
+            reads, writes = get_read_and_written_data_from_subgraph(graph, successor)
+            read_memory_regions.update(reads)
+            written_memory_regions.update(writes)
+    except RecursionError:
+        warnings.warn("Recursion limit exceeeded. Read and write in subtrees might be inaccurate.")
     # add reads and writes of the node itself
     node_data = data_at(graph, node_id)
     read_memory_regions.update([read_access.memory_region for read_access in node_data.read_memory_regions])
     written_memory_regions.update([write_access.memory_region for write_access in node_data.written_memory_regions])
 
     return read_memory_regions, written_memory_regions
 
@@ -447,14 +550,23 @@
         new_parents = [
             parent for parent in get_parents(graph, current) if parent not in queue and parent not in all_parents
         ]
         queue.update(new_parents)
     return list(all_parents)
 
 
+def get_parent_function(graph: nx.DiGraph, node_id: int) -> int:
+    """Returns the parent function of node_id"""
+    all_parents = get_all_parents(graph, node_id)
+    for p in all_parents:
+        if type(data_at(graph, p)) == FunctionRoot:
+            return p
+    raise ValueError("No parent exists for node " + str(node_id) + ", type: " + str(type(data_at(graph, node_id))))
+
+
 global_graph = None
 global_arguments = None
 
 
 def get_available_decisions_for_functions(
     graph: nx.DiGraph, arguments: OptimizerArguments
 ) -> Dict[FunctionRoot, List[List[int]]]:
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/RandomSamples.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/GlobalOptimization/RandomSamples.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/TopDown.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/utilities/optimization/LocalOptimization/TopDown.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 import copy
+import sys
 from typing import Dict, List, Tuple, Set, cast
 
 import networkx as nx  # type: ignore
 from sympy import Symbol, Expr
 
 from discopop_library.discopop_optimizer.CostModels.CostModel import CostModel
 from discopop_library.discopop_optimizer.CostModels.DataTransfer.DataTransferCosts import (
@@ -128,25 +129,27 @@
             minimum = sorted(unpacked_models, key=lambda x: x[2])[0]
             locally_optimal_choices.append(minimum[0])
 
         if len(locally_optimal_choices) == 0:
             continue
 
         # construct locally optimal model
+        sys.setrecursionlimit(100000)
         performance_models = get_node_performance_models(
             experiment,
             graph,
             function_node,
             set(),
             all_function_nodes,
             restrict_to_decisions=set(locally_optimal_choices),
             ignore_node_costs=[
                 cast(FunctionRoot, data_at(graph, function_node)).node_id
             ],  # ignore first node to prevent duplication of function costs
         )
+        sys.setrecursionlimit(1000)
         # calculate and append necessary data transfers to the models
         performance_models_with_transfers = calculate_data_transfers(
             graph, {cast(FunctionRoot, data_at(graph, function_node)): performance_models}, experiment
         )
 
         # calculate and append costs of data transfers to the performance models
         complete_performance_models = add_data_transfer_costs(graph, performance_models_with_transfers, environment)
```

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/utilities/simple_utilities.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/utilities/simple_utilities.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/utilities/visualization/plotting.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/utilities/visualization/plotting.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/discopop_optimizer/utilities/visualization/update_graph.py` & `discopop-3.2.0/discopop_library/discopop_optimizer/utilities/visualization/update_graph.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/global_data/version/__pycache__/utils.cpython-38.pyc` & `discopop-3.2.0/discopop_library/global_data/version/__pycache__/utils.cpython-38.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Wed Jan 17 10:29:46 2024 UTC, .py size: 539 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 550d 0d0a 0000 0000 1aac a765 1b02 0000  U..........e....
+00000000: 550d 0d0a 0000 0000 1d8b 3366 1b02 0000  U.........3f....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
 00000030: 6401 6c00 5a01 6400 6402 6c02 6d03 5a03  d.l.Z.d.d.l.m.Z.
 00000040: 0100 6504 6403 9c01 6404 6405 8404 5a05  ..e.d...d.d...Z.
 00000050: 6401 5300 2906 e900 0000 004e 2901 da04  d.S.)......N)...
 00000060: 5061 7468 2901 da06 7265 7475 726e 6300  Path)...returnc.
 00000070: 0000 0000 0000 0000 0000 0002 0000 000a  ................
```

### Comparing `discopop-3.1.1/discopop_library/global_data/version/utils.py` & `discopop-3.2.0/discopop_library/global_data/version/utils.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/result_classes/DetectionResult.py` & `discopop-3.2.0/discopop_library/result_classes/DetectionResult.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/discopop_library/result_classes/OptimizerOutputPattern.py` & `discopop-3.2.0/discopop_library/result_classes/OptimizerOutputPattern.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,33 +9,35 @@
 
 import json
 from typing import Any, Dict, List
 from discopop_explorer.PEGraphX import Node
 from discopop_explorer.pattern_detectors.PatternBase import PatternBase
 
 from discopop_library.PatternIdManagement.unique_pattern_id import get_unique_pattern_id
+from discopop_library.discopop_optimizer.Variables.Experiment import Experiment
 from discopop_library.discopop_optimizer.classes.context.Update import Update, construct_update_from_dict
 from discopop_library.discopop_optimizer.classes.system.devices.DeviceTypeEnum import DeviceTypeEnum
 from discopop_library.discopop_optimizer.classes.types.Aliases import DeviceID
 
 SuggestionId = int
 
 
 class OptimizerOutputPattern(PatternBase):
     applied_patterns: List[Dict[str, Any]]
     data_movement: List[Update]
     decisions: List[int]
     host_device_id: int
 
-    def __init__(self, node: Node, decisions: List[int], host_device_id: int):
+    def __init__(self, node: Node, decisions: List[int], host_device_id: int, experiment: Experiment):
         PatternBase.__init__(self, node)
         self.applied_patterns = []
         self.data_movement = []
         self.decisions = decisions
         self.host_device_id = host_device_id
+        experiment.pattern_id_to_decisions_dict[self.pattern_id] = decisions
 
     def reconstruct_from_file(self, file_path: str):  # todo remove?
         with open(file_path, "r") as f:
             loaded_data = json.load(f)
         self.applied_patterns = loaded_data["applied_patterns"]
         self.pattern_id = loaded_data["pattern_id"]
         self.host_device_id = loaded_data["host_device_id"]
@@ -58,7 +60,19 @@
             # get a unique pattern_id
             self.pattern_id = get_unique_pattern_id()
         tmp_dict = {"pattern_id": pattern_id, "device_id": target_device_id, "device_type": device_type}
         self.applied_patterns.append(tmp_dict)
 
     def add_data_movement(self, update: Update):
         self.data_movement.append(update)
+
+    def get_contained_decisions(self, experiment: Experiment) -> List[int]:
+        decision_list: List[int] = []
+        for d in self.decisions:
+            if d not in decision_list:
+                decision_list.append(d)
+        for tmp_dict in self.applied_patterns:
+            if tmp_dict["pattern_id"] in experiment.pattern_id_to_decisions_dict:
+                for d in experiment.pattern_id_to_decisions_dict[tmp_dict["pattern_id"]]:
+                    if d not in decision_list:
+                        decision_list.append(d)
+        return decision_list
```

### Comparing `discopop-3.1.1/discopop_library/result_classes/PatternStorage.py` & `discopop-3.2.0/discopop_library/result_classes/PatternStorage.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # Copyright (c) 2020, Technische Universitaet Darmstadt, Germany
 #
 # This software may be modified and distributed under the terms of
 # the 3-Clause BSD License.  See the LICENSE file in the package base
 # directory for details.
 
-from typing import List
+from typing import List, cast
 
 from discopop_explorer.pattern_detectors.PatternBase import PatternBase
 from discopop_explorer.pattern_detectors.PatternInfo import PatternInfo
 from discopop_explorer.pattern_detectors.do_all_detector import DoAllInfo
 from discopop_explorer.pattern_detectors.geometric_decomposition_detector import GDInfo
 from discopop_explorer.pattern_detectors.pipeline_detector import PipelineInfo
 from discopop_explorer.pattern_detectors.reduction_detector import ReductionInfo
@@ -21,10 +21,19 @@
     do_all: List[DoAllInfo]
     pipeline: List[PipelineInfo]
     geometric_decomposition: List[GDInfo]
     task: List[PatternInfo]
     simple_gpu: List[PatternInfo]
     combined_gpu: List[PatternInfo]
     optimizer_output: List[PatternBase]
+    merged_pattern: List[PatternBase]
 
     def __init__(self):
         self.optimizer_output = []
+        self.merged_pattern = []
+
+    def get_pattern_from_id(self, pattern_id: int) -> PatternBase:
+        for type in self.__dict__:
+            for suggestion in self.__dict__[type]:
+                if suggestion.pattern_id == pattern_id:
+                    return cast(PatternBase, suggestion)
+        raise ValueError("Pattern not found: " + str(pattern_id))
```

### Comparing `discopop-3.1.1/requirements.txt` & `discopop-3.2.0/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # directory for details.
 
 --index-url https://pypi.python.org/simple/
 
 about-time==4.2.1
 alive-progress==3.1.4
 appdirs==1.4.4
-black==23.7.0
+black==24.3.0
 click==8.1.7
 contextlib2==21.6.0
 contourpy==1.1.0
 cycler==0.11.0
 data-science-types==0.2.23
 extrap==4.0.3
 fonttools==4.43.0
@@ -31,15 +31,15 @@
 mpmath==1.3.0
 mypy==1.5.1
 mypy-extensions==1.0.0
 networkx==3.1
 numpy==1.24.4
 packaging==23.1
 pathspec==0.11.2
-Pillow==10.0.1
+Pillow==10.3.0
 pip==23.3
 platformdirs==3.10.0
 pluginbase==1.0.1
 pstats2==0.1.0
 pycubexr==1.2.1
 pyparsing==3.0.9
 PySide2==5.15.2.1
```

### Comparing `discopop-3.1.1/setup.py` & `discopop-3.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `discopop-3.1.1/test/do_all/daxpy/test.py` & `discopop-3.2.0/test/do_all/simple/not_nested/negative/stack_access/test.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,68 +1,74 @@
 import os
 import pathlib
 import unittest
 
 import jsonpickle
 
 from discopop_library.result_classes.DetectionResult import DetectionResult
+from test.utils.subprocess_wrapper.command_execution_wrapper import run_cmd
 from test.utils.validator_classes.DoAllInfoForValidation import DoAllInfoForValidation
 
+from discopop_library.ConfigProvider.config_provider import run as run_config_provider
+from discopop_library.ConfigProvider.ConfigProviderArguments import ConfigProviderArguments
+
 
 class TestMethods(unittest.TestCase):
     def test(self):
         current_dir = pathlib.Path(__file__).parent.resolve()
-        discopop_dir = os.path.join(current_dir, "..", "..", "..")
-        build_dir = os.path.join(discopop_dir, "build")
+        dp_build_dir = run_config_provider(
+            ConfigProviderArguments(
+                return_dp_build_dir=True,
+                return_dp_source_dir=False,
+                return_llvm_bin_dir=False,
+                return_version_string=False,
+            )
+        )
+
+        env_vars = dict(os.environ)
 
         src_dir = os.path.join(current_dir, "src")
         os.chdir(src_dir)
 
         # create FileMapping
-        os.system("" + os.path.join(build_dir, "scripts", "dp-fmap"))
+        cmd = os.path.join(dp_build_dir, "scripts", "dp-fmap")
+        run_cmd(cmd, src_dir, env_vars)
 
         # build
-        # make_command = "DP_FM_PATH=" + os.path.join(src_dir, "FileMapping.txt") + " "
-        make_command = ""
-        make_command += "CC=" + os.path.join(build_dir, "scripts", "CC_wrapper.sh") + " "
-        make_command += "CXX=" + os.path.join(build_dir, "scripts", "CXX_wrapper.sh") + " "
-        # make_command += "LINKER=" + os.path.join(build_dir, "scripts", "LINKER_wrapper.sh") + " "
-        make_command += "make "
-        os.system(make_command)
+        env_vars["CC"] = os.path.join(dp_build_dir, "scripts", "CC_wrapper.sh")
+        env_vars["CXX"] = os.path.join(dp_build_dir, "scripts", "CXX_wrapper.sh")
+        cmd = "make"
+        run_cmd(cmd, src_dir, env_vars)
+
         # execute instrumented program
-        os.system("./prog")
+        run_cmd("./prog", src_dir, env_vars)
         # execute DiscoPoP analysis
-        os.chdir(".discopop")
-        os.system("discopop_explorer")
-        os.chdir("..")
+
+        cwd = os.path.join(src_dir, ".discopop")
+        cmd = "discopop_explorer --enable-patterns doall,reduction"
+        run_cmd(cmd, cwd, env_vars)
         # validate results
-        self.validate_results(current_dir, src_dir)
-        # clean environment
-        os.system("make veryclean")
+        try:
+            self.validate_results(current_dir, src_dir)
+            # clean environment
+            run_cmd("make veryclean", src_dir, env_vars)
+        except Exception as ex:
+            # clean environment
+            run_cmd("make veryclean", src_dir, env_vars)
+            raise ex
 
     def validate_results(self, test_dir, src_dir):
-        """compare results to gold standard"""
-        gold_standard_file = os.path.join(test_dir, "detection_result_dump.json")
+        """Check that exactly one do-all is suggested"""
         test_output_file = os.path.join(src_dir, ".discopop", "explorer", "detection_result_dump.json")
-        # load both detection results
-        with open(gold_standard_file, "r") as f:
-            tmp_str = f.read()
-        gold_standard: DetectionResult = jsonpickle.decode(tmp_str)
-
+        # load detection results
         with open(test_output_file, "r") as f:
             tmp_str = f.read()
         test_output: DetectionResult = jsonpickle.decode(tmp_str)
 
-        # convert DoAllInfo objects to DoAllInfoForValidation objects to make use of custom __eq__
-        converted_gold_standard = [DoAllInfoForValidation(elem) for elem in gold_standard.do_all]
-        converted_test_output = [DoAllInfoForValidation(elem) for elem in test_output.patterns.do_all]
-
-        # sort the lists
-        converted_gold_standard = sorted(
-            converted_gold_standard, key=lambda x: (x.dai.node_id, x.dai.start_line, x.dai.end_line)
-        )
-        converted_test_output = sorted(
-            converted_test_output, key=lambda x: (x.dai.node_id, x.dai.start_line, x.dai.end_line)
-        )
-
-        # compare doall list elements
-        self.assertListEqual(converted_gold_standard, converted_test_output)
+        for pattern_type in test_output.patterns.__dict__:
+            amount_of_identified_patterns = len(test_output.patterns.__dict__[pattern_type])
+            if pattern_type == "do_all":
+                self.assertEqual(amount_of_identified_patterns, 0)
+            elif pattern_type == "reduction":
+                self.assertEqual(amount_of_identified_patterns, 1)
+            else:
+                self.assertEqual(amount_of_identified_patterns, 0)
```

