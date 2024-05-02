# Comparing `tmp/vivarium-core-1.6.3.tar.gz` & `tmp/vivarium-core-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vivarium-core-1.6.3.tar", last modified: Wed Feb 21 16:50:11 2024, max compression
+gzip compressed data, was "vivarium-core-1.6.4.tar", last modified: Thu May  2 15:22:27 2024, max compression
```

## Comparing `vivarium-core-1.6.3.tar` & `vivarium-core-1.6.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.116366 vivarium-core-1.6.3/
--rw-r--r--   0 eranagmon   (503) staff       (20)      733 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/AUTHORS.md
--rw-r--r--   0 eranagmon   (503) staff       (20)    11357 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/LICENSE.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)     5690 2024-02-21 16:50:11.116204 vivarium-core-1.6.3/PKG-INFO
--rw-r--r--   0 eranagmon   (503) staff       (20)     4124 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/README.md
--rw-r--r--   0 eranagmon   (503) staff       (20)       38 2024-02-21 16:50:11.116421 vivarium-core-1.6.3/setup.cfg
--rw-r--r--   0 eranagmon   (503) staff       (20)     2837 2024-02-21 16:04:20.000000 vivarium-core-1.6.3/setup.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.102918 vivarium-core-1.6.3/vivarium/
--rw-r--r--   0 eranagmon   (503) staff       (20)     4085 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/__init__.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.103486 vivarium-core-1.6.3/vivarium/composites/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/composites/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1369 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/composites/injected_glc_phosphorylation.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    30344 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/composites/toys.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.106862 vivarium-core-1.6.3/vivarium/core/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    19080 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/composer.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    12242 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/core/composition.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     9130 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/core/control.py
--rw-r--r--   0 eranagmon   (503) staff       (20)      394 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/directories.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    28121 2024-02-21 16:04:20.000000 vivarium-core-1.6.3/vivarium/core/emitter.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    50852 2024-02-21 16:49:48.000000 vivarium-core-1.6.3/vivarium/core/engine.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    33464 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/process.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    13878 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/registry.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    10337 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/serialize.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     7123 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/serialize_test.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    73759 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/core/store.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1588 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/core/types.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.108786 vivarium-core-1.6.3/vivarium/experiments/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2823 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/bigraph_view.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1005 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/composite_merge.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    38709 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/engine_tests.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2663 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/glucose_phosphorylation.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3488 2024-02-21 16:04:20.000000 vivarium-core-1.6.3/vivarium/experiments/hierarchy_composite_division.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     6225 2024-02-21 16:04:20.000000 vivarium-core-1.6.3/vivarium/experiments/large_experiment.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2955 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/profile_image.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    20995 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/profile_runtime.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     8675 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/experiments/store_api.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1429 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/experiments/test_profiler.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.110580 vivarium-core-1.6.3/vivarium/library/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1897 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/datum.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    12837 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/library/dict_utils.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3255 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/filepath.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     5183 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/make_network.py
--rw-r--r--   0 eranagmon   (503) staff       (20)      145 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/path.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1803 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/pretty.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1789 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/schema.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    11820 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/timeseries.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    11352 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/topology.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2948 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/units.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2209 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/library/wrappers.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.111158 vivarium-core-1.6.3/vivarium/plots/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/plots/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    11417 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/plots/agents_multigen.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    11493 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/plots/simulation_output.py
--rw-r--r--   0 eranagmon   (503) staff       (20)    26041 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/plots/topology.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.115228 vivarium-core-1.6.3/vivarium/processes/
--rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/__init__.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     6181 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/alternator.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     5078 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/burst.py
--rw-r--r--   0 eranagmon   (503) staff       (20)      538 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/clock.py
--rw-r--r--   0 eranagmon   (503) staff       (20)      949 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/divide_condition.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2413 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/division.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     5749 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/ecoli_shape_deriver.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     5137 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/engulf.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3480 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/glucose_phosphorylation.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3158 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/growth_rate.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3235 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/injector.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     6894 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/mass_adaptor.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     6784 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/meta_division.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3421 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/molarity_deriver.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     2432 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/nonspatial_environment.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3304 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/remove.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     1403 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/strip_units.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     5618 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/swap_processes.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3745 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/template_process.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     3260 2023-08-28 17:56:00.000000 vivarium-core-1.6.3/vivarium/processes/timeline.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     7857 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/toy_gillespie.py
--rw-r--r--   0 eranagmon   (503) staff       (20)     4657 2023-12-05 15:07:42.000000 vivarium-core-1.6.3/vivarium/processes/tree_mass.py
-drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-02-21 16:50:11.115948 vivarium-core-1.6.3/vivarium_core.egg-info/
--rw-r--r--   0 eranagmon   (503) staff       (20)     5690 2024-02-21 16:50:11.000000 vivarium-core-1.6.3/vivarium_core.egg-info/PKG-INFO
--rw-r--r--   0 eranagmon   (503) staff       (20)     2408 2024-02-21 16:50:11.000000 vivarium-core-1.6.3/vivarium_core.egg-info/SOURCES.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)        1 2024-02-21 16:50:11.000000 vivarium-core-1.6.3/vivarium_core.egg-info/dependency_links.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)       20 2024-02-21 16:50:11.000000 vivarium-core-1.6.3/vivarium_core.egg-info/entry_points.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)      115 2024-02-21 16:50:11.000000 vivarium-core-1.6.3/vivarium_core.egg-info/requires.txt
--rw-r--r--   0 eranagmon   (503) staff       (20)        9 2024-02-21 16:50:11.000000 vivarium-core-1.6.3/vivarium_core.egg-info/top_level.txt
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.239302 vivarium-core-1.6.4/
+-rw-r--r--   0 eranagmon   (503) staff       (20)      733 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/AUTHORS.md
+-rw-r--r--   0 eranagmon   (503) staff       (20)    11357 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/LICENSE.txt
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5690 2024-05-02 15:22:27.239153 vivarium-core-1.6.4/PKG-INFO
+-rw-r--r--   0 eranagmon   (503) staff       (20)     4124 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/README.md
+-rw-r--r--   0 eranagmon   (503) staff       (20)       38 2024-05-02 15:22:27.239349 vivarium-core-1.6.4/setup.cfg
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2837 2024-05-02 15:17:26.000000 vivarium-core-1.6.4/setup.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.222203 vivarium-core-1.6.4/vivarium/
+-rw-r--r--   0 eranagmon   (503) staff       (20)     4085 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/__init__.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.222800 vivarium-core-1.6.4/vivarium/composites/
+-rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/composites/__init__.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1369 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/composites/injected_glc_phosphorylation.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    30344 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/composites/toys.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.227415 vivarium-core-1.6.4/vivarium/core/
+-rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/__init__.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    19080 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/composer.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    12242 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/core/composition.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     9130 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/core/control.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)      394 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/directories.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    28121 2024-02-21 16:04:20.000000 vivarium-core-1.6.4/vivarium/core/emitter.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    50852 2024-02-21 16:49:48.000000 vivarium-core-1.6.4/vivarium/core/engine.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    33464 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/process.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    13878 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/registry.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    10337 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/serialize.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     7123 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/serialize_test.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    73759 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/core/store.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1588 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/core/types.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.230180 vivarium-core-1.6.4/vivarium/experiments/
+-rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/__init__.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2823 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/bigraph_view.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1005 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/composite_merge.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    38709 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/engine_tests.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2663 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/glucose_phosphorylation.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3488 2024-02-21 16:04:20.000000 vivarium-core-1.6.4/vivarium/experiments/hierarchy_composite_division.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     6225 2024-02-21 16:04:20.000000 vivarium-core-1.6.4/vivarium/experiments/large_experiment.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2955 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/profile_image.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    20995 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/profile_runtime.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     8675 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/experiments/store_api.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1429 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/experiments/test_profiler.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.232457 vivarium-core-1.6.4/vivarium/library/
+-rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/__init__.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1897 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/datum.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    12837 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/library/dict_utils.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3255 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/filepath.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5183 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/make_network.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)      145 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/path.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1803 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/pretty.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1789 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/schema.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    11820 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/timeseries.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    11352 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/topology.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2867 2024-05-02 15:01:23.000000 vivarium-core-1.6.4/vivarium/library/units.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2209 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/library/wrappers.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.233151 vivarium-core-1.6.4/vivarium/plots/
+-rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/plots/__init__.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    11417 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/plots/agents_multigen.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    11493 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/plots/simulation_output.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)    26041 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/plots/topology.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.237752 vivarium-core-1.6.4/vivarium/processes/
+-rw-r--r--   0 eranagmon   (503) staff       (20)        0 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/__init__.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     6181 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/alternator.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5078 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/burst.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)      538 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/clock.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)      949 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/divide_condition.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2413 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/division.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5749 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/ecoli_shape_deriver.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5137 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/engulf.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3480 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/glucose_phosphorylation.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3158 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/growth_rate.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3235 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/injector.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     6894 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/mass_adaptor.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     6784 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/meta_division.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3421 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/molarity_deriver.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2432 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/nonspatial_environment.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3304 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/remove.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     1403 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/strip_units.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5618 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/swap_processes.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3745 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/template_process.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     3260 2023-08-28 17:56:00.000000 vivarium-core-1.6.4/vivarium/processes/timeline.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     7857 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/toy_gillespie.py
+-rw-r--r--   0 eranagmon   (503) staff       (20)     4657 2023-12-05 15:07:42.000000 vivarium-core-1.6.4/vivarium/processes/tree_mass.py
+drwxr-xr-x   0 eranagmon   (503) staff       (20)        0 2024-05-02 15:22:27.238938 vivarium-core-1.6.4/vivarium_core.egg-info/
+-rw-r--r--   0 eranagmon   (503) staff       (20)     5690 2024-05-02 15:22:27.000000 vivarium-core-1.6.4/vivarium_core.egg-info/PKG-INFO
+-rw-r--r--   0 eranagmon   (503) staff       (20)     2408 2024-05-02 15:22:27.000000 vivarium-core-1.6.4/vivarium_core.egg-info/SOURCES.txt
+-rw-r--r--   0 eranagmon   (503) staff       (20)        1 2024-05-02 15:22:27.000000 vivarium-core-1.6.4/vivarium_core.egg-info/dependency_links.txt
+-rw-r--r--   0 eranagmon   (503) staff       (20)       20 2024-05-02 15:22:27.000000 vivarium-core-1.6.4/vivarium_core.egg-info/entry_points.txt
+-rw-r--r--   0 eranagmon   (503) staff       (20)      115 2024-05-02 15:22:27.000000 vivarium-core-1.6.4/vivarium_core.egg-info/requires.txt
+-rw-r--r--   0 eranagmon   (503) staff       (20)        9 2024-05-02 15:22:27.000000 vivarium-core-1.6.4/vivarium_core.egg-info/top_level.txt
```

### Comparing `vivarium-core-1.6.3/AUTHORS.md` & `vivarium-core-1.6.4/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/LICENSE.txt` & `vivarium-core-1.6.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/PKG-INFO` & `vivarium-core-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-core
-Version: 1.6.3
+Version: 1.6.4
 Summary: Engine for composing and simulating computational biology models with the Vivarium interface.
 Home-page: https://github.com/vivarium-collective/vivarium-core
 Author: Eran Agmon, Ryan Spangler
 Author-email: eagmon@stanford.edu, ryan.spangler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/vivarium-collective/vivarium-core
 Project-URL: Documentation, https://vivarium-core.readthedocs.io/en/latest/
```

### Comparing `vivarium-core-1.6.3/README.md` & `vivarium-core-1.6.4/README.md`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/setup.py` & `vivarium-core-1.6.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import re
 from setuptools import setup
 
 
-VERSION = '1.6.3'
+VERSION = '1.6.4'
 
 
 if __name__ == '__main__':
     with open("README.md", 'r') as readme:
         description = readme.read()
         # Patch the relative links to absolute URLs that will work on PyPI.
         description2 = re.sub(
@@ -50,15 +50,15 @@
         package_data={},
         include_package_data=True,
         python_requires='>=3.9, <3.12',
         install_requires=[
             'matplotlib>=3.5.1',
             'networkx>=2.6.3',
             'numpy>=1.22.1',
-            'Pint>=0.18',
+            'Pint>=0.23',
             'pymongo>=4.0.1',
             'scipy>=1.7.3',
             'pytest>=6.2.5',
             'orjson>=3.8.0'
         ],
         classifiers=[
             'Development Status :: 4 - Beta',
```

### Comparing `vivarium-core-1.6.3/vivarium/__init__.py` & `vivarium-core-1.6.4/vivarium/__init__.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/composites/injected_glc_phosphorylation.py` & `vivarium-core-1.6.4/vivarium/composites/injected_glc_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/composites/toys.py` & `vivarium-core-1.6.4/vivarium/composites/toys.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/composer.py` & `vivarium-core-1.6.4/vivarium/core/composer.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/composition.py` & `vivarium-core-1.6.4/vivarium/core/composition.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/control.py` & `vivarium-core-1.6.4/vivarium/core/control.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/emitter.py` & `vivarium-core-1.6.4/vivarium/core/emitter.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/engine.py` & `vivarium-core-1.6.4/vivarium/core/engine.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/process.py` & `vivarium-core-1.6.4/vivarium/core/process.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/registry.py` & `vivarium-core-1.6.4/vivarium/core/registry.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/serialize.py` & `vivarium-core-1.6.4/vivarium/core/serialize.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/serialize_test.py` & `vivarium-core-1.6.4/vivarium/core/serialize_test.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/store.py` & `vivarium-core-1.6.4/vivarium/core/store.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/core/types.py` & `vivarium-core-1.6.4/vivarium/core/types.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/bigraph_view.py` & `vivarium-core-1.6.4/vivarium/experiments/bigraph_view.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/composite_merge.py` & `vivarium-core-1.6.4/vivarium/experiments/composite_merge.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/engine_tests.py` & `vivarium-core-1.6.4/vivarium/experiments/engine_tests.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/glucose_phosphorylation.py` & `vivarium-core-1.6.4/vivarium/experiments/glucose_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/hierarchy_composite_division.py` & `vivarium-core-1.6.4/vivarium/experiments/hierarchy_composite_division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/large_experiment.py` & `vivarium-core-1.6.4/vivarium/experiments/large_experiment.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/profile_image.py` & `vivarium-core-1.6.4/vivarium/experiments/profile_image.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/profile_runtime.py` & `vivarium-core-1.6.4/vivarium/experiments/profile_runtime.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/store_api.py` & `vivarium-core-1.6.4/vivarium/experiments/store_api.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/experiments/test_profiler.py` & `vivarium-core-1.6.4/vivarium/experiments/test_profiler.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/datum.py` & `vivarium-core-1.6.4/vivarium/library/datum.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/dict_utils.py` & `vivarium-core-1.6.4/vivarium/library/dict_utils.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/filepath.py` & `vivarium-core-1.6.4/vivarium/library/filepath.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/make_network.py` & `vivarium-core-1.6.4/vivarium/library/make_network.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/pretty.py` & `vivarium-core-1.6.4/vivarium/library/pretty.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/schema.py` & `vivarium-core-1.6.4/vivarium/library/schema.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/timeseries.py` & `vivarium-core-1.6.4/vivarium/library/timeseries.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/topology.py` & `vivarium-core-1.6.4/vivarium/library/topology.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/library/units.py` & `vivarium-core-1.6.4/vivarium/library/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,18 +22,15 @@
 
 from typing import Any
 
 import pint
 
 # noinspection PyProtectedMember
 from pint import Unit
-try:
-    from pint.quantity import _Quantity as Quantity
-except ImportError:
-    from pint import Quantity
+from pint import Quantity
 
 #: Units registry that stores the units used throughout Vivarium
 units = pint.UnitRegistry()
 
 # We need to set this registry as the default application-wide so our
 # registry will be used when unpickling
 pint.set_application_registry(units)
```

### Comparing `vivarium-core-1.6.3/vivarium/library/wrappers.py` & `vivarium-core-1.6.4/vivarium/library/wrappers.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/plots/agents_multigen.py` & `vivarium-core-1.6.4/vivarium/plots/agents_multigen.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/plots/simulation_output.py` & `vivarium-core-1.6.4/vivarium/plots/simulation_output.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/plots/topology.py` & `vivarium-core-1.6.4/vivarium/plots/topology.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/alternator.py` & `vivarium-core-1.6.4/vivarium/processes/alternator.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/burst.py` & `vivarium-core-1.6.4/vivarium/processes/burst.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/clock.py` & `vivarium-core-1.6.4/vivarium/processes/clock.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/divide_condition.py` & `vivarium-core-1.6.4/vivarium/processes/divide_condition.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/division.py` & `vivarium-core-1.6.4/vivarium/processes/division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/ecoli_shape_deriver.py` & `vivarium-core-1.6.4/vivarium/processes/ecoli_shape_deriver.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/engulf.py` & `vivarium-core-1.6.4/vivarium/processes/engulf.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/glucose_phosphorylation.py` & `vivarium-core-1.6.4/vivarium/processes/glucose_phosphorylation.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/growth_rate.py` & `vivarium-core-1.6.4/vivarium/processes/growth_rate.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/injector.py` & `vivarium-core-1.6.4/vivarium/processes/injector.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/mass_adaptor.py` & `vivarium-core-1.6.4/vivarium/processes/mass_adaptor.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/meta_division.py` & `vivarium-core-1.6.4/vivarium/processes/meta_division.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/molarity_deriver.py` & `vivarium-core-1.6.4/vivarium/processes/molarity_deriver.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/nonspatial_environment.py` & `vivarium-core-1.6.4/vivarium/processes/nonspatial_environment.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/remove.py` & `vivarium-core-1.6.4/vivarium/processes/remove.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/strip_units.py` & `vivarium-core-1.6.4/vivarium/processes/strip_units.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/swap_processes.py` & `vivarium-core-1.6.4/vivarium/processes/swap_processes.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/template_process.py` & `vivarium-core-1.6.4/vivarium/processes/template_process.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/timeline.py` & `vivarium-core-1.6.4/vivarium/processes/timeline.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/toy_gillespie.py` & `vivarium-core-1.6.4/vivarium/processes/toy_gillespie.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium/processes/tree_mass.py` & `vivarium-core-1.6.4/vivarium/processes/tree_mass.py`

 * *Files identical despite different names*

### Comparing `vivarium-core-1.6.3/vivarium_core.egg-info/PKG-INFO` & `vivarium-core-1.6.4/vivarium_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vivarium-core
-Version: 1.6.3
+Version: 1.6.4
 Summary: Engine for composing and simulating computational biology models with the Vivarium interface.
 Home-page: https://github.com/vivarium-collective/vivarium-core
 Author: Eran Agmon, Ryan Spangler
 Author-email: eagmon@stanford.edu, ryan.spangler@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/vivarium-collective/vivarium-core
 Project-URL: Documentation, https://vivarium-core.readthedocs.io/en/latest/
```

### Comparing `vivarium-core-1.6.3/vivarium_core.egg-info/SOURCES.txt` & `vivarium-core-1.6.4/vivarium_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

