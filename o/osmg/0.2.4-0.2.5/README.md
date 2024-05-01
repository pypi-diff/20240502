# Comparing `tmp/osmg-0.2.4.tar.gz` & `tmp/osmg-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmg-0.2.4.tar", last modified: Tue Feb 20 14:54:06 2024, max compression
+gzip compressed data, was "osmg-0.2.5.tar", last modified: Wed May  1 22:19:13 2024, max compression
```

## Comparing `osmg-0.2.4.tar` & `osmg-0.2.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.017577 osmg-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-20 14:53:54.000000 osmg-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-02-20 14:53:54.000000 osmg-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-20 14:54:06.017577 osmg-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-02-20 14:53:54.000000 osmg-0.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-02-20 14:53:54.000000 osmg-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-02-20 14:54:06.017577 osmg-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-20 14:53:54.000000 osmg-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.005576 osmg-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.009576 osmg-0.2.4/src/osmg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     3672 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/component_assembly.py
--rw-r--r--   0 runner    (1001) docker     (127)     4287 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.013576 osmg-0.2.4/src/osmg/gen/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    54817 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/component_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    16317 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/material_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/mesh_shapes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/node_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)     8500 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    16124 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/section_gen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.013576 osmg-0.2.4/src/osmg/gen/steel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/steel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/steel/brb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/uid_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    21086 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/gen/zerolength_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/get_latest_pypi_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.013576 osmg-0.2.4/src/osmg/graphics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/general_2d.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/graphics_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/graphics_common_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    66172 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/postprocessing_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)    41472 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/preprocessing_3d.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/graphics/visibility.py
--rw-r--r--   0 runner    (1001) docker     (127)     4521 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/ground_motion_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/line.py
--rw-r--r--   0 runner    (1001) docker     (127)     9439 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/load_case.py
--rw-r--r--   0 runner    (1001) docker     (127)    34729 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/mesh.py
--rw-r--r--   0 runner    (1001) docker     (127)    13315 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/obj_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.013576 osmg-0.2.4/src/osmg/ops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12617 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/ops/element.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/ops/node.py
--rw-r--r--   0 runner    (1001) docker     (127)     9044 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/ops/section.py
--rw-r--r--   0 runner    (1001) docker     (127)    14188 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/ops/uniaxial_material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/physical_material.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.013576 osmg-0.2.4/src/osmg/postprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/postprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/postprocessing/basic_forces.py
--rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/postprocessing/design.py
--rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/postprocessing/steel_design_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.013576 osmg-0.2.4/src/osmg/preprocessing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/preprocessing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/preprocessing/rigid_diaphragm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/preprocessing/self_weight_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     6614 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/preprocessing/split_component.py
--rw-r--r--   0 runner    (1001) docker     (127)    21768 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/preprocessing/tributary_area_analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   450065 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/sections.json
--rw-r--r--   0 runner    (1001) docker     (127)    93487 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/solver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-02-20 14:53:54.000000 osmg-0.2.4/src/osmg/transformations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-20 14:54:06.017577 osmg-0.2.4/src/osmg.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-02-20 14:54:05.000000 osmg-0.2.4/src/osmg.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-02-20 14:54:05.000000 osmg-0.2.4/src/osmg.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 14:54:05.000000 osmg-0.2.4/src/osmg.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-20 14:54:05.000000 osmg-0.2.4/src/osmg.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-02-20 14:54:05.000000 osmg-0.2.4/src/osmg.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-20 14:54:05.000000 osmg-0.2.4/src/osmg.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:13.003150 osmg-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 22:19:03.000000 osmg-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-01 22:19:03.000000 osmg-0.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 22:19:13.003150 osmg-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-01 22:19:03.000000 osmg-0.2.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-01 22:19:03.000000 osmg-0.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-01 22:19:13.003150 osmg-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-01 22:19:03.000000 osmg-0.2.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:12.991150 osmg-0.2.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:12.995150 osmg-0.2.5/src/osmg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/component_assembly.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:12.999150 osmg-0.2.5/src/osmg/gen/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54732 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/component_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16497 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/material_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/mesh_shapes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/node_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8593 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16086 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/section_gen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:12.999150 osmg-0.2.5/src/osmg/gen/steel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/steel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6477 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/steel/brb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/uid_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21131 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/gen/zerolength_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/get_latest_pypi_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:12.999150 osmg-0.2.5/src/osmg/graphics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4569 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/general_2d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/graphics_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/graphics_common_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    67032 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/postprocessing_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41699 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/preprocessing_3d.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/graphics/visibility.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4433 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/ground_motion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7382 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/line.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9421 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/load_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34696 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13288 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8766 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/obj_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:13.003150 osmg-0.2.5/src/osmg/ops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12615 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/ops/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/ops/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/ops/section.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14109 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/ops/uniaxial_material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/physical_material.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:13.003150 osmg-0.2.5/src/osmg/postprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/postprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3084 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/postprocessing/basic_forces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4524 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/postprocessing/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4905 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/postprocessing/steel_design_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:13.003150 osmg-0.2.5/src/osmg/preprocessing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/preprocessing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/preprocessing/rigid_diaphragm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2925 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/preprocessing/self_weight_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/preprocessing/split_component.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22027 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/preprocessing/tributary_area_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   450065 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/sections.json
+-rw-r--r--   0 runner    (1001) docker     (127)    92561 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/solver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8348 2024-05-01 22:19:03.000000 osmg-0.2.5/src/osmg/transformations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:19:13.003150 osmg-0.2.5/src/osmg.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-01 22:19:12.000000 osmg-0.2.5/src/osmg.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-05-01 22:19:12.000000 osmg-0.2.5/src/osmg.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:19:12.000000 osmg-0.2.5/src/osmg.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:19:12.000000 osmg-0.2.5/src/osmg.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-01 22:19:12.000000 osmg-0.2.5/src/osmg.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 22:19:12.000000 osmg-0.2.5/src/osmg.egg-info/top_level.txt
```

### Comparing `osmg-0.2.4/LICENSE` & `osmg-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/PKG-INFO` & `osmg-0.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmg
-Version: 0.2.4
+Version: 0.2.5
 Summary: OpenSees Model Generator
 Home-page: https://github.com/ioannis-vm/OpenSees_Model_Generator
 Author: John Vouvakis Manousakis
 License: GPL
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `osmg-0.2.4/README.md` & `osmg-0.2.5/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # OpenSees Model Generator
-![Tests](https://github.com/ioannis-vm/OpenSees_Model_Generator/actions/workflows/test_and_deploy.yaml/badge.svg)
+![Tests](https://github.com/ioannis-vm/OpenSees_Model_Generator/actions/workflows/test.yaml/badge.svg)
 ![PyPI version](https://badge.fury.io/py/osmg.svg)
 ![Zenodo](https://zenodo.org/badge/DOI/10.5281/zenodo.7536062.svg)
 
 ![](img/img.png)
 
 This Python package aims to help users define, analyze, and post-process 3D models using OpenSees. `osmg` is utilizing the Python interpreter of OpenSees. Anyone is free and welcome to use, fork, extend and redistribute the code.
```

### Comparing `osmg-0.2.4/pyproject.toml` & `osmg-0.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/setup.cfg` & `osmg-0.2.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = osmg
-version = 0.2.4
+version = 0.2.5
 url = https://github.com/ioannis-vm/OpenSees_Model_Generator
 description = OpenSees Model Generator
 long_description = OpenSees Model Generator
 long_description_content_type = text/x-rst
 author = John Vouvakis Manousakis
 license = GPL
 license_files = LICENSE
```

### Comparing `osmg-0.2.4/src/osmg/common.py` & `osmg-0.2.5/src/osmg/common.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/component_assembly.py` & `osmg-0.2.5/src/osmg/component_assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,17 +57,15 @@
     elements: (
         obj_collections.CollectionWithConnectivity[int, element.Element]
     ) = field(init=False)
 
     def __post_init__(self):
         self.external_nodes = obj_collections.NodeCollection(self)
         self.internal_nodes = obj_collections.NodeCollection(self)
-        self.elements = (
-            obj_collections.CollectionWithConnectivity(self)
-        )
+        self.elements = obj_collections.CollectionWithConnectivity(self)
 
     def __srepr__(self):
         """
         Short version of repr
         """
         return f"Component assembly, uid: {self.uid}"
```

### Comparing `osmg-0.2.4/src/osmg/defaults.py` & `osmg-0.2.5/src/osmg/defaults.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,18 +62,15 @@
 
     """
 
     # intantiate a section generator object for the model
     sgen = SectionGenerator(model)
     # generate a default elastic section and add it to the model
     sgen.generate_generic_elastic(
-        name=sec_name,
-        e_times_a=1.00,
-        e_times_i=1.00,
-        g_times_j=1.00
+        name=sec_name, e_times_a=1.00, e_times_i=1.00, g_times_j=1.00
     )
 
 
 def load_default_steel(model: Model) -> None:
     """
     Adds a default steel material to the model.
```

### Comparing `osmg-0.2.4/src/osmg/gen/component_gen.py` & `osmg-0.2.5/src/osmg/gen/component_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,16 +52,20 @@
     from ..level import Level
 
 
 nparr = npt.NDArray[np.float64]
 
 
 def retrieve_snap_pt_global_offset(
-        placement: str, section: ElasticSection | FiberSection,
-        p_i: nparr, p_j: nparr, angle: float) -> nparr:
+    placement: str,
+    section: ElasticSection | FiberSection,
+    p_i: nparr,
+    p_j: nparr,
+    angle: float,
+) -> nparr:
     """
     Returns the necessary offset to connect an element at a specified
     snap point of the section.
 
     Arguments:
       placement: Placement tag. Can be any of "centroid",
         "top_center", "top_left", "top_right", "center_left",
@@ -146,17 +150,15 @@
                     "top_right",
                     "center_left",
                     "center_right",
                     "bottom_center",
                     "bottom_left",
                     "bottom_right",
                 ]:
-                    elm = component.elements.named_contents[
-                        "elm_interior"
-                    ]
+                    elm = component.elements.named_contents["elm_interior"]
                     d_z, d_y = elm.section.snap_points[snap]
                     sec_offset_local: nparr = -np.array([0.00, d_y, d_z])
                     # retrieve local coordinate system
                     x_axis = elm.geomtransf.x_axis
                     y_axis = elm.geomtransf.y_axis
                     z_axis = elm.geomtransf.z_axis
                     t_glob_to_loc = transformation_matrix(
@@ -194,15 +196,16 @@
                             y_axis = elm.geomtransf.y_axis
                             z_axis = elm.geomtransf.z_axis
                             t_glob_to_loc = transformation_matrix(
                                 x_axis, y_axis, z_axis
                             )
                             t_loc_to_glob = t_glob_to_loc.T
                             sec_offset_global = (
-                                t_loc_to_glob @ sec_offset_local)
+                                t_loc_to_glob @ sec_offset_local
+                            )
                             e_o += sec_offset_global
     return node, e_o
 
 
 def look_for_panel_zone(node: Node, lvl: Level, query: ElmQuery) -> Node:
     """
     Determines if a panel zone joint component assembly is present
@@ -228,33 +231,33 @@
     Bar elements are linear elements that can only carry axial load.
 
     """
 
     model: Model = field(repr=False)
 
     def add(
-            self,
-            xi_coord: float,
-            yi_coord: float,
-            lvl_key_i: int,
-            offset_i: nparr,
-            snap_i: str,
-            xj_coord: float,
-            yj_coord: float,
-            lvl_key_j: int,
-            offset_j: nparr,
-            snap_j: str,
-            transf_type: str,
-            area: float,
-            mat: UniaxialMaterial,
-            outside_shape: Mesh,
-            weight_per_length: float = 0.00,
-            split_existing_i: bool = None,
-            split_existing_j: bool = None,
-            component_purpose: str = 'Truss Element'
+        self,
+        xi_coord: float,
+        yi_coord: float,
+        lvl_key_i: int,
+        offset_i: nparr,
+        snap_i: str,
+        xj_coord: float,
+        yj_coord: float,
+        lvl_key_j: int,
+        offset_j: nparr,
+        snap_j: str,
+        transf_type: str,
+        area: float,
+        mat: UniaxialMaterial,
+        outside_shape: Mesh,
+        weight_per_length: float = 0.00,
+        split_existing_i: bool = None,
+        split_existing_j: bool = None,
+        component_purpose: str = 'Truss Element',
     ) -> ComponentAssembly:
         """
         Adds a truss bar element.
         If offsets are required, they are implemented through the
         addition of RigidLink elements.
 
         """
@@ -298,20 +301,18 @@
         # the brace to be located at the coordinates we specify, which
         # is different to what is done with the connectivity of beams.
         # Therefore, if the coordinates of the returned nodes differ
         # with those that we specified, we add the difference in the
         # offset, to move the ends of the brace back where we want
         # them to be. The effect of this is that the rigid offsets
         # (twonodelinks) will connect to that other node.
-        i_diff = (np.array((xi_coord, yi_coord))
-                  - np.array(node_i.coords[0:2]))
+        i_diff = np.array((xi_coord, yi_coord)) - np.array(node_i.coords[0:2])
         if np.linalg.norm(i_diff) > common.EPSILON:
             eo_i[0:2] += i_diff
-        j_diff = (np.array((xj_coord, yj_coord))
-                  - np.array(node_j.coords[0:2]))
+        j_diff = np.array((xj_coord, yj_coord)) - np.array(node_j.coords[0:2])
         if np.linalg.norm(j_diff) > common.EPSILON:
             eo_j[0:2] += j_diff
 
         # instantiate a component assembly
         component = ComponentAssembly(
             uid=self.model.uid_generator.new("component"),
             parent_collection=lvl_i.components,
@@ -319,60 +320,63 @@
         )
         # add it to the level
         lvl_i.components.add(component)
         # fill component assembly
         component.external_nodes.add(node_i)
         component.external_nodes.add(node_j)
 
-        def prepare_connection(
-                node_x: Node, eo_x: nparr) \
-                -> Node:
+        def prepare_connection(node_x: Node, eo_x: nparr) -> Node:
             """
             For each end of the bar element, creates a rigid link if
             an offset exists, and returns the node to which the bar
             element should connect to. This function is called twice,
             once for the i-end and once for the j-end.  For purposes
             of clarity, the index x will be used here, assuming that
             it will be substituted with i and j.
             """
 
             # if there is an offset at the x-end, create an internal node
             # and add a rigidlink element to the component assembly
             if np.linalg.norm(eo_x) > common.EPSILON:
                 int_node_x = Node(
                     self.model.uid_generator.new('node'),
-                    [*(np.array(node_x.coords) + eo_x)]
+                    [*(np.array(node_x.coords) + eo_x)],
                 )
                 component.internal_nodes.add(int_node_x)
                 n_x = int_node_x
                 dirs, mats = zerolength_gen.fix_all(self.model)
                 # flip the nodes if the element is about to be defined
                 # upside down
-                if np.allclose(
+                if (
+                    np.allclose(
                         np.array(node_x.coords[0:2]),
                         np.array(int_node_x.coords[0:2]),
-                ) and int_node_x.coords[2] > node_x.coords[2]:
+                    )
+                    and int_node_x.coords[2] > node_x.coords[2]
+                ):
                     x_axis, y_axis, _ = local_axes_from_points_and_angle(
                         np.array(int_node_x.coords),
                         np.array(node_x.coords),
-                        0.00)
+                        0.00,
+                    )
                     elm_link = TwoNodeLink(
                         component,
                         self.model.uid_generator.new("element"),
                         [node_x, int_node_x],
                         mats,
                         dirs,
                         x_axis,
                         y_axis,
                     )
                 else:
                     x_axis, y_axis, _ = local_axes_from_points_and_angle(
                         np.array(node_x.coords),
                         np.array(int_node_x.coords),
-                        0.00)
+                        0.00,
+                    )
                     elm_link = TwoNodeLink(
                         component,
                         self.model.uid_generator.new("element"),
                         [node_x, int_node_x],
                         mats,
                         dirs,
                         x_axis,
@@ -392,15 +396,15 @@
             parent_component=component,
             uid=self.model.uid_generator.new("element"),
             nodes=[n_i, n_j],
             transf_type=transf_type,
             area=area,
             mat=mat,
             outside_shape=outside_shape,
-            weight_per_length=weight_per_length
+            weight_per_length=weight_per_length,
         )
 
         # add it to the component assembly
         component.elements.add(elm_truss)
 
         return component
 
@@ -411,26 +415,26 @@
     Introduces beamcolumn elements to a model.
 
     """
 
     model: Model = field(repr=False)
 
     def define_beamcolumn(
-            self,
-            assembly: ComponentAssembly,
-            node_i: Node,
-            node_j: Node,
-            offset_i: nparr,
-            offset_j: nparr,
-            transf_type: str,
-            section: ElasticSection | FiberSection,
-            element_type: Type[Union[ElasticBeamColumn, DispBeamColumn]],
-            angle: float = 0.00,
-            n_x: Optional[float] = None,
-            n_y: Optional[float] = None
+        self,
+        assembly: ComponentAssembly,
+        node_i: Node,
+        node_j: Node,
+        offset_i: nparr,
+        offset_j: nparr,
+        transf_type: str,
+        section: ElasticSection | FiberSection,
+        element_type: Type[Union[ElasticBeamColumn, DispBeamColumn]],
+        angle: float = 0.00,
+        n_x: Optional[float] = None,
+        n_y: Optional[float] = None,
     ) -> ElasticBeamColumn | DispBeamColumn:
         """
         Adds a beamcolumn element to the model, connecting the
         specified nodes.
 
         """
 
@@ -450,15 +454,16 @@
             )
             elm_el = ElasticBeamColumn(
                 parent_component=assembly,
                 uid=self.model.uid_generator.new("element"),
                 nodes=[node_i, node_j],
                 section=section,
                 geomtransf=transf,
-                n_x=n_x, n_y=n_y
+                n_x=n_x,
+                n_y=n_y,
             )
             res: Union[ElasticBeamColumn, DispBeamColumn] = elm_el
         elif element_type.__name__ == "DispBeamColumn":
             assert isinstance(section, FiberSection)
             assert n_x is None
             assert n_y is None
             # TODO: add elastic section support
@@ -480,16 +485,15 @@
                 nodes=[node_i, node_j],
                 section=section,
                 geomtransf=transf,
                 integration=beam_integration,
             )
             res = elm_disp
         else:
-            raise ValueError(
-                'Invalid element type: {element_type.__name__}')
+            raise ValueError('Invalid element type: {element_type.__name__}')
         return res
 
     def define_zerolength(
         self,
         assembly: ComponentAssembly,
         node_i: Node,
         node_j: Node,
@@ -553,15 +557,15 @@
         transf_type,
         section,
         element_type,
         angle,
         camber_2,
         camber_3,
         n_x=None,
-        n_y=None
+        n_y=None,
     ):
         """
         Adds beamcolumn elemens in series.
 
         """
 
         if (n_x is not None) or (n_y is not None):
@@ -612,29 +616,32 @@
             if i == n_sub - 1:
                 n_j = node_j
                 o_j = eo_j
             else:
                 n_j = intnodes[i]
                 o_j = np.zeros(3)
             if element_type.__name__ not in {
-                    'ElasticBeamColumn', 'DispBeamColumn'}:
+                'ElasticBeamColumn',
+                'DispBeamColumn',
+            }:
                 raise TypeError(
-                    "Unsupported element type:" f" {element_type.__name__}"
+                    f"Unsupported element type: {element_type.__name__}"
                 )
             element = self.define_beamcolumn(
                 assembly=component,
                 node_i=n_i,
                 node_j=n_j,
                 offset_i=o_i,
                 offset_j=o_j,
                 transf_type=transf_type,
                 section=section,
                 element_type=element_type,
                 angle=angle,
-                n_x=n_x, n_y=n_y
+                n_x=n_x,
+                n_y=n_y,
             )
             component.elements.add(element)
 
     def generate_plain_component_assembly(
         self,
         component_purpose,
         lvl,
@@ -646,15 +653,15 @@
         section,
         element_type,
         transf_type,
         angle,
         camber_2,
         camber_3,
         n_x=None,
-        n_y=None
+        n_y=None,
     ):
         """
         Generates a plain component assembly, with line elements in
         series.
 
         """
 
@@ -687,15 +694,16 @@
             n_sub,
             transf_type,
             section,
             element_type,
             angle,
             camber_2,
             camber_3,
-            n_x, n_y
+            n_x,
+            n_y,
         )
 
         return component
 
     def generate_hinged_component_assembly(
         self,
         component_purpose,
@@ -707,15 +715,16 @@
         eo_j,
         section,
         element_type,
         transf_type,
         angle,
         camber_2,
         camber_3,
-        n_x, n_y,
+        n_x,
+        n_y,
         zerolength_gen_i,
         zerolength_gen_args_i,
         zerolength_gen_j,
         zerolength_gen_args_j,
     ):
         """
         Defines a component assembly that is comprised of
@@ -749,15 +758,14 @@
         clear_length = np.linalg.norm(p_j - p_i)
         zerolength_gen_args_i.update({"element_length": clear_length})
         zerolength_gen_args_j.update({"element_length": clear_length})
 
         # we can have hinges at both ends, or just one of the two ends.
         # ...or even no hinges!
         if zerolength_gen_i:
-
             hinge_location_i = p_i + x_axis * zerolength_gen_args_i["distance"]
             nh_i_out = Node(
                 self.model.uid_generator.new("node"), [*hinge_location_i]
             )
             nh_i_in = Node(
                 self.model.uid_generator.new("node"), [*hinge_location_i]
             )
@@ -792,17 +800,21 @@
                     element_type_i,
                     angle,
                     0.00,
                     0.00,
                 )
             elif element_type_i.__name__ == "TwoNodeLink":
                 elm = self.define_two_node_link(
-                    component, node_i, nh_i_out,
-                    x_axis, y_axis,
-                    zerolength_gen.fix_all, {}
+                    component,
+                    node_i,
+                    nh_i_out,
+                    x_axis,
+                    y_axis,
+                    zerolength_gen.fix_all,
+                    {},
                 )
                 component.elements.add(elm)
             else:
                 raise ValueError(f"Invalid element_type_i: {element_type_i}")
             zerolen_elm = self.define_zerolength(
                 component,
                 nh_i_out,
@@ -815,15 +827,14 @@
             component.elements.add(zerolen_elm)
             conn_node_i = nh_i_in
             conn_eo_i = np.zeros(3)
         else:
             conn_node_i = node_i
             conn_eo_i = eo_i
         if zerolength_gen_j:
-
             hinge_location_j = p_i + x_axis * (
                 clear_length - zerolength_gen_args_j["distance"]
             )
             nh_j_out = Node(
                 self.model.uid_generator.new("node"), [*hinge_location_j]
             )
             nh_j_in = Node(
@@ -856,21 +867,25 @@
                     eo_j,
                     zerolength_gen_args_j["n_sub"],
                     transf_type_j,
                     section_j,
                     element_type_j,
                     angle,
                     0.00,
-                    0.00
+                    0.00,
                 )
             elif element_type_j.__name__ == "TwoNodeLink":
                 elm = self.define_two_node_link(
-                    component, nh_j_out, node_j,
-                    x_axis, y_axis,
-                    zerolength_gen.fix_all, {}
+                    component,
+                    nh_j_out,
+                    node_j,
+                    x_axis,
+                    y_axis,
+                    zerolength_gen.fix_all,
+                    {},
                 )
                 component.elements.add(elm)
             else:
                 raise ValueError(f"Invalid element_type_j: {element_type_j}")
             zerolen_elm = self.define_zerolength(
                 component,
                 nh_j_out,
@@ -896,15 +911,16 @@
             n_sub,
             transf_type,
             section,
             element_type,
             angle,
             camber_2,
             camber_3,
-            n_x, n_y
+            n_x,
+            n_y,
         )
         return component
 
     def add_vertical_active(
         self,
         x_coord: float,
         y_coord: float,
@@ -1029,17 +1045,17 @@
 
             # retrieve local coordinate system
             x_axis, y_axis, z_axis = local_axes_from_points_and_angle(
                 p_i_init, p_j_init, angle
             )  # type: ignore
 
             p_i_init += h_offset_i * x_axis
-            p_j_init += - h_offset_j * x_axis
+            p_j_init += -h_offset_j * x_axis
             offset_i += h_offset_i * x_axis
-            offset_j += - h_offset_j * x_axis
+            offset_j += -h_offset_j * x_axis
 
             if section.snap_points and (placement != "centroid"):
                 # obtain offset from section (local system)
                 d_z, d_y = section.snap_points[placement]
                 sec_offset_local: nparr = np.array([0.00, d_y, d_z])
                 t_glob_to_loc = transformation_matrix(x_axis, y_axis, z_axis)
                 t_loc_to_glob = t_glob_to_loc.T
@@ -1091,131 +1107,141 @@
             args.update(additional_args)
             assert hasattr(self, method), f"Method not available: {method}"
             mthd = getattr(self, method)
             defined_component_assemblies[key] = mthd(**args)
         return defined_component_assemblies
 
     def add_diagonal_active(
-            self,
-            xi_coord: float,
-            yi_coord: float,
-            xj_coord: float,
-            yj_coord: float,
-            offset_i: nparr,
-            offset_j: nparr,
-            snap_i: str,
-            snap_j: str,
-            transf_type: str,
-            n_sub: int,
-            section: ElasticSection,
-            element_type: Type[Union[ElasticBeamColumn, DispBeamColumn]],
-            placement: str = 'centroid',
-            angle: float = 0.00,
-            camber_2: float = 0.00, camber_3: float = 0.00,
-            split_existing_i: Optional[ComponentAssembly] = None,
-            split_existing_j: Optional[ComponentAssembly] = None,
-            method: str = 'generate_plain_component_assembly',
-            additional_args: dict[str, object] = {}
+        self,
+        xi_coord: float,
+        yi_coord: float,
+        xj_coord: float,
+        yj_coord: float,
+        offset_i: nparr,
+        offset_j: nparr,
+        snap_i: str,
+        snap_j: str,
+        transf_type: str,
+        n_sub: int,
+        section: ElasticSection,
+        element_type: Type[Union[ElasticBeamColumn, DispBeamColumn]],
+        placement: str = 'centroid',
+        angle: float = 0.00,
+        camber_2: float = 0.00,
+        camber_3: float = 0.00,
+        split_existing_i: Optional[ComponentAssembly] = None,
+        split_existing_j: Optional[ComponentAssembly] = None,
+        method: str = 'generate_plain_component_assembly',
+        additional_args: dict[str, object] = {},
     ) -> dict[int, ComponentAssembly]:
         """
         Adds a diagonal beamcolumn element to all active levels.
 
         """
 
         query = ElmQuery(self.model)
         ndg = NodeGenerator(self.model)
         lvls = self.model.levels
         assert lvls.active, 'No active levels.'
         defined_component_assemblies: dict[int, ComponentAssembly] = {}
         for key in lvls.active:
             lvl = lvls[key]
-            lvl_prev = lvls.get(key-1)
+            lvl_prev = lvls.get(key - 1)
 
             if not lvl_prev:
                 continue
 
             p_i_init = np.array((xi_coord, yi_coord, lvl.elevation)) + offset_i
             p_j_init = np.array((xj_coord, yj_coord, lvl.elevation)) + offset_j
 
             if section.snap_points and (placement != 'centroid'):
                 # obtain offset from section (local system)
                 d_z, d_y = section.snap_points[placement]
                 sec_offset_local: nparr = np.array([0.00, d_y, d_z])
                 # retrieve local coordinate system
-                x_axis, y_axis, z_axis = \
-                    local_axes_from_points_and_angle(
-                        p_i_init, p_j_init, angle)  # type: ignore
-                t_glob_to_loc = transformation_matrix(
-                    x_axis, y_axis, z_axis)
+                x_axis, y_axis, z_axis = local_axes_from_points_and_angle(
+                    p_i_init, p_j_init, angle
+                )  # type: ignore
+                t_glob_to_loc = transformation_matrix(x_axis, y_axis, z_axis)
                 t_loc_to_glob = t_glob_to_loc.T
                 sec_offset_global = t_loc_to_glob @ sec_offset_local
             else:
                 sec_offset_global = np.zeros(3)
 
             node_i, eo_i = beam_placement_lookup(
-                xi_coord, yi_coord, query, ndg,
-                lvls, key, offset_i,
+                xi_coord,
+                yi_coord,
+                query,
+                ndg,
+                lvls,
+                key,
+                offset_i,
                 sec_offset_global,
                 split_existing_i,
-                snap_i)
+                snap_i,
+            )
             node_j, eo_j = beam_placement_lookup(
-                xj_coord, yj_coord, query, ndg,
-                lvls, key-1, offset_j,
+                xj_coord,
+                yj_coord,
+                query,
+                ndg,
+                lvls,
+                key - 1,
+                offset_j,
                 sec_offset_global,
                 split_existing_j,
-                snap_j)
+                snap_j,
+            )
 
             args = {
                 'component_purpose': 'diagonal_component',
                 'lvl': lvl,
                 'node_i': node_i,
                 'node_j': node_j,
                 'n_sub': n_sub,
                 'eo_i': eo_i,
                 'eo_j': eo_j,
                 'section': section,
                 'element_type': element_type,
                 'transf_type': transf_type,
                 'angle': angle,
                 'camber_2': camber_2,
-                'camber_3': camber_3
+                'camber_3': camber_3,
             }
 
             args.update(additional_args)
-            assert hasattr(self, method), \
-                f'Method not available: {method}'
+            assert hasattr(self, method), f'Method not available: {method}'
             mthd = getattr(self, method)
             defined_component_assemblies[key] = mthd(**args)
         return defined_component_assemblies
 
     def add_pz_active(
-            self,
-            x_coord: float,
-            y_coord: float,
-            section: ElasticSection,
-            physical_material: PhysicalMaterial,
-            angle: float,
-            column_depth: float,
-            beam_depth: float,
-            zerolength_method: str,
-            zerolength_args: dict[str, object],
+        self,
+        x_coord: float,
+        y_coord: float,
+        section: ElasticSection,
+        physical_material: PhysicalMaterial,
+        angle: float,
+        column_depth: float,
+        beam_depth: float,
+        zerolength_method: str,
+        zerolength_args: dict[str, object],
     ) -> dict[int, ComponentAssembly]:
         """
         Adds a component assembly representing a steel W-section
         panel zone joint.
 
         """
 
         ndg = NodeGenerator(self.model)
         query = ElmQuery(self.model)
         lvls = self.model.levels
         assert lvls.active, "No active levels."
         defined_components: dict[int, ComponentAssembly] = {}
         for key in lvls.active:
-
             lvl = lvls[key]
             if key - 1 not in lvls:
                 continue
 
             top_node = query.search_node_lvl(x_coord, y_coord, key)
             if not top_node:
                 top_node = ndg.add_node_lvl(x_coord, y_coord, key)
@@ -1308,21 +1334,21 @@
             new_uid = self.model.uid_generator.new("section")
             rigid_sec = ElasticSection(
                 name="rigid_link_section",
                 uid=new_uid,
                 outside_shape=None,
                 snap_points=None,
                 e_mod=section.e_mod,
-                area=section.area*factor_a,
-                i_y=section.i_y*factor_i,
-                i_x=section.i_x*factor_i,
+                area=section.area * factor_a,
+                i_y=section.i_y * factor_i,
+                i_x=section.i_x * factor_i,
                 g_mod=section.g_mod,
-                j_mod=section.j_mod*factor_j,
+                j_mod=section.j_mod * factor_j,
                 sec_w=0.00,
-                )
+            )
 
             elm_top_h_f = ElasticBeamColumn(
                 component,
                 self.model.uid_generator.new("element"),
                 [top_node, top_h_f],
                 rigid_sec,
                 GeomTransf(
@@ -1479,60 +1505,60 @@
                     z_axis,
                 ),
             )
             elm_interior.visibility.skip_opensees_definition = True
             elm_interior.visibility.hidden_at_line_plots = True
 
             assert hasattr(
-                zerolength_gen, zerolength_method), \
-                f"Method not available: {zerolength_method}"
+                zerolength_gen, zerolength_method
+            ), f"Method not available: {zerolength_method}"
             mthd = getattr(zerolength_gen, zerolength_method)
 
             # define zerolength elements
             zerolength_gen_args = {
-                    "section": section,
-                    "physical_material": physical_material,
-                    "pz_length": beam_depth
-                 }
+                "section": section,
+                "physical_material": physical_material,
+                "pz_length": beam_depth,
+            }
             zerolength_gen_args.update(zerolength_args)
             zerolen_top_f = self.define_zerolength(
                 component,
                 top_h_f,
                 top_v_f,
                 x_axis,
                 y_axis,
                 mthd,
-                zerolength_gen_args
+                zerolength_gen_args,
             )
             zerolen_top_b = self.define_zerolength(
                 component,
                 top_h_b,
                 top_v_b,
                 x_axis,
                 y_axis,
                 zerolength_gen.release_6,
-                {}
+                {},
             )
             zerolen_bottom_f = self.define_zerolength(
                 component,
                 bottom_h_f,
                 bottom_v_f,
                 x_axis,
                 y_axis,
                 zerolength_gen.release_6,
-                {}
+                {},
             )
             zerolen_bottom_b = self.define_zerolength(
                 component,
                 bottom_h_b,
                 bottom_v_b,
                 x_axis,
                 y_axis,
                 zerolength_gen.release_6,
-                {}
+                {},
             )
 
             # fill component assembly
             component.external_nodes.add(top_node)
             component.external_nodes.named_contents["top_node"] = top_node
             component.external_nodes.add(bottom_mid)
             component.external_nodes.named_contents["bottom_node"] = bottom_mid
@@ -1547,43 +1573,29 @@
             component.internal_nodes.add(top_v_b)
             component.internal_nodes.add(bottom_h_f)
             component.internal_nodes.add(bottom_h_b)
             component.internal_nodes.add(bottom_v_f)
             component.internal_nodes.add(bottom_v_b)
 
             component.elements.add(elm_top_h_f)
-            (
-                component.elements.named_contents[
-                    "elm_top_h_f"
-                ]
-            ) = elm_top_h_f
+            (component.elements.named_contents["elm_top_h_f"]) = elm_top_h_f
             component.elements.add(elm_top_h_b)
-            (
-                component.elements.named_contents[
-                    "elm_top_h_b"
-                ]
-            ) = elm_top_h_b
+            (component.elements.named_contents["elm_top_h_b"]) = elm_top_h_b
             component.elements.add(elm_bottom_h_f)
             component.elements.add(elm_bottom_h_b)
             component.elements.add(elm_top_v_f)
             component.elements.add(elm_top_v_b)
             component.elements.add(elm_bottom_v_f)
             component.elements.add(elm_bottom_v_b)
             component.elements.add(elm_interior)
-            (
-                component.elements.named_contents[
-                    "elm_interior"
-                ]
-            ) = elm_interior
+            (component.elements.named_contents["elm_interior"]) = elm_interior
 
             component.elements.add(zerolen_top_f)
             (
-                component.elements.named_contents[
-                    "nonlinear_spring"
-                ]
+                component.elements.named_contents["nonlinear_spring"]
             ) = zerolen_top_f  # type: ignore
             component.elements.add(zerolen_top_b)
             component.elements.add(zerolen_bottom_f)
             component.elements.add(zerolen_bottom_b)
             defined_components[key] = component
 
         return defined_components
```

### Comparing `osmg-0.2.4/src/osmg/gen/material_gen.py` & `osmg-0.2.5/src/osmg/gen/material_gen.py`

 * *Files 4% similar despite different names*

```diff
@@ -140,23 +140,23 @@
             param_b,
             param_r0,
             param_c_r1,
             param_c_r2,
             a1=0.2,
             a2=1.0,
             a3=0.2,
-            a4=1.0
+            a4=1.0,
         )
 
         fatigue_mat = Fatigue(
             self.model.uid_generator.new("uniaxial material"),
             "auto_fatigue_brace_mat",
             steel02_mat,
             var_e0,
-            var_m
+            var_m,
         )
 
         return fatigue_mat
 
     def generate_steel_w_imk_material(
         self,
         section,
@@ -166,15 +166,15 @@
         loverh,
         rbs_factor,
         consider_composite,
         axial_load_ratio,
         direction="strong",
         moment_modifier=1.00,
         n_parameter=0.00,
-        only_elastic=False
+        only_elastic=False,
     ):
         """
         Lignos, D. G., & Krawinkler, H. (2011). Deterioration modeling of
         steel components in support of collapse prediction of steel moment
         frames under earthquake loading. Journal of Structural
         Engineering-Reston, 137(11), 1291.
 
@@ -220,15 +220,14 @@
         elm_l = loverh * elm_h
         elm_lb = lboverl * elm_l
         lbry = elm_lb / sec_ry
 
         # consider cases
 
         if rbs_factor:
-
             # RBS case
             assert direction == "strong"
             assert rbs_factor <= 1.00, "rbs_factor must be <= 1.00"
             # checks ~ acceptable range
             if not 20.00 < sec_d / sec_tw < 55.00:
                 print(
                     f"Warning: sec_d/sec_tw={sec_d/sec_tw:.2f}"
@@ -245,23 +244,21 @@
                     f"Warning: bf/(2 tf)={sec_bf/(2.*sec_tf):.2f}"
                     " outside regression range"
                 )
                 print("4.00 < (sec_bf/(2.*sec_tf)) < 8.00")
                 print(section.name, "\n")
             if not 2.5 < elm_l / sec_d < 7.0:
                 print(
-                    f"Warning: L/d={elm_l/sec_d:.2f}"
-                    "  outside regression range"
+                    f"Warning: L/d={elm_l/sec_d:.2f}  outside regression range"
                 )
                 print("2.5 < elm_l/sec_d < 7.0")
                 print(section.name, "\n")
             if not 4.00 < sec_d < 36.00:
                 print(
-                    f"Warning: Section d={sec_d:.2f} "
-                    "outside regression range"
+                    f"Warning: Section d={sec_d:.2f} outside regression range"
                 )
                 print("4.00 < sec_d < 36.00")
                 print(section.name, "\n")
             if not 35.00 < mat_fy < 65.00:
                 print(f"Warning: Fy={mat_fy:.2f} outside regression range")
                 print("35.00 < mat_fy < 65.00")
                 print(section.name, "\n")
@@ -292,15 +289,14 @@
             rbs_c = sec_bf * (1.0 - rbs_factor) / 2.0
             z_rbs = sec_z - 2.0 * rbs_c * sec_tf * (sec_d - sec_tf)
             sec_m = 1.06 * z_rbs * mat_fy * 1.0e3
             mcmy_plus = 1.10
             mcmy_minus = 1.10
 
         else:
-
             # Other-than-RBS case
             if axial_load_ratio:
                 # column case
                 theta_p = (
                     294.00
                     * (sec_d / sec_tw) ** (-1.70)
                     * lbry ** (-0.70)
@@ -326,33 +322,42 @@
                         268000.00
                         * (sec_d / sec_tw) ** (-2.30)
                         * lbry ** (-1.30)
                         * (1.00 - axial_load_ratio) ** (1.19)
                     )
                 if axial_load_ratio <= 0.20:
                     sec_m = (
-                        1.15/1.10 * (sec_z * mat_fy) * 1.0e3
-                        * (1.00 - axial_load_ratio / 2.00))
+                        1.15
+                        / 1.10
+                        * (sec_z * mat_fy)
+                        * 1.0e3
+                        * (1.00 - axial_load_ratio / 2.00)
+                    )
                 else:
                     sec_m = (
-                        1.15/1.10 * (sec_z * mat_fy) * 1.0e3
-                        * 9.0/8.0 * (1.00 - axial_load_ratio))
+                        1.15
+                        / 1.10
+                        * (sec_z * mat_fy)
+                        * 1.0e3
+                        * 9.0
+                        / 8.0
+                        * (1.00 - axial_load_ratio)
+                    )
                 mcmy = (
                     12.5
                     * (sec_d / sec_tw) ** (-0.20)
                     * lbry ** (-0.40)
                     * (1.00 - axial_load_ratio) ** (0.40)
-                    )
+                )
                 mcmy = min(mcmy, 1.00)
                 mcmy = max(mcmy, 1.30)
                 mcmy_plus = mcmy
                 mcmy_minus = mcmy
 
             else:
-
                 # non-RBS beam case
                 theta_p = (
                     0.0865
                     * (sec_d / sec_tw) ** (-0.365)
                     * (sec_bf / (2.0 * sec_tf)) ** (-0.14)
                     * (elm_l / sec_d) ** 0.34
                     * (25.4 * sec_d / 533.0) ** (-0.721)
@@ -384,27 +389,27 @@
         theta_pc_minus = theta_pc
         d_plus = 1.00
         d_minus = 1.00
         m_plus = sec_m
         m_minus = -sec_m
 
         if consider_composite:
-
             # Elkady, A., & Lignos, D. G. (2014). Modeling of the
             # composite action in fully restrained beam‐to‐column
             # connections: implications in the seismic design and
             # collapse capacity of steel special moment
             # frames. Earthquake Engineering & Structural Dynamics,
             # 43(13), 1935-1954.  Table II
 
-            assert axial_load_ratio == 0.00, \
-                "Can't consider composite action for columns"
-            assert direction == "strong", \
-                "Composite action affects the " \
-                "behavior in strong-axis bending"
+            assert (
+                axial_load_ratio == 0.00
+            ), "Can't consider composite action for columns"
+            assert (
+                direction == "strong"
+            ), "Composite action affects the behavior in strong-axis bending"
 
             theta_p_plus *= 1.80
             theta_p_minus *= 0.95
             theta_pc_plus *= 1.35
             theta_pc_minus *= 0.95
             d_plus = 1.15
             d_minus = 1.00
@@ -413,24 +418,22 @@
             m_plus *= 1.35
             m_minus *= 1.25
             residual_plus = 0.30
             residual_minus = 0.20
 
         # adjust parameters to account for the presence of the elastic element
         stiffness_init = 6.00 * section.e_mod * sec_i / elm_h
-        stiffness = (n_parameter+1.00) * stiffness_init
+        stiffness = (n_parameter + 1.00) * stiffness_init
         theta_y = sec_m / stiffness_init
         theta_p_plus -= (mcmy_plus - 1.0) * (sec_m / stiffness)
         theta_p_minus -= (mcmy_minus - 1.0) * (sec_m / stiffness)
         theta_pc_plus += theta_y + (mcmy_plus - 1.0) * (sec_m / stiffness)
         theta_pc_plus += theta_y + (mcmy_minus - 1.0) * (sec_m / stiffness)
         beta_plus = (mcmy_plus - 1.0) * m_plus / theta_p_plus / stiffness
-        beta_minus = (
-            -(mcmy_minus - 1.0) * m_minus / theta_p_minus / stiffness
-        )
+        beta_minus = -(mcmy_minus - 1.0) * m_minus / theta_p_minus / stiffness
 
         # # old model
         # from ..ops.uniaxial_material import Bilin
         # bilin_mat = Bilin(
         #     self.model.uid_generator.new("uniaxial material"),
         #     "auto_IMK",
         #     stiffness * moment_modifier,
@@ -460,36 +463,36 @@
         # )
 
         # new model
         if only_elastic:
             elastic_mat = Elastic(
                 self.model.uid_generator.new("uniaxial material"),
                 "auto_IMK",
-                stiffness * moment_modifier
+                stiffness * moment_modifier,
             )
             return elastic_mat
         bilin_mat = IMKBilin(
             self.model.uid_generator.new("uniaxial material"),
             "auto_IMK",
             stiffness * moment_modifier,
             theta_p_plus,
             theta_pc_plus,
             theta_u,
-            m_plus*moment_modifier,
+            m_plus * moment_modifier,
             (1.0 + beta_plus),
             residual_plus,
             theta_p_minus,
             theta_pc_minus,
             theta_u,
-            -m_minus*moment_modifier,
+            -m_minus * moment_modifier,
             (1.0 + beta_minus),
             residual_minus,
             lamda,
             lamda,
             lamda,
             1.00,
             1.00,
             1.00,
             d_plus,
-            d_minus
+            d_minus,
         )
         return bilin_mat
```

### Comparing `osmg-0.2.4/src/osmg/gen/mesh_shapes.py` & `osmg-0.2.5/src/osmg/gen/mesh_shapes.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,18 +243,17 @@
     num_vertices = 32  # Number of vertices on the circumference
 
     angle_increment = 2 * np.pi / num_vertices
 
     vertices = []
     for i in range(num_vertices):
         angle = i * angle_increment
-        vertices.append(Vertex((
-            radius * np.cos(angle),
-            radius * np.sin(angle)
-        )))
+        vertices.append(
+            Vertex((radius * np.cos(angle), radius * np.sin(angle)))
+        )
 
     edges = define_edges(vertices)
     return generate(edges)
 
 
 def generic_snap_points(mesh: Mesh) -> dict[str, nparr]:
     """
```

### Comparing `osmg-0.2.4/src/osmg/gen/node_gen.py` & `osmg-0.2.5/src/osmg/gen/node_gen.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/gen/query.py` & `osmg-0.2.5/src/osmg/gen/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,16 +169,16 @@
                     reject = True
                     continue
             if not reject:
                 retrieved_component = component
         return retrieved_component
 
     def retrieve_component(
-            self, x_loc: float, y_loc: float, lvl: int) \
-            -> Optional[ComponentAssembly]:
+        self, x_loc: float, y_loc: float, lvl: int
+    ) -> Optional[ComponentAssembly]:
         """
         Retrieves a component assembly of a level if any of its
         line elements passes trhough the specified point.
 
         Arguments:
           x_loc: x-coordinate
           y_loc: y-coordinate
@@ -188,35 +188,40 @@
           The first element found, None otherwise.
 
         """
         level = self.model.levels[lvl]
         for component in level.components.values():
             if len(component.external_nodes) != 2:
                 continue
-            line_elems: list[Union[
-                element.TrussBar,
-                element.ElasticBeamColumn,
-                element.DispBeamColumn]] = []
+            line_elems: list[
+                Union[
+                    element.TrussBar,
+                    element.ElasticBeamColumn,
+                    element.DispBeamColumn,
+                ]
+            ] = []
             for elm in component.elements.values():
                 if isinstance(elm, element.TrussBar):
                     line_elems.append(elm)
                 if isinstance(elm, element.ElasticBeamColumn):
                     line_elems.append(elm)
                 if isinstance(elm, element.DispBeamColumn):
                     line_elems.append(elm)
 
             for elm in line_elems:
                 if isinstance(elm, element.TrussBar):
                     p_i = np.array(elm.nodes[0].coords)
                     p_j = np.array(elm.nodes[1].coords)
                 else:
-                    p_i = np.array(
-                        elm.nodes[0].coords) + elm.geomtransf.offset_i
-                    p_j = np.array(
-                        elm.nodes[1].coords) + elm.geomtransf.offset_j
+                    p_i = (
+                        np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
+                    )
+                    p_j = (
+                        np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
+                    )
                 if np.linalg.norm(p_i[0:2] - p_j[0:2]) < common.EPSILON:
                     if (
                         np.linalg.norm(np.array((x_loc, y_loc)) - p_i[0:2])
                         < common.EPSILON
                     ):
                         return component
                 else:
```

### Comparing `osmg-0.2.4/src/osmg/gen/section_gen.py` & `osmg-0.2.5/src/osmg/gen/section_gen.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,17 +341,15 @@
                 # suare and round HSS
                 assert sec_data["Type"] == "HSS"
                 # must be circular: name will have 1.
                 assert len(label.split("X")) == 2
                 sec_h = sec_data["OD"]
                 sec_t = sec_data["tdes"]
                 outside_shape = mesh_shapes.circ_mesh(sec_h)
-                hole = mesh_shapes.circ_mesh(
-                    sec_h - 2.00 * sec_t
-                )
+                hole = mesh_shapes.circ_mesh(sec_h - 2.00 * sec_t)
                 bbox = outside_shape.bounding_box()
                 z_min, y_min, z_max, y_max = bbox.flatten()
                 snap_points = {
                     "centroid": np.array([0.0, 0.0]),
                     "top_center": np.array([0.0, -y_max]),
                     "top_left": np.array([-z_min, -y_max]),
                     "top_right": np.array([-z_max, -y_max]),
```

### Comparing `osmg-0.2.4/src/osmg/gen/steel/brb.py` & `osmg-0.2.5/src/osmg/gen/steel/brb.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     """
     This object holds default values that are used by BRBGenerator
     objects, to better organize those values and improve the usability
     of the BRBGenerator objects by allowing their methods to have
     fewer arguments.
 
     """
+
     steel4_b_k: float = field(default=0.003)
     steel4_b_kc: float = field(default=0.023)
     steel4_R_0: float = field(default=25.00)
     steel4_R_0c: float = field(default=25.00)
     steel4_r_1: float = field(default=0.90)
     steel4_r_1c: float = field(default=0.90)
     steel4_r_2: float = field(default=0.15)
@@ -77,30 +78,30 @@
 
     """
 
     model: Model
     settings: BRBGenSettings = field(default_factory=BRBGenSettings)
 
     def add_brb(
-            self,
-            xi_coord: float,
-            yi_coord: float,
-            lvl_key_i: int,
-            offset_i: nparr,
-            snap_i: str,
-            xj_coord: float,
-            yj_coord: float,
-            lvl_key_j: int,
-            offset_j: nparr,
-            snap_j: str,
-            area: float,
-            f_y: float,
-            e_0: float,
-            casing_size: float,
-            unit_weight: float
+        self,
+        xi_coord: float,
+        yi_coord: float,
+        lvl_key_i: int,
+        offset_i: nparr,
+        snap_i: str,
+        xj_coord: float,
+        yj_coord: float,
+        lvl_key_j: int,
+        offset_j: nparr,
+        snap_j: str,
+        area: float,
+        f_y: float,
+        e_0: float,
+        casing_size: float,
+        unit_weight: float,
     ) -> None:
         """
         Adds a BRB element to the model.
 
         Parameters:
           xi_coord: x coordinate of the i-end
           yi_coord: y coordinate of the i-end
@@ -135,16 +136,15 @@
             self-weight and self-mass preprocessing methods are
             called.
 
         """
 
         trg = TrussBarGenerator(self.model)
 
-        uid = self.model.uid_generator.new(
-            "uniaxial material")
+        uid = self.model.uid_generator.new("uniaxial material")
         mat = Steel4(
             uid=uid,
             name=f'auto_BRB_{uid}',
             Fy=f_y,
             E0=e_0,
             b_k=self.settings.steel4_b_k,
             b_kc=self.settings.steel4_b_kc,
@@ -160,30 +160,32 @@
             rho_ic=self.settings.steel4_rho_ic,
             b_l=self.settings.steel4_b_l,
             b_lc=self.settings.steel4_b_lc,
             R_i=self.settings.steel4_R_i,
             R_ic=self.settings.steel4_R_ic,
             l_yp=self.settings.steel4_l_yp,
         )
-        uid = self.model.uid_generator.new(
-            "uniaxial material")
+        uid = self.model.uid_generator.new("uniaxial material")
         mat_fatigue = Fatigue(
             uid=uid,
             name=f'auto_BRB_fatigue_{uid}',
             predecessor=mat,
             e_mod=self.settings.fatigue_e_mod,
-            var_m=self.settings.fatigue_var_m)
+            var_m=self.settings.fatigue_var_m,
+        )
         trg.add(
-            xi_coord, yi_coord,
+            xi_coord,
+            yi_coord,
             lvl_key_i,
             offset_i,
             snap_i,
-            xj_coord, yj_coord,
+            xj_coord,
+            yj_coord,
             lvl_key_j,
             offset_j,
             snap_j,
             transf_type=self.settings.transf_type,
             area=area,
             mat=mat_fatigue,
             outside_shape=rect_mesh(casing_size, casing_size),
-            weight_per_length=unit_weight*casing_size**2
+            weight_per_length=unit_weight * casing_size**2,
         )
```

### Comparing `osmg-0.2.4/src/osmg/gen/uid_gen.py` & `osmg-0.2.5/src/osmg/gen/uid_gen.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/gen/zerolength_gen.py` & `osmg-0.2.5/src/osmg/gen/zerolength_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,89 +30,89 @@
 
 if TYPE_CHECKING:
     from ..model import Model
     from ..physical_material import PhysicalMaterial
 
 
 def fix_all(
-        model: Model, **kwargs: dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model, **kwargs: dict[object, object]
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Fixed in all directions.
 
     """
 
     dirs = [1, 2, 3, 4, 5, 6]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat] * 3
     return dirs, mats
 
 
 def release_6(
-        model: Model, **kwargs: dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model, **kwargs: dict[object, object]
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Frees strong axis bending.
 
     """
 
     dirs = [1, 2, 3, 4, 5]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat] * 2
     return dirs, mats
 
 
 def release_5(
-        model: Model, **kwargs: dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model, **kwargs: dict[object, object]
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Frees weak axis bending.
 
     """
 
     dirs = [1, 2, 3, 4, 6]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat] * 2
     return dirs, mats
 
 
 def release_56(
-        model: Model, **kwargs: dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model, **kwargs: dict[object, object]
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Frees both strong and weak axis bending.
 
     """
 
     dirs = [1, 2, 3, 4]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat]
     return dirs, mats
 
 
 def imk_6(
-        model: Model,
-        element_length: float,
-        lboverl: float,
-        loverh: float,
-        rbs_factor: Optional[float],
-        consider_composite: bool,
-        axial_load_ratio: float,
-        section: ElasticSection,
-        physical_material: PhysicalMaterial,
-        **kwargs: dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model,
+    element_length: float,
+    lboverl: float,
+    loverh: float,
+    rbs_factor: Optional[float],
+    consider_composite: bool,
+    axial_load_ratio: float,
+    section: ElasticSection,
+    physical_material: PhysicalMaterial,
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Lignos, D. G., & Krawinkler, H. (2011). Deterioration modeling of
     steel components in support of collapse prediction of steel moment
     frames under earthquake loading. Journal of Structural
     Engineering-Reston, 137(11), 1291.
 
     Elkady, A., & Lignos, D. G. (2014). Modeling of the composite
@@ -136,36 +136,36 @@
         loverh,
         rbs_factor,
         consider_composite,
         axial_load_ratio,
         direction="strong",
         moment_modifier=moment_modifier,
         n_parameter=n_parameter,
-        only_elastic=only_elastic
+        only_elastic=only_elastic,
     )
     dirs = [1, 2, 3, 4, 5, 6]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat] * 2 + [mat]
     return dirs, mats
 
 
 def imk_56(
-        model: Model,
-        element_length: float,
-        lboverl: float,
-        loverh: float,
-        rbs_factor: Optional[float],
-        consider_composite: bool,
-        axial_load_ratio: float,
-        section: ElasticSection,
-        physical_material: PhysicalMaterial,
-        **kwargs:  dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model,
+    element_length: float,
+    lboverl: float,
+    loverh: float,
+    rbs_factor: Optional[float],
+    consider_composite: bool,
+    axial_load_ratio: float,
+    section: ElasticSection,
+    physical_material: PhysicalMaterial,
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     release in the weak axis bending direction,
     :func:`~osmg.gen.zerolength_gen.imk_6` in the strong axis bending
     direction
 
     """
 
@@ -182,49 +182,49 @@
         loverh,
         rbs_factor,
         consider_composite,
         axial_load_ratio,
         direction="strong",
         moment_modifier=moment_modifier,
         n_parameter=n_parameter,
-        only_elastic=only_elastic
+        only_elastic=only_elastic,
     )
     mat_weak = mat_generator.generate_steel_w_imk_material(
         section,
         physical_material,
         element_length,
         lboverl,
         loverh,
         rbs_factor,
         consider_composite,
         axial_load_ratio,
         direction="weak",
         moment_modifier=moment_modifier,
-        only_elastic=only_elastic
+        only_elastic=only_elastic,
     )
     dirs = [1, 2, 3, 4, 5, 6]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat, mat_weak, mat_strong]
     return dirs, mats
 
 
 def imk_6_release_5(
-        model: Model,
-        element_length: float,
-        lboverl: float,
-        loverh: float,
-        rbs_factor: Optional[float],
-        consider_composite: bool,
-        axial_load_ratio: float,
-        section: ElasticSection,
-        physical_material: PhysicalMaterial,
-        **kwargs:  dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model,
+    element_length: float,
+    lboverl: float,
+    loverh: float,
+    rbs_factor: Optional[float],
+    consider_composite: bool,
+    axial_load_ratio: float,
+    section: ElasticSection,
+    physical_material: PhysicalMaterial,
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     release in the weak axis bending direction,
     :func:`~osmg.gen.zerolength_gen.imk_6` in the strong axis bending
     direction
 
     """
 
@@ -241,31 +241,31 @@
         loverh,
         rbs_factor,
         consider_composite,
         axial_load_ratio,
         direction="strong",
         moment_modifier=moment_modifier,
         n_parameter=n_parameter,
-        only_elastic=only_elastic
+        only_elastic=only_elastic,
     )
     dirs = [1, 2, 3, 4, 6]
     mat_repo = model.uniaxial_materials
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat, mat_strong]
     return dirs, mats
 
 
 def gravity_shear_tab(
-        model: Model,
-        consider_composite: bool,
-        section: ElasticSection,
-        physical_material: PhysicalMaterial,
-        **kwargs:  dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model,
+    consider_composite: bool,
+    section: ElasticSection,
+    physical_material: PhysicalMaterial,
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Elkady, A., & Lignos, D. G. (2015). Effect of gravity framing on
     the overstrength and collapse capacity of steel frame buildings
     with perimeter special moment frames. Earthquake Engineering &
     Structural Dynamics, 44(8), 1289-1307.
 
     """
@@ -397,24 +397,24 @@
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     release_mat = mat_repo.retrieve_by_attr("name", "release")
     mats = [fix_mat] * 3 + [fix_rot_mat, release_mat, mat]
     return dirs, mats
 
 
 def steel_w_col_pz(
-        model: Model,
-        section: ElasticSection,
-        physical_material: PhysicalMaterial,
-        pz_length: float,
-        pz_doubler_plate_thickness: float,
-        pz_hardening: float,
-        only_elastic: bool = False,
-        moment_modifier: float = 1.00,
-        **kwargs:  dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model,
+    section: ElasticSection,
+    physical_material: PhysicalMaterial,
+    pz_length: float,
+    pz_doubler_plate_thickness: float,
+    pz_hardening: float,
+    only_elastic: bool = False,
+    moment_modifier: float = 1.00,
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Gupta, A., & Krawinkler, H. (1999). Seismic demands for the
     performance evaluation of steel moment resisting frame
     structures. Rep. No. 132.
 
     """
 
@@ -433,26 +433,26 @@
     v_y = 0.55 * f_y * d_c * t_p
     g_mod = physical_material.g_mod
     k_e = 0.95 * g_mod * t_p * d_c
     k_p = 0.95 * g_mod * bfc * t_f**2 / pz_length
     gamma_1 = v_y / k_e
     gamma_2 = 4.0 * gamma_1
     gamma_3 = 100.0 * gamma_1
-    m1y = (gamma_1 * k_e * pz_length
-           * moment_modifier)
-    m2y = (m1y + k_p * pz_length * (gamma_2 - gamma_1)
-           * moment_modifier)
-    m3y = (m2y + (hardening * k_e * pz_length) * (gamma_3 - gamma_2)
-           * moment_modifier)
+    m1y = gamma_1 * k_e * pz_length * moment_modifier
+    m2y = m1y + k_p * pz_length * (gamma_2 - gamma_1) * moment_modifier
+    m3y = (
+        m2y
+        + (hardening * k_e * pz_length) * (gamma_3 - gamma_2) * moment_modifier
+    )
 
     if only_elastic:
         mat: UniaxialMaterial = Elastic(
             model.uid_generator.new("uniaxial material"),
             "auto_steel_W_PZ",
-            m1y/gamma_1
+            m1y / gamma_1,
         )
     else:
         mat = Hysteretic(
             model.uid_generator.new("uniaxial material"),
             "auto_steel_W_PZ",
             (m1y, gamma_1),
             (m2y, gamma_2),
@@ -482,16 +482,16 @@
     pz_doubler_plate_thickness: float,
     axial_load_ratio: float,
     slab_depth: float,
     consider_composite: bool,
     location: str,
     only_elastic: bool = False,
     moment_modifier: float = 1.00,
-    **kwargs:  dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Skiadopoulos, A., Elkady, A. and D. G. Lignos (2020). "Proposed
     Panel Zone Model for Seismic Design of Steel Moment-Resisting
     Frames." ASCE Journal of Structural Engineering. DOI:
     10.1061/(ASCE)ST.1943-541X.0002935.
 
     """
@@ -522,23 +522,36 @@
     if consider_composite:
         d_BeamP = d_Beam + trib + 0.50 * ts
     # effective depth in negative moment
     d_BeamN = d_Beam
 
     # Stiffness Calculation
     Ks = tpz * (d_Col - tf_Col) * g_mod
-    Kb = (12.0 * e_mod * (Ix_Col + tdp *
-          ((d_Col - 2.0 * tf_Col)**3) / 12.00) / (d_Beam**3) * d_Beam)
+    Kb = (
+        12.0
+        * e_mod
+        * (Ix_Col + tdp * ((d_Col - 2.0 * tf_Col) ** 3) / 12.00)
+        / (d_Beam**3)
+        * d_Beam
+    )
     Ke = Ks * Kb / (Ks + Kb)
 
     # flange stiffness: shear contribution
     Ksf = 2.0 * (bf_Col * tf_Col) * g_mod
     # flange stiffness: bending contribution
-    Kbf = (2.0 * 12.0 * e_mod * bf_Col
-           * (tf_Col**3) / 12.0 / (d_Beam**3) * d_Beam)
+    Kbf = (
+        2.0
+        * 12.0
+        * e_mod
+        * bf_Col
+        * (tf_Col**3)
+        / 12.0
+        / (d_Beam**3)
+        * d_Beam
+    )
     # flange stiffness: total contribution
     Kef = (Ksf * Kbf) / (Ksf + Kbf)
 
     ay = (0.58 * Kef / Ke + 0.88) / (1.0 - Kef / Ke)
 
     aw_eff_4gamma = 1.10
     aw_eff_6gamma = 1.15
@@ -547,24 +560,34 @@
     af_eff_6gamma = 1.05 * Kef / Ke + 0.020
     # reduction factor accounting for axial load
     r = np.sqrt(1.0 - (n**2))
 
     Vy = r * 0.577 * f_y * ay * (d_Col - tf_Col) * tpz
     # Plastic Shear Force at 4 gammaY
     Vp_4gamma = (
-        r * 0.577 * f_y * (
-            aw_eff_4gamma * (d_Col - tf_Col)
-            * tpz + af_eff_4gamma * (bf_Col - tw_Col) * 2*tf_Col))
+        r
+        * 0.577
+        * f_y
+        * (
+            aw_eff_4gamma * (d_Col - tf_Col) * tpz
+            + af_eff_4gamma * (bf_Col - tw_Col) * 2 * tf_Col
+        )
+    )
     # Plastic Shear Force at 6 gammaY
     Vp_6gamma = (
-        r * 0.577 * f_y * (
-            aw_eff_6gamma * (d_Col - tf_Col)
-            * tpz + af_eff_6gamma * (bf_Col - tw_Col) * 2*tf_Col))
+        r
+        * 0.577
+        * f_y
+        * (
+            aw_eff_6gamma * (d_Col - tf_Col) * tpz
+            + af_eff_6gamma * (bf_Col - tw_Col) * 2 * tf_Col
+        )
+    )
 
-    gamma_y = Vy/Ke
+    gamma_y = Vy / Ke
     gamma4_y = 4.0 * gamma_y
 
     My_P = Vy * d_BeamP
     Mp_4gamma_P = Vp_4gamma * d_BeamP
     Mp_6gamma_P = Vp_6gamma * d_BeamP
 
     My_N = Vy * d_BeamN
@@ -592,60 +615,84 @@
     M2_P *= moment_modifier
     M3_P *= moment_modifier
     M1_N *= moment_modifier
     M2_N *= moment_modifier
     M3_N *= moment_modifier
 
     if not consider_composite:
-        args = ((M1_N, gamma1),
-                (M2_N, gamma2),
-                (M3_N, gamma3),
-                (-M1_N, -gamma1),
-                (-M2_N, -gamma2),
-                (-M3_N, -gamma3),
-                0.25, 0.75, 0.0, 0.0, 0.0)
+        args = (
+            (M1_N, gamma1),
+            (M2_N, gamma2),
+            (M3_N, gamma3),
+            (-M1_N, -gamma1),
+            (-M2_N, -gamma2),
+            (-M3_N, -gamma3),
+            0.25,
+            0.75,
+            0.0,
+            0.0,
+            0.0,
+        )
     elif location == 'interior':
-        args = ((M1_P, gamma1),
-                (M2_P, gamma2),
-                (M3_P, gamma3),
-                (-M1_P, -gamma1),
-                (-M2_P, -gamma2),
-                (-M3_P, -gamma3),
-                0.25, 0.75, 0.0, 0.0, 0.0)
+        args = (
+            (M1_P, gamma1),
+            (M2_P, gamma2),
+            (M3_P, gamma3),
+            (-M1_P, -gamma1),
+            (-M2_P, -gamma2),
+            (-M3_P, -gamma3),
+            0.25,
+            0.75,
+            0.0,
+            0.0,
+            0.0,
+        )
     elif location == 'exterior_first':
-        args = ((M1_N, gamma1),
-                (M2_N, gamma2),
-                (M3_N, gamma3),
-                (-M1_P, -gamma1),
-                (-M2_P, -gamma2),
-                (-M3_P, -gamma3),
-                0.25, 0.75, 0.0, 0.0, 0.0)
+        args = (
+            (M1_N, gamma1),
+            (M2_N, gamma2),
+            (M3_N, gamma3),
+            (-M1_P, -gamma1),
+            (-M2_P, -gamma2),
+            (-M3_P, -gamma3),
+            0.25,
+            0.75,
+            0.0,
+            0.0,
+            0.0,
+        )
     elif location == 'exterior_last':
-        args = ((M1_P, gamma1),
-                (M2_P, gamma2),
-                (M3_P, gamma3),
-                (-M1_N, -gamma1),
-                (-M2_N, -gamma2),
-                (-M3_N, -gamma3),
-                0.25, 0.75, 0.0, 0.0, 0.0)
+        args = (
+            (M1_P, gamma1),
+            (M2_P, gamma2),
+            (M3_P, gamma3),
+            (-M1_N, -gamma1),
+            (-M2_N, -gamma2),
+            (-M3_N, -gamma3),
+            0.25,
+            0.75,
+            0.0,
+            0.0,
+            0.0,
+        )
     else:
         raise ValueError(f'Invalid Location: {location}')
 
     if only_elastic:
         m1y, gamma_1 = args[0]  # type: ignore
         mat: UniaxialMaterial = Elastic(
             model.uid_generator.new("uniaxial material"),
             "auto_steel_W_PZ",
-            m1y/gamma_1  # type: ignore
+            m1y / gamma_1,  # type: ignore
         )
     else:
         mat = Hysteretic(
             model.uid_generator.new("uniaxial material"),
             "auto_steel_W_pz_updated",
-            *args
+            *args,
         )
     # minmaxmat = MinMax(
     #     model.uid_generator.new("uniaxial material"),
     #     "auto_steel_W_pz_updated_minmax",
     #     mat, gammaU_N, gammaU_P)
     # print(mat.ops_args())
     dirs = [1, 2, 3, 4, 5, 6]
@@ -653,22 +700,22 @@
     fix_mat = mat_repo.retrieve_by_attr("name", "fix")
     fix_rot_mat = mat_repo.retrieve_by_attr("name", "fix_rot")
     mats = [fix_mat] * 3 + [fix_rot_mat] * 2 + [mat]
     return dirs, mats
 
 
 def steel_brace_gusset(
-        model: Model,
-        physical_mat: PhysicalMaterial,
-        d_brace: float,
-        l_c: float,
-        t_p: float,
-        l_b: float,
-        **kwargs:  dict[object, object]) \
-        -> tuple[list[int], list[UniaxialMaterial]]:
+    model: Model,
+    physical_mat: PhysicalMaterial,
+    d_brace: float,
+    l_c: float,
+    t_p: float,
+    l_b: float,
+    **kwargs: dict[object, object],
+) -> tuple[list[int], list[UniaxialMaterial]]:
     """
     Hsiao, P-C., Lehman, D.E., and Roeder, C.W., 2012, Improved
     analytical model for special concentrically braced frames, Journal
     of Constructional Steel Research, Vol. 73, pp 80-94.
 
     Arguments:
       model: Model object
```

### Comparing `osmg-0.2.4/src/osmg/get_latest_pypi_version.py` & `osmg-0.2.5/src/osmg/get_latest_pypi_version.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/graphics/general_2d.py` & `osmg-0.2.5/src/osmg/graphics/general_2d.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/graphics/graphics_common.py` & `osmg-0.2.5/src/osmg/graphics/graphics_common.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/graphics/graphics_common_3d.py` & `osmg-0.2.5/src/osmg/graphics/graphics_common_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             zaxis=dict(range=[p_min[2], p_max[2]], autorange=False),
             # it's interesting that we have to do this to get the
             # axes aspect ratio right.. but hey! it works
             aspectratio=dict(
                 x=(p_max[0] - p_min[0]) / (ref_len / 4.0),
                 y=(p_max[1] - p_min[1]) / (ref_len / 4.0),
                 z=(p_max[2] - p_min[2]) / (ref_len / 4.0),
-            )
+            ),
             # note:
             # aspectmode='data': was causing issues with
             # the camera 'moving' across different animation frames
         )
     )
```

### Comparing `osmg-0.2.4/src/osmg/graphics/postprocessing_3d.py` & `osmg-0.2.5/src/osmg/graphics/postprocessing_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -229,42 +229,49 @@
         r_j = analysis.results[case_name].node_displacements[elm.nodes[1].uid][
             step
         ][3:6]
         # transferring them to the clear element ends
         if isinstance(elm, element.TrussBar):
             offset_i = np.zeros(3)
             offset_j = np.zeros(3)
-            x_vec, y_vec, z_vec = (
-                transformations.local_axes_from_points_and_angle(
-                    np.array(elm.nodes[0].coords),
-                    np.array(elm.nodes[1].coords),
-                    0.00))
+            (
+                x_vec,
+                y_vec,
+                z_vec,
+            ) = transformations.local_axes_from_points_and_angle(
+                np.array(elm.nodes[0].coords),
+                np.array(elm.nodes[1].coords),
+                0.00,
+            )
             outside_shape = elm.outside_shape
         else:
             offset_i = elm.geomtransf.offset_i
             offset_j = elm.geomtransf.offset_j
             x_vec = elm.geomtransf.x_axis
             y_vec = elm.geomtransf.y_axis
             z_vec = elm.geomtransf.z_axis
             outside_shape = elm.section.outside_shape
         u_i_o = transformations.offset_transformation(offset_i, u_i, r_i)
         u_j_o = transformations.offset_transformation(offset_j, u_j, r_j)
         if isinstance(elm, element.TrussBar):
-            d_global = np.column_stack((
-                np.linspace(u_i[0], u_j[0], num_points),
-                np.linspace(u_i[1], u_j[1], num_points),
-                np.linspace(u_i[2], u_j[2], num_points),
-            ))
+            d_global = np.column_stack(
+                (
+                    np.linspace(u_i[0], u_j[0], num_points),
+                    np.linspace(u_i[1], u_j[1], num_points),
+                    np.linspace(u_i[2], u_j[2], num_points),
+                )
+            )
             r_local = np.zeros((num_points, 3))
             interpolation_points = interp_3d_points(
                 elm, d_global, num_points, scaling
             )
         else:
             d_global, r_local = interp_3d_deformation(
-                elm, u_i_o, r_i, u_j_o, r_j, num_points)
+                elm, u_i_o, r_i, u_j_o, r_j, num_points
+            )
             interpolation_points = interp_3d_points(
                 elm, d_global, num_points, scaling
             )
         for i in range(num_points - 1):
             loc_i_global = interpolation_points[i, :]
             loc_j_global = interpolation_points[i + 1, :]
             rot_i_local = r_local[i, :]
@@ -322,36 +329,32 @@
                     )
                     * scaling
                 )
                 loc0 = loc_i_global + defo_ia_global
                 loc1 = loc_j_global + defo_ja_global
                 loc2 = loc_j_global + defo_jb_global
                 loc3 = loc_i_global + defo_ib_global
-                x_list.extend((
-                    loc0[0], loc1[0], loc2[0], loc3[0]))
-                y_list.extend((
-                    loc0[1], loc1[1], loc2[1], loc3[1]))
-                z_list.extend((
-                    loc0[2], loc1[2], loc2[2], loc3[2]))
-                i_list.extend((
-                    index + 0, index + 0))
-                j_list.extend((
-                    index + 1, index + 2))
-                k_list.extend((
-                    index + 2, index + 3))
+                x_list.extend((loc0[0], loc1[0], loc2[0], loc3[0]))
+                y_list.extend((loc0[1], loc1[1], loc2[1], loc3[1]))
+                z_list.extend((loc0[2], loc1[2], loc2[2], loc3[2]))
+                i_list.extend((index + 0, index + 0))
+                j_list.extend((index + 1, index + 2))
+                k_list.extend((index + 2, index + 3))
                 intensity.append(
-                    float(np.sqrt(d_global[i, :] @ d_global[i, :])))
+                    float(np.sqrt(d_global[i, :] @ d_global[i, :]))
+                )
                 intensity.append(
                     float(np.sqrt(d_global[i + 1, :] @ d_global[i + 1, :]))
                 )
                 intensity.append(
                     float(np.sqrt(d_global[i + 1, :] @ d_global[i + 1, :]))
                 )
                 intensity.append(
-                    float(np.sqrt(d_global[i, :] @ d_global[i, :])))
+                    float(np.sqrt(d_global[i, :] @ d_global[i, :]))
+                )
                 index += 4
     data_dict.append(
         {
             "type": "mesh3d",
             "x": x_list,
             "y": y_list,
             "z": z_list,
@@ -405,19 +408,21 @@
             u_i_o = transformations.offset_transformation(offset_i, u_i, r_i)
             u_j_o = transformations.offset_transformation(offset_j, u_j, r_j)
             d_global, _ = interp_3d_deformation(
                 elm, u_i_o, r_i, u_j_o, r_j, num_points
             )
         else:
             # for a truss member, just connect the two ends
-            d_global = np.column_stack((
-                np.linspace(u_i[0], u_j[0], num_points),
-                np.linspace(u_i[1], u_j[1], num_points),
-                np.linspace(u_i[2], u_j[2], num_points),
-            ))
+            d_global = np.column_stack(
+                (
+                    np.linspace(u_i[0], u_j[0], num_points),
+                    np.linspace(u_i[1], u_j[1], num_points),
+                    np.linspace(u_i[2], u_j[2], num_points),
+                )
+            )
         interpolation_points = interp_3d_points(
             elm, d_global, num_points, scaling
         )
         for i in range(len(interpolation_points) - 1):
             x_list.extend(
                 (
                     interpolation_points[i, 0],
@@ -535,15 +540,14 @@
     """
 
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
 
     for elm in list_of_line_elems:
-
         if isinstance(elm, element.TrussBar):
             p_i = np.array(elm.nodes[0].coords)
             p_j = np.array(elm.nodes[1].coords)
         else:
             p_i = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
             p_j = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
 
@@ -608,22 +612,24 @@
         {
             "type": "scatter3d",
             "mode": "markers",
             "x": location_data[:, 0] + displacement_data[:, 0] * scaling,
             "y": location_data[:, 1] + displacement_data[:, 1] * scaling,
             "z": location_data[:, 2] + displacement_data[:, 2] * scaling,
             "customdata": displacement_data,
-            "hovertemplate": "ux: %{customdata[0]:.6g}<br>"
-            + "uy: %{customdata[1]:.6g}<br>"
-            + "uz: %{customdata[2]:.6g}<br>"
-            + "combined: %{customdata[6]:.6g}<br>"
-            + "rx: %{customdata[3]:.6g} (rad)<br>"
-            + "ry: %{customdata[4]:.6g} (rad)<br>"
-            + "rz: %{customdata[5]:.6g} (rad)<br>"
-            + "<extra>Node %{customdata[7]:d}</extra>",
+            "hovertemplate": (
+                "ux: %{customdata[0]:.6g}<br>"
+                + "uy: %{customdata[1]:.6g}<br>"
+                + "uz: %{customdata[2]:.6g}<br>"
+                + "combined: %{customdata[6]:.6g}<br>"
+                + "rx: %{customdata[3]:.6g} (rad)<br>"
+                + "ry: %{customdata[4]:.6g} (rad)<br>"
+                + "rz: %{customdata[5]:.6g} (rad)<br>"
+                + "<extra>Node %{customdata[7]:d}</extra>"
+            ),
             "marker": {
                 "symbol": marker,
                 "color": color,
                 "size": size,
                 "line": {"color": color, "width": 4},
             },
         }
@@ -637,21 +643,17 @@
     the building's bounding box.
 
     """
 
     ref_len = mdl.reference_length()
     # maximum displacement
     max_d = 0.00
-    elms: list[
-        Union[element.ElasticBeamColumn,
-              element.DispBeamColumn]] = []
-    elms.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
-    elms.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+    elms: list[Union[element.ElasticBeamColumn, element.DispBeamColumn]] = []
+    elms.extend(mdl.list_of_specific_element(element.ElasticBeamColumn))
+    elms.extend(mdl.list_of_specific_element(element.DispBeamColumn))
 
     for elm in elms:
         u_i = analysis.results[case_name].node_displacements[elm.nodes[0].uid][
             step
         ][0:3]
         r_i = analysis.results[case_name].node_displacements[elm.nodes[0].uid][
             step
@@ -675,27 +677,26 @@
     # (usually when this is required, things have gone bad
     #  and we should be able to realize that immediately)
     scaling = max(scaling, 1.00)
     return scaling
 
 
 def show_deformed_shape(
-        analysis: Analysis,
-        case_name: str,
-        step: int,
-        scaling: float,
-        extrude: bool,
-        camera: Optional[dict[str, object]] = None,
-        subset_model: Model = None,
-        animation: bool = False,
-        init_step: int = 0,
-        step_skip: int = 0,
-        to_html_file: Optional[str] = None
+    analysis: Analysis,
+    case_name: str,
+    step: int,
+    scaling: float,
+    extrude: bool,
+    camera: Optional[dict[str, object]] = None,
+    subset_model: Model = None,
+    animation: bool = False,
+    init_step: int = 0,
+    step_skip: int = 0,
+    to_html_file: Optional[str] = None,
 ) -> dict[str, Any]:
-
     """
     Visualize the model in its deformed state
 
     Arguments:
       analysis: an analysis object
       case_name: the name of the load_case to be visualized
       step: the analysis step to be visualized
@@ -729,20 +730,21 @@
     # instantiate layout and datastructures
     layout = graphics_common_3d.global_layout(mdl, camera)
     data_dict: list[dict[str, object]] = []
     frame_data_dict: list[list[dict[str, object]]] = []
 
     # gather lists of associated objects
     list_of_line_elems: list[element.Element] = []
+    list_of_line_elems.extend(mdl.list_of_specific_element(element.TrussBar))
     list_of_line_elems.extend(
-        mdl.list_of_specific_element(element.TrussBar))
-    list_of_line_elems.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
+        mdl.list_of_specific_element(element.ElasticBeamColumn)
+    )
     list_of_line_elems.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+        mdl.list_of_specific_element(element.DispBeamColumn)
+    )
     list_of_primary_nodes = mdl.list_of_primary_nodes()
     list_of_internal_nodes = mdl.list_of_internal_nodes()
     # list_of_parent_nodes = mdl.list_of_parent_nodes()
 
     # add data for the global axes
     ref_len = mdl.reference_length()
 
@@ -796,15 +798,15 @@
             "mode": "immediate",
             "fromcurrent": True,
             "transition": {"duration": duration, "easing": "linear"},
         }
 
     if animation:
         step_of_frame = []
-        for j in range(first_step, step+1, step_skip + 1):
+        for j in range(first_step, step + 1, step_skip + 1):
             step_of_frame.append(j)
         for _, j in enumerate(step_of_frame):
             frame_data_dict.append([])
             add_data__global_axes(frame_data_dict[-1], ref_len)
             # add_data__global_axes(frame_data_dict[0], ref_len)
             add_data__nodes_deformed(
                 analysis,
@@ -930,15 +932,15 @@
     scaling_t,
     num_points,
     force_conversion=1.00,
     moment_conversion=1.00,
     global_axes=False,
     camera=None,
     subset_model=None,
-    to_html_file=None
+    to_html_file=None,
 ):
     """
     Visualize the model and plot the frame element basic forces.
 
     Arguments:
       analysis: an analysis object
       case_name: the name of the load_case to be visualized
@@ -968,28 +970,24 @@
 
     if subset_model:
         mdl = subset_model
     else:
         mdl = analysis.mdl
 
     elms: list[
-        Union[element.TrussBar,
-              element.ElasticBeamColumn,
-              element.DispBeamColumn]] = []
-    elms.extend(
-        mdl.list_of_specific_element(element.TrussBar))
-    elms.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
-    elms.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+        Union[
+            element.TrussBar, element.ElasticBeamColumn, element.DispBeamColumn
+        ]
+    ] = []
+    elms.extend(mdl.list_of_specific_element(element.TrussBar))
+    elms.extend(mdl.list_of_specific_element(element.ElasticBeamColumn))
+    elms.extend(mdl.list_of_specific_element(element.DispBeamColumn))
 
     list_of_line_elements = [
-        elm
-        for elm in elms
-        if not elm.visibility.skip_opensees_definition
+        elm for elm in elms if not elm.visibility.skip_opensees_definition
     ]
 
     layout = graphics_common_3d.global_layout(mdl, camera)
     data_dict: list[dict[str, object]] = []
 
     # draw the frames
     add_data__frames_undeformed(data_dict, list_of_line_elements)
@@ -1049,15 +1047,14 @@
     qy_vecs = {}
     qz_vecs = {}
     tx_vecs = {}
     mz_vecs = {}
     my_vecs = {}
 
     for elm in list_of_line_elements:
-
         if elm.visibility.hidden_basic_forces:
             continue
 
         forces = basic_forces(
             analysis, case_name, step, elm, num_points, as_tuple=True
         )
         assert isinstance(forces, tuple)
@@ -1111,46 +1108,49 @@
         scaling_m = scaling_my
     else:
         scaling_m = 0.00
     if scaling_m > 1.0e8:
         scaling_m = 1.00
 
     for elm in list_of_line_elements:
-
         if elm.visibility.hidden_basic_forces:
             continue
 
         # retrieve results from the preallocated arrays
         nx_vec = nx_vecs[elm.uid]
         qy_vec = qy_vecs[elm.uid]
         qz_vec = qz_vecs[elm.uid]
         tx_vec = tx_vecs[elm.uid]
         my_vec = my_vecs[elm.uid]
         mz_vec = mz_vecs[elm.uid]
         if isinstance(
-                elm, (element.ElasticBeamColumn, element.DispBeamColumn)):
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        ):
             x_vec = elm.geomtransf.x_axis
             y_vec = elm.geomtransf.y_axis
             z_vec = elm.geomtransf.z_axis
             i_pos = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
             p_i = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
             p_j = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
         else:
             p_i = np.array(elm.nodes[0].coords)
             p_j = np.array(elm.nodes[1].coords)
             i_pos = np.array(elm.nodes[0].coords)
-            x_vec, y_vec, z_vec = (
-                transformations.local_axes_from_points_and_angle(
-                    p_i, p_j, 0.00))
+            (
+                x_vec,
+                y_vec,
+                z_vec,
+            ) = transformations.local_axes_from_points_and_angle(
+                p_i, p_j, 0.00
+            )
 
         len_clr = np.linalg.norm(p_i - p_j)
         t_vec = np.linspace(0.00, len_clr, num=num_points)
 
         for i in range(num_points - 1):
-
             p_start = i_pos + t_vec[i] * x_vec
             p_end = i_pos + t_vec[i + 1] * x_vec
 
             # axial load
             p_i = p_start + nx_vec[i] * y_vec * scaling_n * scaling_global
             p_j = p_end + nx_vec[i + 1] * y_vec * scaling_n * scaling_global
 
@@ -1257,80 +1257,80 @@
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_a,
             "y": y1_a,
             "z": z1_a,
             "visible": False,
             "customdata": customdata_a,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_a},
         }
     ]
     dt_b = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_b,
             "y": y1_b,
             "z": z1_b,
             "visible": False,
             "customdata": customdata_b,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_b},
         }
     ]
     dt_c = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_c,
             "y": y1_c,
             "z": z1_c,
             "visible": False,
             "customdata": customdata_c,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_c},
         }
     ]
     dt_d = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_d,
             "y": y1_d,
             "z": z1_d,
             "visible": False,
             "customdata": customdata_d,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_d},
         }
     ]
     dt_e = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_e,
             "y": y1_e,
             "z": z1_e,
             "visible": False,
             "customdata": customdata_e,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_e},
         }
     ]
     dt_f = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_f,
             "y": y1_f,
             "z": z1_f,
             "visible": False,
             "customdata": customdata_f,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_f},
         }
     ]
 
     fig_datastructure = dict(
         data=data_dict + dt_a + dt_b + dt_c + dt_d + dt_e + dt_f, layout=layout
     )
@@ -1348,76 +1348,88 @@
                         ],
                     ),
                     dict(
                         label="Axial",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [True]
-                                + [False] * 5
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [True]
+                                    + [False] * 5
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Shear",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False]
-                                + [True]
-                                + [False] * 4
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False]
+                                    + [True]
+                                    + [False] * 4
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Moment",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False] * 2
-                                + [True]
-                                + [False] * 3
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False] * 2
+                                    + [True]
+                                    + [False] * 3
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Torsion",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False] * 3
-                                + [True]
-                                + [False] * 2
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False] * 3
+                                    + [True]
+                                    + [False] * 2
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Shear (combined)",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False] * 4
-                                + [True]
-                                + [False]
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False] * 4
+                                    + [True]
+                                    + [False]
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Moment (combined)",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False] * 5
-                                + [True]
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False] * 5
+                                    + [True]
+                                )
                             }
                         ],
                     ),
                 ],
             )
         ]
     )
@@ -1446,15 +1458,15 @@
     scaling_t,
     num_points,
     force_conversion=1.00,
     moment_conversion=1.00,
     global_axes=False,
     camera=None,
     subset_model=None,
-    to_html_file=None
+    to_html_file=None,
 ):
     """
     Visualize the model and plot the enveloped frame element basic forces
     for a load combination.
 
     Arguments:
       combo: a load combination object
@@ -1485,27 +1497,23 @@
     # TODO: merge code repetitions with the previous function
 
     if subset_model:
         mdl = subset_model
     else:
         mdl = combo.mdl
     elms: list[
-        Union[element.TrussBar,
-              element.ElasticBeamColumn,
-              element.DispBeamColumn]] = []
-    elms.extend(
-        mdl.list_of_specific_element(element.TrussBar))
-    elms.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
-    elms.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+        Union[
+            element.TrussBar, element.ElasticBeamColumn, element.DispBeamColumn
+        ]
+    ] = []
+    elms.extend(mdl.list_of_specific_element(element.TrussBar))
+    elms.extend(mdl.list_of_specific_element(element.ElasticBeamColumn))
+    elms.extend(mdl.list_of_specific_element(element.DispBeamColumn))
     list_of_line_elements = [
-        elm
-        for elm in elms
-        if not elm.visibility.skip_opensees_definition
+        elm for elm in elms if not elm.visibility.skip_opensees_definition
     ]
 
     layout = graphics_common_3d.global_layout(mdl, camera)
     data_dict: list[dict[str, object]] = []
 
     # draw the frames
     add_data__frames_undeformed(data_dict, list_of_line_elements)
@@ -1559,15 +1567,14 @@
     qy_vecs_max = {}
     qz_vecs_max = {}
     tx_vecs_max = {}
     mz_vecs_max = {}
     my_vecs_max = {}
 
     for elm in list_of_line_elements:
-
         if elm.visibility.hidden_basic_forces:
             continue
 
         df_min, df_max = combo.envelope_basic_forces(elm, num_points)
 
         # store results in the preallocated arrays
 
@@ -1647,15 +1654,14 @@
         scaling_m = scaling_my
     else:
         scaling_m = 0.00
     if scaling_m > 1.0e8:
         scaling_m = 1.00
 
     for elm in list_of_line_elements:
-
         if elm.visibility.hidden_basic_forces:
             continue
 
         # retrieve results from the preallocated arrays
         nx_vec_min = nx_vecs_min[elm.uid]
         qy_vec_min = qy_vecs_min[elm.uid]
         qz_vec_min = qz_vecs_min[elm.uid]
@@ -1667,34 +1673,38 @@
         qy_vec_max = qy_vecs_max[elm.uid]
         qz_vec_max = qz_vecs_max[elm.uid]
         tx_vec_max = tx_vecs_max[elm.uid]
         my_vec_max = my_vecs_max[elm.uid]
         mz_vec_max = mz_vecs_max[elm.uid]
 
         if isinstance(
-                elm, (element.ElasticBeamColumn, element.DispBeamColumn)):
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        ):
             x_vec = elm.geomtransf.x_axis
             y_vec = elm.geomtransf.y_axis
             z_vec = elm.geomtransf.z_axis
             i_pos = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
             p_i = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
             p_j = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
         else:
             p_i = np.array(elm.nodes[0].coords)
             p_j = np.array(elm.nodes[1].coords)
             i_pos = np.array(elm.nodes[0].coords)
-            x_vec, y_vec, z_vec = (
-                transformations.local_axes_from_points_and_angle(
-                    p_i, p_j, 0.00))
+            (
+                x_vec,
+                y_vec,
+                z_vec,
+            ) = transformations.local_axes_from_points_and_angle(
+                p_i, p_j, 0.00
+            )
 
         len_clr = np.linalg.norm(p_i - p_j)
         t_vec = np.linspace(0.00, len_clr, num=num_points)
 
         for i in range(num_points - 1):
-
             p_start = i_pos + t_vec[i] * x_vec
             p_end = i_pos + t_vec[i + 1] * x_vec
 
             # axial load
             p_i = p_start + nx_vec_min[i] * y_vec * scaling_n * scaling_global
             p_j = (
                 p_end + nx_vec_min[i + 1] * y_vec * scaling_n * scaling_global
@@ -1818,54 +1828,54 @@
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_a,
             "y": y1_a,
             "z": z1_a,
             "visible": False,
             "customdata": customdata_a,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_a},
         }
     ]
     dt_b = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_b,
             "y": y1_b,
             "z": z1_b,
             "visible": False,
             "customdata": customdata_b,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_b},
         }
     ]
     dt_c = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_c,
             "y": y1_c,
             "z": z1_c,
             "visible": False,
             "customdata": customdata_c,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_c},
         }
     ]
     dt_d = [
         {
             "type": "scatter3d",
             "mode": "lines",
             "x": x1_d,
             "y": y1_d,
             "z": z1_d,
             "visible": False,
             "customdata": customdata_d,
-            "hovertemplate": " %{customdata:.0f}<br>" "<extra></extra>",
+            "hovertemplate": " %{customdata:.0f}<br><extra></extra>",
             "line": {"width": 3, "color": colors1_d},
         }
     ]
 
     fig_datastructure = dict(
         data=data_dict + dt_a + dt_b + dt_c + dt_d, layout=layout
     )
@@ -1883,52 +1893,60 @@
                         ],
                     ),
                     dict(
                         label="Axial",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [True]
-                                + [False] * 3
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [True]
+                                    + [False] * 3
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Shear",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False]
-                                + [True]
-                                + [False] * 2
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False]
+                                    + [True]
+                                    + [False] * 2
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Moment",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False] * 2
-                                + [True]
-                                + [False]
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False] * 2
+                                    + [True]
+                                    + [False]
+                                )
                             }
                         ],
                     ),
                     dict(
                         label="Torsion",
                         method="update",
                         args=[
                             {
-                                "visible": [True] * len(data_dict)
-                                + [False] * 3
-                                + [True]
+                                "visible": (
+                                    [True] * len(data_dict)
+                                    + [False] * 3
+                                    + [True]
+                                )
                             }
                         ],
                     ),
                 ],
             )
         ]
     )
```

### Comparing `osmg-0.2.4/src/osmg/graphics/preprocessing_3d.py` & `osmg-0.2.5/src/osmg/graphics/preprocessing_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,26 +80,27 @@
                 "type": "scatter3d",
                 "mode": "markers",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "customdata": customdata,
                 "text": restraints,
-                "hovertemplate": "Coordinates: "
-                "(%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
-                + "Restraint: %{text}<br>"
-                + "Mass: (%{customdata[1]:.3g}, "
-                + "%{customdata[2]:.3g}, %{customdata[3]:.3g}, "
-                + "%{customdata[4]:.3g}, %{customdata[5]:.3g}, "
-                + "%{customdata[6]:.3g})<br>"
-                + "Load: (%{customdata[7]:.3g}, "
-                + "%{customdata[8]:.3g}, %{customdata[9]:.3g}, "
-                + "%{customdata[10]:.3g}, %{customdata[11]:.3g}, "
-                + "%{customdata[12]:.3g})"
-                + "<extra>Node: %{customdata[0]:d}</extra>",
+                "hovertemplate": (
+                    "Coordinates: (%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
+                    + "Restraint: %{text}<br>"
+                    + "Mass: (%{customdata[1]:.3g}, "
+                    + "%{customdata[2]:.3g}, %{customdata[3]:.3g}, "
+                    + "%{customdata[4]:.3g}, %{customdata[5]:.3g}, "
+                    + "%{customdata[6]:.3g})<br>"
+                    + "Load: (%{customdata[7]:.3g}, "
+                    + "%{customdata[8]:.3g}, %{customdata[9]:.3g}, "
+                    + "%{customdata[10]:.3g}, %{customdata[11]:.3g}, "
+                    + "%{customdata[12]:.3g})"
+                    + "<extra>Node: %{customdata[0]:d}</extra>"
+                ),
                 "marker": {
                     "symbol": [
                         graphics_common_3d.node_marker[sym][0]
                         for sym in restraint_symbols
                     ],
                     "color": graphics_common.NODE_PRIMARY_COLOR,
                     "size": [
@@ -120,18 +121,19 @@
                 "type": "scatter3d",
                 "mode": "markers",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "customdata": customdata,
                 "text": restraints,
-                "hovertemplate": "Coordinates: "
-                "(%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
-                + "Restraint: %{text}<br>"
-                + "<extra>Node: %{customdata[0]:d}</extra>",
+                "hovertemplate": (
+                    "Coordinates: (%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
+                    + "Restraint: %{text}<br>"
+                    + "<extra>Node: %{customdata[0]:d}</extra>"
+                ),
                 "marker": {
                     "symbol": [
                         graphics_common_3d.node_marker[sym][0]
                         for sym in restraint_symbols
                     ],
                     "color": graphics_common.NODE_PRIMARY_COLOR,
                     "size": [
@@ -144,16 +146,16 @@
                     },
                 },
             }
         )
 
 
 def add_data__parent_nodes(
-        data_dict: list[dict[str, object]],
-        load_case: LoadCase) -> None:
+    data_dict: list[dict[str, object]], load_case: LoadCase
+) -> None:
     """
     Adds a trace containing parent nodes
 
     Arguments:
       data_dict:
         list of dictionaries containing figure data
       mdl: the model to be visualized
@@ -182,45 +184,47 @@
             "type": "scatter3d",
             "mode": "markers",
             "x": x_list,
             "y": y_list,
             "z": z_list,
             "customdata": customdata,
             "text": restraints,
-            "hovertemplate": "Coordinates: (%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
-            + "Restraint: %{text}<br>"
-            + "Mass: (%{customdata[1]:.3g}, "
-            + "%{customdata[2]:.3g}, %{customdata[3]:.3g}, "
-            + "%{customdata[4]:.3g}, %{customdata[5]:.3g}, "
-            + "%{customdata[6]:.3g})<br>"
-            + "Load: (%{customdata[7]:.3g}, "
-            + "%{customdata[8]:.3g}, %{customdata[9]:.3g}, "
-            + "%{customdata[10]:.3g}, %{customdata[11]:.3g}, "
-            + "%{customdata[12]:.3g})"
-            + "<extra>Parent Node: %{customdata[0]:d}</extra>",
+            "hovertemplate": (
+                "Coordinates: (%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
+                + "Restraint: %{text}<br>"
+                + "Mass: (%{customdata[1]:.3g}, "
+                + "%{customdata[2]:.3g}, %{customdata[3]:.3g}, "
+                + "%{customdata[4]:.3g}, %{customdata[5]:.3g}, "
+                + "%{customdata[6]:.3g})<br>"
+                + "Load: (%{customdata[7]:.3g}, "
+                + "%{customdata[8]:.3g}, %{customdata[9]:.3g}, "
+                + "%{customdata[10]:.3g}, %{customdata[11]:.3g}, "
+                + "%{customdata[12]:.3g})"
+                + "<extra>Parent Node: %{customdata[0]:d}</extra>"
+            ),
             "marker": {
-                "symbol": [
-                    graphics_common_3d.node_marker[
-                        "parent"][0]]*len(list_of_nodes),
+                "symbol": [graphics_common_3d.node_marker["parent"][0]]
+                * len(list_of_nodes),
                 "color": graphics_common.NODE_PRIMARY_COLOR,
-                "size": [
-                    graphics_common_3d.node_marker[
-                        "parent"][1]]*len(list_of_nodes),
+                "size": [graphics_common_3d.node_marker["parent"][1]]
+                * len(list_of_nodes),
                 "line": {
                     "color": graphics_common.NODE_PRIMARY_COLOR,
                     "width": 4,
                 },
             },
         }
     )
 
 
 def add_data__internal_nodes(
-        data_dict: list[dict[str, object]],
-        mdl: Model, load_case: Optional[LoadCase] = None) -> None:
+    data_dict: list[dict[str, object]],
+    mdl: Model,
+    load_case: Optional[LoadCase] = None,
+) -> None:
     """
     Adds a trace containing internal nodes
 
     Arguments:
       data_dict:
         list of dictionaries containing figure data
       mdl: the model to be visualized
@@ -260,22 +264,23 @@
                 "type": "scatter3d",
                 "mode": "markers",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "customdata": customdata,
                 "text": restraints,
-                "hovertemplate": "Coordinates: "
-                "(%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
-                + "Restraint: %{text}<br>"
-                + "Mass: (%{customdata[1]:.3g}, "
-                + "%{customdata[2]:.3g}, %{customdata[3]:.3g})<br>"
-                + "Load: (%{customdata[4]:.3g}, "
-                + "%{customdata[5]:.3g}, %{customdata[6]:.3g})"
-                + "<extra>Node: %{customdata[0]:d}</extra>",
+                "hovertemplate": (
+                    "Coordinates: (%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
+                    + "Restraint: %{text}<br>"
+                    + "Mass: (%{customdata[1]:.3g}, "
+                    + "%{customdata[2]:.3g}, %{customdata[3]:.3g})<br>"
+                    + "Load: (%{customdata[4]:.3g}, "
+                    + "%{customdata[5]:.3g}, %{customdata[6]:.3g})"
+                    + "<extra>Node: %{customdata[0]:d}</extra>"
+                ),
                 "marker": {
                     "symbol": [
                         graphics_common_3d.node_marker[sym][0]
                         for sym in restraint_symbols
                     ],
                     "color": graphics_common.NODE_INTERNAL_COLOR,
                     "size": [
@@ -296,18 +301,19 @@
                 "type": "scatter3d",
                 "mode": "markers",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "customdata": customdata,
                 "text": restraints,
-                "hovertemplate": "Coordinates: "
-                "(%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
-                + "Restraint: %{text}<br>"
-                + "<extra>Node: %{customdata[0]:d}</extra>",
+                "hovertemplate": (
+                    "Coordinates: (%{x:.2f}, %{y:.2f}, %{z:.2f})<br>"
+                    + "Restraint: %{text}<br>"
+                    + "<extra>Node: %{customdata[0]:d}</extra>"
+                ),
                 "marker": {
                     "symbol": [
                         graphics_common_3d.node_marker[sym][0]
                         for sym in restraint_symbols
                     ],
                     "color": graphics_common.NODE_INTERNAL_COLOR,
                     "size": [
@@ -320,16 +326,16 @@
                     },
                 },
             }
         )
 
 
 def add_data__release_nodes(
-        data_dict: list[dict[str, object]],
-        list_of_nodes: list[node_module.Node]) -> None:
+    data_dict: list[dict[str, object]], list_of_nodes: list[node_module.Node]
+) -> None:
     """
     Adds a trace containing release nodes
 
     Arguments:
       data_dict:
         list of dictionaries containing figure data
       list_of_nodes: List of nodes where a release is present.
@@ -359,41 +365,45 @@
                 },
             },
         }
     )
 
 
 def add_data__frames(
-        data_dict: list[dict[str, object]],
-        mdl: Model,
-        load_case: Optional[LoadCase] = None) -> None:
+    data_dict: list[dict[str, object]],
+    mdl: Model,
+    load_case: Optional[LoadCase] = None,
+) -> None:
     """
     Adds a trace containing frame element centroidal axis lines
 
     Arguments:
       data_dict:
         list of dictionaries containing figure data
       mdl: the model to be visualized
       load_case: the load_case to be visualized
 
     """
 
     line_elems: list[
-        Union[element.ElasticBeamColumn,
-              element.DispBeamColumn]] = []
+        Union[element.ElasticBeamColumn, element.DispBeamColumn]
+    ] = []
 
     # >>>
     # it feels ridiculous to do this, but it's the only way I am
     # getting rid of type checking warnings.
     elms_elastic = [
-        elm for elm in mdl.list_of_specific_element(element.ElasticBeamColumn)
-        if isinstance(elm, element.ElasticBeamColumn)]
+        elm
+        for elm in mdl.list_of_specific_element(element.ElasticBeamColumn)
+        if isinstance(elm, element.ElasticBeamColumn)
+    ]
     line_elems.extend(elms_elastic)
     elms_disp = [
-        elm for elm in mdl.list_of_specific_element(element.DispBeamColumn)
+        elm
+        for elm in mdl.list_of_specific_element(element.DispBeamColumn)
         if isinstance(elm, element.DispBeamColumn)
     ]
     line_elems.extend(elms_disp)
     # <<<
 
     if not line_elems:
         return
@@ -448,20 +458,22 @@
                 "type": "scatter3d",
                 "mode": "lines",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "text": section_names,
                 "customdata": customdata,
-                "hovertemplate": "Section: %{text}<br>"
-                + "UDL (local): (%{customdata[1]:.3g}, "
-                + "%{customdata[2]:.3g}, %{customdata[3]:.3g})"
-                + "<extra>Element: %{customdata[0]:d}<br>"
-                + "Node @ this end: %{customdata[4]:d}<br>"
-                "Parent: %{customdata[5]}</extra>",
+                "hovertemplate": (
+                    "Section: %{text}<br>"
+                    + "UDL (local): (%{customdata[1]:.3g}, "
+                    + "%{customdata[2]:.3g}, %{customdata[3]:.3g})"
+                    + "<extra>Element: %{customdata[0]:d}<br>"
+                    + "Node @ this end: %{customdata[4]:d}<br>"
+                    "Parent: %{customdata[5]}</extra>"
+                ),
                 "line": {"width": 5, "color": graphics_common.FRAME_COLOR},
             }
         )
     else:
         customdata = np.array(customdata_list, dtype="object")
         data_dict.append(
             {
@@ -469,39 +481,45 @@
                 "type": "scatter3d",
                 "mode": "lines",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "text": section_names,
                 "customdata": customdata,
-                "hovertemplate": "Section: %{text}<br>"
-                + "<extra>Element: %{customdata[0]:d}<br>"
-                + "Node @ this end: %{customdata[1]:d}<br>"
-                "Parent: %{customdata[2]}</extra>",
+                "hovertemplate": (
+                    "Section: %{text}<br>"
+                    + "<extra>Element: %{customdata[0]:d}<br>"
+                    + "Node @ this end: %{customdata[1]:d}<br>"
+                    "Parent: %{customdata[2]}</extra>"
+                ),
                 "line": {"width": 5, "color": graphics_common.FRAME_COLOR},
             }
         )
 
 
 def add_data__bars(
-        data_dict: list[dict[str, object]],
-        mdl: Model,
-        load_case: Optional[LoadCase] = None) -> None:
+    data_dict: list[dict[str, object]],
+    mdl: Model,
+    load_case: Optional[LoadCase] = None,
+) -> None:
     """
     Adds a trace containing frame element centroidal axis lines
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
       load_case: the load_case to be visualized
 
     """
 
-    line_elems = [elm for elm in mdl.list_of_specific_element(element.TrussBar)
-                  if isinstance(elm, element.TrussBar)]
+    line_elems = [
+        elm
+        for elm in mdl.list_of_specific_element(element.TrussBar)
+        if isinstance(elm, element.TrussBar)
+    ]
     if not line_elems:
         return
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
     customdata_list: list[tuple[Any, ...]] = []
     section_areas = []
@@ -549,18 +567,20 @@
                 "type": "scatter3d",
                 "mode": "lines",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "text": section_areas,
                 "customdata": customdata,
-                "hovertemplate": "Section area: %{text}<br>"
-                + "<extra>Element: %{customdata[0]:d}<br>"
-                + "Node @ this end: %{customdata[1]:d}<br>"
-                "Parent: %{customdata[2]}</extra>",
+                "hovertemplate": (
+                    "Section area: %{text}<br>"
+                    + "<extra>Element: %{customdata[0]:d}<br>"
+                    + "Node @ this end: %{customdata[1]:d}<br>"
+                    "Parent: %{customdata[2]}</extra>"
+                ),
                 "line": {"width": 5, "color": graphics_common.FRAME_COLOR},
             }
         )
     else:
         customdata = np.array(customdata_list, dtype="object")
         data_dict.append(
             {
@@ -568,39 +588,42 @@
                 "type": "scatter3d",
                 "mode": "lines",
                 "x": x_list,
                 "y": y_list,
                 "z": z_list,
                 "text": section_areas,
                 "customdata": customdata,
-                "hovertemplate": "Section area: %{text}<br>"
-                + "<extra>Element: %{customdata[0]:d}<br>"
-                + "Node @ this end: %{customdata[1]:d}<br>"
-                "Parent: %{customdata[2]}</extra>",
+                "hovertemplate": (
+                    "Section area: %{text}<br>"
+                    + "<extra>Element: %{customdata[0]:d}<br>"
+                    + "Node @ this end: %{customdata[1]:d}<br>"
+                    "Parent: %{customdata[2]}</extra>"
+                ),
                 "line": {"width": 5, "color": graphics_common.FRAME_COLOR},
             }
         )
 
 
 def add_data__twonodelinks(
-        data_dict: list[dict[str, object]],
-        mdl: Model) -> None:
+    data_dict: list[dict[str, object]], mdl: Model
+) -> None:
     """
     Adds a trace containing twonodelink elements
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
 
     """
 
     link_elems = [
         elm
         for elm in mdl.list_of_elements()
-        if isinstance(elm, element.TwoNodeLink)]
+        if isinstance(elm, element.TwoNodeLink)
+    ]
 
     if not link_elems:
         return
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
     customdata_list: list[tuple[Any, ...]] = []
@@ -625,52 +648,56 @@
             "type": "scatter3d",
             "mode": "lines",
             "x": x_list,
             "y": y_list,
             "z": z_list,
             # "text": section_names,
             "customdata": customdata,
-            "hovertemplate": "Section: %{text}<br>"
-            + "<extra>Element: %{customdata[0]:d}<br>"
-            + "Node @ this end: %{customdata[1]:d}<br>"
-            "Parent: %{customdata[2]}</extra>",
+            "hovertemplate": (
+                "Section: %{text}<br>"
+                + "<extra>Element: %{customdata[0]:d}<br>"
+                + "Node @ this end: %{customdata[1]:d}<br>"
+                "Parent: %{customdata[2]}</extra>"
+            ),
             "line": {"width": 5, "color": graphics_common.LINK_COLOR},
         }
     )
 
 
 def add_data__frame_offsets(
-        data_dict: list[dict[str, object]],
-        mdl: Model) -> None:
+    data_dict: list[dict[str, object]], mdl: Model
+) -> None:
     """
     Adds a trace containing frame element rigid offset lines
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
 
     """
 
-    beamcolumn_elems: list[
-        element.Element] = []
+    beamcolumn_elems: list[element.Element] = []
     beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
+        mdl.list_of_specific_element(element.ElasticBeamColumn)
+    )
     beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+        mdl.list_of_specific_element(element.DispBeamColumn)
+    )
 
     if not beamcolumn_elems:
         return
 
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
 
     for elm in beamcolumn_elems:
         assert isinstance(
-            elm, (element.ElasticBeamColumn, element.DispBeamColumn))
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        )
         p_i: nparr = np.array(elm.nodes[0].coords)
         p_io: nparr = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
         p_j: nparr = np.array(elm.nodes[1].coords)
         p_jo: nparr = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
 
         x_list.extend((p_i[0], p_io[0], None))
         y_list.extend((p_i[1], p_io[1], None))
@@ -690,44 +717,45 @@
             "hoverinfo": "skip",
             "line": {"width": 8, "color": graphics_common.OFFSET_COLOR},
         }
     )
 
 
 def add_data__frame_axes(
-        data_dict: list[dict[str, object]],
-        mdl: Model,
-        ref_len: float) -> None:
+    data_dict: list[dict[str, object]], mdl: Model, ref_len: float
+) -> None:
     """
     Adds a trace containing frame element local axis lines
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
       ref_len: model reference length to scale the axes
 
     """
 
     beamcolumn_elems: list[element.Element] = []
+    beamcolumn_elems.extend(mdl.list_of_specific_element(element.TrussBar))
     beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.TrussBar))
-    beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
+        mdl.list_of_specific_element(element.ElasticBeamColumn)
+    )
     beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+        mdl.list_of_specific_element(element.DispBeamColumn)
+    )
     if not beamcolumn_elems:
         return
     scaling = ref_len * 0.025
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
     colors: list[Optional[str]] = []
     for elm in beamcolumn_elems:
         assert isinstance(
-            elm, (element.ElasticBeamColumn, element.DispBeamColumn))
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        )
         if elm.visibility.hidden_at_line_plots:
             continue
         x_vec = elm.geomtransf.x_axis
         y_vec = elm.geomtransf.y_axis
         z_vec = elm.geomtransf.z_axis
         l_clear = elm.clear_length()
         i_pos = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
@@ -755,29 +783,30 @@
             "hoverinfo": "skip",
             "line": {"width": 8, "color": colors},
         }
     )
 
 
 def add_data__zerolength_axes(
-        data_dict: list[dict[str, object]],
-        mdl: Model, ref_len: float) -> None:
+    data_dict: list[dict[str, object]], mdl: Model, ref_len: float
+) -> None:
     """
     Adds a trace containing zerolength element local axis lines
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
       ref_len: model reference length to scale the axes
 
     """
 
     zerolength_elements: list[element.Element] = []
     zerolength_elements.extend(
-        mdl.list_of_specific_element(element.ZeroLength))
+        mdl.list_of_specific_element(element.ZeroLength)
+    )
     if not zerolength_elements:
         return
     scaling = ref_len * 0.025
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
     colors: list[Optional[str]] = []
@@ -810,16 +839,16 @@
             "hoverinfo": "skip",
             "line": {"width": 8, "color": colors},
         }
     )
 
 
 def add_data__global_axes(
-        data_dict: list[dict[str, object]],
-        ref_len: float) -> None:
+    data_dict: list[dict[str, object]], ref_len: float
+) -> None:
     """
     Adds a trace containing global axes
 
     Arguments:
       data_dict: dictionary containing figure data
       ref_len: model reference length to scale the axes
 
@@ -861,16 +890,16 @@
             }
         ]
         * 2
     )
 
 
 def add_data__diaphragm_lines(
-        data_dict: list[dict[str, object]],
-        loadcase: LoadCase) -> None:
+    data_dict: list[dict[str, object]], loadcase: LoadCase
+) -> None:
     """
     Adds a trace containing lines indicating rigid diaphragm
     constraints.
 
     Arguments:
       data_dict: dictionary containing figure data
       loadcase: loadcase
@@ -887,15 +916,14 @@
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
 
     # for each level that has a parent node, draw the lines
     mdl = loadcase.parent_model
     for lvl_uid, pnode in pnodes.items():
-
         level = mdl.levels[lvl_uid]
         level_primary_nodes = level.nodes.values()
         for node in level_primary_nodes:
             if node.coords[2] == level.elevation:
                 x_list.extend((node.coords[0], pnode.coords[0], None))
                 y_list.extend((node.coords[1], pnode.coords[1], None))
                 z_list.extend((level.elevation, level.elevation, None))
@@ -911,16 +939,16 @@
             "hoverinfo": "skip",
             "line": {"width": 2, "color": graphics_common.GRID_COLOR},
         }
     )
 
 
 def add_data__tributary_area_boundaries(
-        data_dict: list[dict[str, object]],
-        loadcase: LoadCase) -> None:
+    data_dict: list[dict[str, object]], loadcase: LoadCase
+) -> None:
     """
     Adds a trace containing lines indicating tributary area boundaries
     that are used for load distribution.
 
     Arguments:
       data_dict: dictionary containing figure data
       loadcase: loadcase
@@ -930,28 +958,27 @@
     trib_area_analysis_collection = loadcase.tributary_area_analysis
 
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
 
     for analysis in trib_area_analysis_collection.values():
-
         level = analysis.parent_level
         data = analysis.data
         edge_polygons = data.edge_polygons
 
         for polygon_list in edge_polygons.values():
             for polygon in polygon_list:
                 x_vals = [v[0] for v in polygon]
                 y_vals = [v[1] for v in polygon]
                 x_vals.append(x_vals[0])
                 y_vals.append(y_vals[0])
                 x_list.extend((*x_vals, None))
                 y_list.extend((*y_vals, None))
-                z_list.extend((*[level.elevation]*len(x_vals), None))
+                z_list.extend((*[level.elevation] * len(x_vals), None))
 
     data_dict.append(
         {
             "name": "Trib. Area",
             "type": "scatter3d",
             "mode": "lines",
             "x": x_list,
@@ -960,41 +987,45 @@
             "hoverinfo": "skip",
             "line": {"width": 2, "color": graphics_common.BISECTOR_COLOR},
         }
     )
 
 
 def add_data__extruded_frames_mesh(
-        data_dict: list[dict[str, object]], mdl: Model) -> None:
+    data_dict: list[dict[str, object]], mdl: Model
+) -> None:
     """
     Adds a trace containing frame element extrusion mesh
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
 
     """
 
     beamcolumn_elems: list[element.Element] = []
     beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.ElasticBeamColumn))
+        mdl.list_of_specific_element(element.ElasticBeamColumn)
+    )
     beamcolumn_elems.extend(
-        mdl.list_of_specific_element(element.DispBeamColumn))
+        mdl.list_of_specific_element(element.DispBeamColumn)
+    )
     if not beamcolumn_elems:
         return
     x_list: list[Optional[float]] = []
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
     i_list: list[Optional[int]] = []
     j_list: list[Optional[int]] = []
     k_list: list[Optional[int]] = []
     index = 0
     for elm in beamcolumn_elems:
         assert isinstance(
-            elm, (element.ElasticBeamColumn, element.DispBeamColumn))
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        )
         if elm.visibility.hidden_when_extruded:
             continue
         side_a = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
         side_b = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
         y_vec = elm.geomtransf.y_axis
         z_vec = elm.geomtransf.z_axis
         if not elm.section.outside_shape:
@@ -1002,39 +1033,37 @@
         loop = elm.section.outside_shape.halfedges
         for halfedge in loop:
             assert halfedge.nxt is not None
             assert halfedge.nxt.vertex is not None
             loc0 = (
                 halfedge.vertex.coords[0] * z_vec
                 + halfedge.vertex.coords[1] * y_vec
-                + side_a)
+                + side_a
+            )
             loc1 = (
                 halfedge.vertex.coords[0] * z_vec
                 + halfedge.vertex.coords[1] * y_vec
-                + side_b)
+                + side_b
+            )
             loc2 = (
                 halfedge.nxt.vertex.coords[0] * z_vec
                 + halfedge.nxt.vertex.coords[1] * y_vec
-                + side_b)
+                + side_b
+            )
             loc3 = (
                 halfedge.nxt.vertex.coords[0] * z_vec
                 + halfedge.nxt.vertex.coords[1] * y_vec
-                + side_a)
-            x_list.extend((
-                loc0[0], loc1[0], loc2[0], loc3[0]))
-            y_list.extend((
-                loc0[1], loc1[1], loc2[1], loc3[1]))
-            z_list.extend((
-                loc0[2], loc1[2], loc2[2], loc3[2]))
-            i_list.extend((
-                index + 0, index + 0))
-            j_list.extend((
-                index + 1, index + 2))
-            k_list.extend((
-                index + 2, index + 3))
+                + side_a
+            )
+            x_list.extend((loc0[0], loc1[0], loc2[0], loc3[0]))
+            y_list.extend((loc0[1], loc1[1], loc2[1], loc3[1]))
+            z_list.extend((loc0[2], loc1[2], loc2[2], loc3[2]))
+            i_list.extend((index + 0, index + 0))
+            j_list.extend((index + 1, index + 2))
+            k_list.extend((index + 2, index + 3))
             index += 4
     data_dict.append(
         {
             "type": "mesh3d",
             "x": x_list,
             "y": y_list,
             "z": z_list,
@@ -1045,15 +1074,16 @@
             "color": graphics_common.BEAM_MESH_COLOR,
             "opacity": 0.70,
         }
     )
 
 
 def add_data__extruded_bars_mesh(
-        data_dict: list[dict[str, object]], mdl: Model) -> None:
+    data_dict: list[dict[str, object]], mdl: Model
+) -> None:
     """
     Adds a trace containing frame element extrusion mesh
 
     Arguments:
       data_dict: dictionary containing figure data
       mdl: the model to be visualized
 
@@ -1066,15 +1096,14 @@
     y_list: list[Optional[float]] = []
     z_list: list[Optional[float]] = []
     i_list: list[Optional[int]] = []
     j_list: list[Optional[int]] = []
     k_list: list[Optional[int]] = []
     index = 0
     for elm in line_elems:
-
         assert isinstance(elm, element.TrussBar)
         if elm.visibility.hidden_when_extruded:
             continue
         if not elm.outside_shape:
             continue
 
         side_a = np.array(elm.nodes[0].coords)
@@ -1091,39 +1120,37 @@
 
         loop = elm.outside_shape.halfedges
         for halfedge in loop:
             assert halfedge.nxt
             loc0 = (
                 halfedge.vertex.coords[0] * z_vec
                 + halfedge.vertex.coords[1] * y_vec
-                + side_a)
+                + side_a
+            )
             loc1 = (
                 halfedge.vertex.coords[0] * z_vec
                 + halfedge.vertex.coords[1] * y_vec
-                + side_b)
+                + side_b
+            )
             loc2 = (
                 halfedge.nxt.vertex.coords[0] * z_vec
                 + halfedge.nxt.vertex.coords[1] * y_vec
-                + side_b)
+                + side_b
+            )
             loc3 = (
                 halfedge.nxt.vertex.coords[0] * z_vec
                 + halfedge.nxt.vertex.coords[1] * y_vec
-                + side_a)
-            x_list.extend((
-                loc0[0], loc1[0], loc2[0], loc3[0]))
-            y_list.extend((
-                loc0[1], loc1[1], loc2[1], loc3[1]))
-            z_list.extend((
-                loc0[2], loc1[2], loc2[2], loc3[2]))
-            i_list.extend((
-                index + 0, index + 0))
-            j_list.extend((
-                index + 1, index + 2))
-            k_list.extend((
-                index + 2, index + 3))
+                + side_a
+            )
+            x_list.extend((loc0[0], loc1[0], loc2[0], loc3[0]))
+            y_list.extend((loc0[1], loc1[1], loc2[1], loc3[1]))
+            z_list.extend((loc0[2], loc1[2], loc2[2], loc3[2]))
+            i_list.extend((index + 0, index + 0))
+            j_list.extend((index + 1, index + 2))
+            k_list.extend((index + 2, index + 3))
             index += 4
     data_dict.append(
         {
             "type": "mesh3d",
             "x": x_list,
             "y": y_list,
             "z": z_list,
@@ -1134,27 +1161,28 @@
             "color": graphics_common.BEAM_MESH_COLOR,
             "opacity": 0.30,
         }
     )
 
 
 def show(
-        mdl: Model,
-        load_case: Optional[LoadCase] = None,
-        extrude: bool = False,
-        offsets: bool = True,
-        global_axes: bool = True,
-        parent_nodes: bool = True,
-        frame_axes: bool = False,
-        zerolength_axes: bool = False,
-        diaphragm_lines: bool = True,
-        tributary_area_boundaries: bool = True,
-        camera: Optional[dict[str, object]] = None,
-        to_html_file: Optional[str] = None,
-        to_figure: Optional[str] = None) -> None:
+    mdl: Model,
+    load_case: Optional[LoadCase] = None,
+    extrude: bool = False,
+    offsets: bool = True,
+    global_axes: bool = True,
+    parent_nodes: bool = True,
+    frame_axes: bool = False,
+    zerolength_axes: bool = False,
+    diaphragm_lines: bool = True,
+    tributary_area_boundaries: bool = True,
+    camera: Optional[dict[str, object]] = None,
+    to_html_file: Optional[str] = None,
+    to_figure: Optional[str] = None,
+) -> None:
     """
     Visualize the model
 
     Arguments:
       mdl: the model to be visualized
       load_case: the load_case to be visualized
       extrude: wether to extrude frame elements
```

### Comparing `osmg-0.2.4/src/osmg/graphics/visibility.py` & `osmg-0.2.5/src/osmg/graphics/visibility.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/ground_motion_utils.py` & `osmg-0.2.5/src/osmg/ground_motion_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,22 +33,18 @@
         for i, line in enumerate(file):
             if i == 2:
                 # Units
                 units = (line.split(sep=' ')[-1]).strip()
             elif i == 3:
                 # Number of points
                 npts = int(
-                    re.sub(
-                        r'NPTS=\s+', '', line.split(sep=', ')[0]
-                    )
+                    re.sub(r'NPTS=\s+', '', line.split(sep=', ')[0])
                 )  # noqa: W605
                 # Time step
-                tmp = re.sub(
-                    r'DT=\s+', '', line.split(sep=', ')[1]
-                )
+                tmp = re.sub(r'DT=\s+', '', line.split(sep=', ')[1])
                 tmp = re.sub(r'\s* SEC', '', tmp)
                 tmp = tmp.replace('SEC', '')  # some files have no space
                 d_t = float(tmp)
             elif i > 3:
                 break
 
     # Assert correct number of points and units
```

### Comparing `osmg-0.2.4/src/osmg/level.py` & `osmg-0.2.5/src/osmg/level.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/line.py` & `osmg-0.2.5/src/osmg/line.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/load_case.py` & `osmg-0.2.5/src/osmg/load_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,16 @@
     """
     Line element uniformly distributed load object.
 
     """
 
     parent_load_case: LoadCase
     parent_line_element: Union[
-        element.ElasticBeamColumn, element.DispBeamColumn]
+        element.ElasticBeamColumn, element.DispBeamColumn
+    ]
     val: nparr = field(default_factory=lambda: np.zeros(shape=3))
 
     def __repr__(self):
         res = ""
         res += "LineElementUDL object\n"
         res += f"parent_line_element.uid: {self.parent_line_element.uid}\n"
         res += "Components:\n"
@@ -117,15 +118,16 @@
         # can't apply a UDL on it. We need to lump the provided UDL to
         # its external nodes.  Since the Corotational transformation
         # also does not support rigid end offests, that lumping
         # process is always valid without requiring any special
         # transformation.
         elm = self.parent_line_element
         assert isinstance(
-            elm, (element.ElasticBeamColumn, element.DispBeamColumn))
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        )
         if elm.geomtransf.transf_type == "Corotational":
             elm_len = elm.clear_length()
             force = udl * elm_len / 2.00
             node_i_uid = elm.nodes[0].uid
             node_j_uid = elm.nodes[1].uid
             lcase = self.parent_load_case
             lcase.node_loads[node_i_uid].add(
@@ -208,29 +210,28 @@
         self.tributary_area_analysis = obj_collections.Collection(self)
         # initialize loads and mass for each node and element
         for node in self.parent_model.list_of_all_nodes():
             self.node_loads[node.uid] = PointLoadMass()
             self.node_mass[node.uid] = PointLoadMass()
         for elm in self.parent_model.list_of_elements():
             # only proceed for certain elements
-            if not isinstance(elm, (
-                    element.ElasticBeamColumn, element.DispBeamColumn)):
+            if not isinstance(
+                elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+            ):
                 continue
-            self.line_element_udl[elm.uid] = LineElementUDL(
-                self, elm
-            )
+            self.line_element_udl[elm.uid] = LineElementUDL(self, elm)
         # initialize tributary area analysis for each level
         for lvlkey, lvl in self.parent_model.levels.items():
             self.tributary_area_analysis[lvlkey] = TributaryAreaAnaysis(
                 self, lvl
             )
 
     def rigid_diaphragms(
-            self, level_uids: list[int],
-            gather_mass: bool = False) -> None:
+        self, level_uids: list[int], gather_mass: bool = False
+    ) -> None:
         """
         Processes the geometry of the given levels and applies rigid
         diaphragm constraints.
 
         """
 
         for lvl_uid in level_uids:
```

### Comparing `osmg-0.2.4/src/osmg/mesh.py` & `osmg-0.2.5/src/osmg/mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -249,15 +249,14 @@
         assert not np.isclose(vec_db @ vec_db, 0.00)
 
         mat_a: nparr = np.column_stack((vec_da, -vec_db))
         mat_b = vec_rb - vec_ra
         determinant = np.linalg.det(mat_a)
 
         if np.isclose(determinant, 0.00):
-
             # there are infinite solutions
             # or there are no solutions
             # i.e., the edges are parallel.
             # If they are parallel but nor colinear, then they don't
             # overlap and the method should return False
             # If they are colinear, then they might overlap. If they
             # do, the method should return True, otherwise False.
@@ -915,17 +914,16 @@
             ax_1.scatter(subregion.centroid.x, subregion.centroid.y)
         ax_1.margins(0.10)
         plt.show()
     return pieces
 
 
 def subdivide_hss_rect(
-        sec_h: float, sec_b: float,
-        sec_t: float, plot: bool = False) \
-        -> list[shapely_Polygon]:
+    sec_h: float, sec_b: float, sec_t: float, plot: bool = False
+) -> list[shapely_Polygon]:
     """
     Used to define the fibers of steel HSS fiber sections.
 
     Arguments:
       sec_h: Section height
       sec_b: Section width
       sec_t: Section thickness
@@ -997,17 +995,16 @@
         ax_1.margins(0.10)
         plt.show()
 
     return pieces
 
 
 def subdivide_hss_circ(
-        sec_d: float, sec_t: float,
-        plot: bool = False) \
-        -> list[shapely_Polygon]:
+    sec_d: float, sec_t: float, plot: bool = False
+) -> list[shapely_Polygon]:
     """
     Used to define the fibers of steel HSS fiber sections.
 
     Arguments:
       sec_d: Section diameter
       sec_t: Section thickness
 
@@ -1015,24 +1012,24 @@
         pieces: shapely_Polygon objects that represent single fibers.
 
     """
 
     num_subdiv_t = 3
     num_subdiv_circ = 12
 
-    radius = sec_d/2.00
+    radius = sec_d / 2.00
 
     pieces = []
 
     for i in range(num_subdiv_t):
         for j in range(num_subdiv_circ):
-            rr_i = radius - i * sec_t/num_subdiv_t
-            rr_j = radius - (i+1.0) * sec_t/num_subdiv_t
+            rr_i = radius - i * sec_t / num_subdiv_t
+            rr_j = radius - (i + 1.0) * sec_t / num_subdiv_t
             ang_i = (2.00 * np.pi) / num_subdiv_circ * j
-            ang_j = (2.00 * np.pi) / num_subdiv_circ * (j+1.00)
+            ang_j = (2.00 * np.pi) / num_subdiv_circ * (j + 1.00)
             pt1 = (rr_i * np.cos(ang_i), rr_i * np.sin(ang_i))
             pt2 = (rr_i * np.cos(ang_j), rr_i * np.sin(ang_j))
             pt3 = (rr_j * np.cos(ang_j), rr_j * np.sin(ang_j))
             pt4 = (rr_j * np.cos(ang_i), rr_j * np.sin(ang_i))
             pol = shapely_Polygon((pt1, pt2, pt3, pt4))
             pieces.append(pol)
```

### Comparing `osmg-0.2.4/src/osmg/model.py` & `osmg-0.2.5/src/osmg/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,15 @@
     from .ops.section import FiberSection
     from .ops.uniaxial_material import UniaxialMaterial
     from .physical_material import PhysicalMaterial
 
 nparr = npt.NDArray[np.float64]
 
 
-def transfer_component(
-        other: Model,
-        component: ComponentAssembly) -> None:
+def transfer_component(other: Model, component: ComponentAssembly) -> None:
     """
     Transfers a single component assembly from one model to
     another, assuming the other model was generated with the
     :func:`~Model.initialize_empty_copy` method.
 
     """
 
@@ -118,20 +116,23 @@
     """
 
     name: str
     levels: obj_collections.CollectionActive[int, Level] = field(init=False)
     elastic_sections: obj_collections.Collection[int, ElasticSection] = field(
         init=False
     )
-    fiber_sections: obj_collections.Collection[
-        int, FiberSection] = field(init=False)
+    fiber_sections: obj_collections.Collection[int, FiberSection] = field(
+        init=False
+    )
     uniaxial_materials: obj_collections.Collection[
-        int, UniaxialMaterial] = field(init=False)
+        int, UniaxialMaterial
+    ] = field(init=False)
     physical_materials: obj_collections.Collection[
-        int, PhysicalMaterial] = field(init=False)
+        int, PhysicalMaterial
+    ] = field(init=False)
     uid_generator: UIDGenerator = field(default_factory=UIDGenerator)
     settings: Settings = field(default_factory=Settings)
 
     def __post_init__(self):
         self.levels = obj_collections.CollectionActive(self)
         self.elastic_sections = obj_collections.Collection(self)
         self.fiber_sections = obj_collections.Collection(self)
@@ -305,16 +306,16 @@
         Returns a list of all element objects in the model.
 
         """
 
         return list(self.dict_of_elements().values())
 
     def dict_of_specific_element(
-            self, element_class: Type[element.Element]) \
-            -> dict[int, element.Element]:
+        self, element_class: Type[element.Element]
+    ) -> dict[int, element.Element]:
         """
         Returns a dictionary of all element objects in the model of a
         particular element class.
         The keys are the uids of the objects.
 
         """
 
@@ -322,16 +323,16 @@
         res: dict[int, element.Element] = {}
         for uid, elm in all_elements.items():
             if isinstance(elm, element_class):
                 res[uid] = elm
         return res
 
     def list_of_specific_element(
-            self, element_class: Type[element.Element]) \
-            -> list[element.Element]:
+        self, element_class: Type[element.Element]
+    ) -> list[element.Element]:
         """
         Returns a list of all element objects in the model of a
         particular element class.
 
         """
 
         return list(self.dict_of_specific_element(element_class).values())
@@ -384,15 +385,16 @@
         res.elastic_sections = self.elastic_sections
         res.fiber_sections = self.fiber_sections
         res.physical_materials = self.physical_materials
         res.uniaxial_materials = self.uniaxial_materials
         return res
 
     def transfer_by_polygon_selection(
-            self, other: Model, coords: nparr) -> None:
+        self, other: Model, coords: nparr
+    ) -> None:
         """
         Uses :func:`~transfer_component` to transfer all components of which
         the projection to the XY plane falls inside the specified
         polygon.
 
         """
```

### Comparing `osmg-0.2.4/src/osmg/obj_collections.py` & `osmg-0.2.5/src/osmg/obj_collections.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,16 @@
                     found = True
                     break
             if found:
                 break
         if res is None:
             raise ValueError(
                 f'Item having the value "{val}" '
-                f'in the attribute "{attr}" not found in collection.')
+                f'in the attribute "{attr}" not found in collection.'
+            )
         return res
 
     def __srepr__(self):
         """
         Concise version of `repr`.
 
         """
```

### Comparing `osmg-0.2.4/src/osmg/ops/element.py` & `osmg-0.2.5/src/osmg/ops/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import numpy.typing as npt
 from .uniaxial_material import UniaxialMaterial
 from .node import Node
 from .section import ElasticSection
 from .section import FiberSection
 from ..mesh import Mesh
 from ..graphics.visibility import ElementVisibility
+
 if TYPE_CHECKING:
     from ..component_assembly import ComponentAssembly
 
 
 nparr = npt.NDArray[np.float64]
 
 
@@ -169,50 +170,44 @@
     def ops_args(self):
         """
         Returns the arguments required to define the object in
         OpenSees
 
         """
 
-        elm_name = {
-            'Linear': 'Truss',
-            'Corotational': 'corotTruss'
-        }
+        elm_name = {'Linear': 'Truss', 'Corotational': 'corotTruss'}
 
         return [
             elm_name[self.transf_type],
             self.uid,
             self.nodes[0].uid,
             self.nodes[1].uid,
             self.area,
             self.mat.uid,
             '-rho',
             self.rho,
             '-cMass',
             self.cflag,
             '-doRayleigh',
-            self.rflag
+            self.rflag,
         ]
 
     def clear_length(self):
         """
         Returns the clear length of the element (without the rigid
         offsets)
 
         """
 
         p_i = np.array(self.nodes[0].coords)
         p_j = np.array(self.nodes[1].coords)
         return np.linalg.norm(p_i - p_j)
 
     def __repr__(self):
-        elm_name = {
-            'Linear': 'Truss',
-            'Corotational': 'corotTruss'
-        }
+        elm_name = {'Linear': 'Truss', 'Corotational': 'corotTruss'}
         res = ""
         res += f"{elm_name[self.transf_type]} element object\n"
         res += f"uid: {self.uid}\n"
         res += f"node_i.uid: {self.nodes[0].uid}\n"
         res += f"node_j.uid: {self.nodes[1].uid}\n"
         res += f"node_i.coords: {self.nodes[0].coords}\n"
         res += f"node_j.coords: {self.nodes[1].coords}\n"
@@ -293,15 +288,17 @@
                 self.nodes[1].uid,
                 self.section.area,
                 self.section.e_mod,
                 self.section.g_mod,
                 self.section.j_mod,
                 self.section.i_y,
                 self.section.i_x,
-                4.00, 4.00, 2.00,
+                4.00,
+                4.00,
+                2.00,
                 k11_x,
                 k33_x,
                 k44_x,
                 self.geomtransf.uid,
             ]
 
         if self.n_y is not None and self.n_x is None:
@@ -315,15 +312,17 @@
                 self.section.g_mod,
                 self.section.j_mod,
                 self.section.i_y,
                 self.section.i_x,
                 k11_y,
                 k33_y,
                 k44_y,
-                4.00, 4.00, 2.00,
+                4.00,
+                4.00,
+                2.00,
                 self.geomtransf.uid,
             ]
 
         if self.n_x is not None and self.n_y is not None:
             return [
                 "ModElasticBeam3d",
                 self.uid,
```

### Comparing `osmg-0.2.4/src/osmg/ops/node.py` & `osmg-0.2.5/src/osmg/ops/node.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/ops/section.py` & `osmg-0.2.5/src/osmg/ops/section.py`

 * *Files 1% similar despite different names*

```diff
@@ -195,16 +195,15 @@
                 self.holes,
                 self.parent_section.n_x,
                 self.parent_section.n_y,
             )
 
         return pieces
 
-    def copy_alter_material(
-            self, mat: UniaxialMaterial) -> SectionComponent:
+    def copy_alter_material(self, mat: UniaxialMaterial) -> SectionComponent:
         """
         Make a shallow copy of a section component and replace the old
         material with the given one.
 
         """
 
         new_component = SectionComponent(
@@ -284,16 +283,16 @@
                 area -= polygon_area(hole_coords)
             density = part.physical_material.density
             # TODO: units
             res += area * density * common.G_CONST_IMPERIAL
         return res * mult
 
     def copy_alter_material(
-            self, mat: UniaxialMaterial,
-            new_uid: int) -> FiberSection:
+        self, mat: UniaxialMaterial, new_uid: int
+    ) -> FiberSection:
         """
         Returns a shallow copy of the section object in which all
         opensees_material objects have been replaced with the given
         material. Required for the modling of steel braced frames.
 
         """
```

### Comparing `osmg-0.2.4/src/osmg/ops/uniaxial_material.py` & `osmg-0.2.5/src/osmg/ops/uniaxial_material.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 from typing import Optional
 from dataclasses import dataclass
 from dataclasses import field
 
 
 # pylint: disable=invalid-name
 
+
 @dataclass
 class UniaxialMaterial:
     """
     OpenSees uniaxialMaterial
     https://openseespydoc.readthedocs.io/en/latest/src/uniaxialMaterial.html
 
     """
@@ -191,34 +192,29 @@
             kinematic = False
 
         #
         # construct argument list
         #
 
         # these are required and will always be there
-        args = [
-            "Steel4",
-            self.uid,
-            self.Fy,
-            self.E0
-        ]
+        args = ["Steel4", self.uid, self.Fy, self.E0]
 
         # optional arguments:
         if asym:
             args.extend(['-asym'])
         if kinematic:
             args.extend(['-kin', self.b_k, self.R_0, self.r_1, self.r_2])
             if asym:
                 args.extend([self.b_kc, self.R_0c, self.r_1c, self.r_2c])
         if iso:
-            args.extend(['-iso', self.b_i, self.rho_i,
-                         self.b_l, self.R_i, self.l_yp])
+            args.extend(
+                ['-iso', self.b_i, self.rho_i, self.b_l, self.R_i, self.l_yp]
+            )
             if asym:
-                args.extend([self.b_ic, self.rho_ic,
-                             self.b_lc, self.R_ic])
+                args.extend([self.b_ic, self.rho_ic, self.b_lc, self.R_ic])
         if ultimate:
             args.extend(['-ult', self.f_u, self.R_u])
             if asym:
                 args.extend([self.f_uc, self.R_uc])
         if self.sig_init:
             args.extend(['-init', self.sig_init])
         if self.cycNum:
@@ -353,15 +349,15 @@
             self.Lamda_S,
             self.Lamda_C,
             self.Lamda_K,
             self.c_S,
             self.c_C,
             self.c_K,
             self.D_Plus,
-            self.D_Neg
+            self.D_Neg,
         ]
 
 
 @dataclass
 class Pinching4(UniaxialMaterial):
     """
     OpenSees Pinching4 Material
@@ -609,11 +605,11 @@
         args = [
             "MinMax",
             self.uid,
             self.predecessor.uid,
             '-min',
             self.min_strain,
             '-max',
-            self.max_strain
+            self.max_strain,
         ]
 
         return args
```

### Comparing `osmg-0.2.4/src/osmg/physical_material.py` & `osmg-0.2.5/src/osmg/physical_material.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/postprocessing/basic_forces.py` & `osmg-0.2.5/src/osmg/postprocessing/basic_forces.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,16 +58,17 @@
 
     if isinstance(anl, ModalResponseSpectrumAnalysis):
         forces = anl.combined_basic_forces(elm.uid)
         w_x, w_y, w_z = (0.00, 0.00, 0.00)
     else:
         forces = anl.results[case_name].element_forces[elm.uid][step]
         if isinstance(elm, (ElasticBeamColumn, DispBeamColumn)):
-            w_x, w_y, w_z = anl.load_cases[
-                case_name].line_element_udl[elm.uid].val
+            w_x, w_y, w_z = (
+                anl.load_cases[case_name].line_element_udl[elm.uid].val
+            )
         else:
             w_x, w_y, w_z = (0.00, 0.00, 0.00)
 
     if isinstance(elm, (ElasticBeamColumn, DispBeamColumn)):
         p_i = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
         p_j = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
     else:
```

### Comparing `osmg-0.2.4/src/osmg/postprocessing/design.py` & `osmg-0.2.5/src/osmg/postprocessing/design.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/postprocessing/steel_design_checks.py` & `osmg-0.2.5/src/osmg/postprocessing/steel_design_checks.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/preprocessing/rigid_diaphragm.py` & `osmg-0.2.5/src/osmg/preprocessing/rigid_diaphragm.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/preprocessing/self_weight_mass.py` & `osmg-0.2.5/src/osmg/preprocessing/self_weight_mass.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,17 +21,17 @@
 def self_weight(mdl, lcase, factor=1.00):
     """
     Assigns the structure's self weight to its members.
 
     """
 
     for elm in mdl.list_of_elements():
-
         if isinstance(
-                elm, (element.ElasticBeamColumn, element.DispBeamColumn)):
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        ):
             weight_per_length = elm.section.weight_per_length()
             # apply weight as UDL
             if elm.visibility.skip_opensees_definition:
                 # in that case apply its weight to the connecting nodes
                 elm_len = elm.clear_length()
                 elm_w = weight_per_length * elm_len * factor
                 lcase.node_loads[elm.nodes[0].uid].add(
@@ -65,17 +65,17 @@
 
     if mdl.settings.imperial_units:
         g_const = common.G_CONST_IMPERIAL
     else:
         g_const = common.G_CONST_SI
 
     for elm in mdl.list_of_elements():
-
         if isinstance(
-                elm, (element.ElasticBeamColumn, element.DispBeamColumn)):
+            elm, (element.ElasticBeamColumn, element.DispBeamColumn)
+        ):
             weight_per_length = elm.section.weight_per_length()
         elif isinstance(elm, element.TrussBar):
             weight_per_length = elm.weight_per_length
         else:
             # don't consider other types of elements
             continue
```

### Comparing `osmg-0.2.4/src/osmg/preprocessing/split_component.py` & `osmg-0.2.5/src/osmg/preprocessing/split_component.py`

 * *Files 12% similar despite different names*

```diff
@@ -27,34 +27,42 @@
 from ..ops.element import Lobatto
 
 
 nparr = npt.NDArray[np.float64]
 
 
 def split_component(
-        component: ComponentAssembly, point: nparr) \
-        -> tuple[Node, nparr]:
+    component: ComponentAssembly, point: nparr
+) -> tuple[Node, nparr]:
     """
     Splits a beam-functioning component assembly to accomodate for a
     node required to connect another component assembly.
 
     Arguments:
       component: Component assembly to split.
       point: Point to be used to split the component.
 
     WARNING:
       This function might no longer work. Needs to be tested and
       perhaps updated.
 
     """
 
+    uid_generator = (
+        component.parent_collection.parent.parent_model.uid_generator
+    )
+
     elms = []
     elms.extend(
-        [elm for elm in component.elements.values()
-         if isinstance(elm, (ElasticBeamColumn, DispBeamColumn))])
+        [
+            elm
+            for elm in component.elements.values()
+            if isinstance(elm, (ElasticBeamColumn, DispBeamColumn))
+        ]
+    )
     distances = np.zeros(len(elms))
     for i, elm in enumerate(elms):
         p_i = np.array(elm.nodes[0].coords) + elm.geomtransf.offset_i
         p_j = np.array(elm.nodes[1].coords) + elm.geomtransf.offset_j
         line = Line("", p_i, p_j)
         dist = line.point_distance(point)
         distances[i] = dist
@@ -89,67 +97,65 @@
     node_j = closest_elm.nodes[1]
     prev_section = closest_elm.section
     prev_gtransf = closest_elm.geomtransf
     component.elements.pop(closest_elm.uid)
 
     # add split node
     middle_node = Node(
-        component.parent_collection.parent.parent_model.uid_generator.new(
+        uid_generator.new(
             "node"
         ),
         list(split_point),
     )
     component.internal_nodes.add(middle_node)
     # add two new line elements
     # part i
     o_i = prev_gtransf.offset_i
     o_j = np.zeros(3)
     n_i = node_i
     n_j = middle_node
     transf_i = GeomTransf(
         prev_gtransf.transf_type,
-        component.parent_collection.parent.parent_model.uid_generator.new(
+        uid_generator.new(
             "transformation"
         ),
         o_i,
         o_j,
         prev_gtransf.x_axis,
         prev_gtransf.y_axis,
         prev_gtransf.z_axis,
     )
     if isinstance(closest_elm, ElasticBeamColumn):
         assert isinstance(prev_section, ElasticSection)
         elm_i = ElasticBeamColumn(
             component,
-            component.parent_collection.parent.parent_model.uid_generator.new(
+            uid_generator.new(
                 "element"
             ),
             [n_i, n_j],
             prev_section,
             transf_i,
         )
         component.elements.add(elm_i)
     elif isinstance(closest_elm, DispBeamColumn):
         assert isinstance(closest_elm.integration, Lobatto)
         beam_integration = Lobatto(
             uid=(
-                component.parent_collection
-                .parent.parent_model.uid_generator.new(
+                uid_generator.new(
                     "beam integration"
                 )
             ),
             parent_section=prev_section,
             n_p=closest_elm.integration.n_p,
         )
         assert isinstance(prev_section, FiberSection)
         elm_i = DispBeamColumn(  # type: ignore
             component,
             (
-                component.parent_collection.parent
-                .parent_model.uid_generator.new(
+                uid_generator.new(
                     "element"
                 )
             ),
             [n_i, n_j],
             prev_section,
             transf_i,
             beam_integration,
@@ -159,58 +165,54 @@
     o_i = np.zeros(3)
     o_j = prev_gtransf.offset_j
     n_i = middle_node
     n_j = node_j
     transf_j = GeomTransf(
         prev_gtransf.transf_type,
         (
-            component.parent_collection
-            .parent.parent_model.uid_generator.new(
+            uid_generator.new(
                 "transformation"
             )
         ),
         o_i,
         o_j,
         prev_gtransf.x_axis,
         prev_gtransf.y_axis,
         prev_gtransf.z_axis,
     )
     if isinstance(closest_elm, ElasticBeamColumn):
         assert isinstance(prev_section, ElasticSection)
         elm_j = ElasticBeamColumn(
             component,
             (
-                component.parent_collection
-                .parent.parent_model.uid_generator.new(
+                uid_generator.new(
                     "element"
                 )
             ),
             [n_i, n_j],
             prev_section,
             transf_j,
         )
         component.elements.add(elm_j)
     elif isinstance(closest_elm, DispBeamColumn):
         assert isinstance(closest_elm.integration, Lobatto)
         beam_integration = Lobatto(
             uid=(
-                component.parent_collection
-                .parent.parent_model.uid_generator.new(
+                uid_generator.new(
                     "beam integration"
                 )
             ),
             parent_section=prev_section,
             n_p=closest_elm.integration.n_p,
         )
         assert isinstance(prev_section, FiberSection)
         elm_j = DispBeamColumn(  # type: ignore
             component,
             (
-                component.parent_collection
-                .parent.parent_model.uid_generator.new(
+                uid_generator.new(
                     "element"
                 )
             ),
             [n_i, n_j],
             prev_section,
             transf_j,
             beam_integration,
```

### Comparing `osmg-0.2.4/src/osmg/preprocessing/tributary_area_analysis.py` & `osmg-0.2.5/src/osmg/preprocessing/tributary_area_analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,23 +196,27 @@
             }
             pz_node[front_nd.uid] = {
                 "substitute_node": main_nd,
                 "additional_offset": -front_offset[0:2],
             }
 
         for comp in horizontal_elements:
-
             line_elements = [
-                elm for elm in comp.elements.values()
+                elm
+                for elm in comp.elements.values()
                 if isinstance(
-                    elm, (ElasticBeamColumn, DispBeamColumn, TwoNodeLink))]
+                    elm, (ElasticBeamColumn, DispBeamColumn, TwoNodeLink)
+                )
+            ]
 
             zerolength_elements = [
-                elm for elm in comp.elements.values()
-                if isinstance(elm, ZeroLength)]
+                elm
+                for elm in comp.elements.values()
+                if isinstance(elm, ZeroLength)
+            ]
             for zelm in zerolength_elements:
                 zn_map[zelm.nodes[1].uid] = zelm.nodes[0].uid
 
             for elm in line_elements:
                 n_i = elm.nodes[0]
                 if hasattr(elm, 'geomtransf'):
                     eo_i = elm.geomtransf.offset_i[0:2]
@@ -513,17 +517,22 @@
                             np.array([half_mass] * 3 + [0.00] * 3)
                         )
 
                 elif isinstance(loaded_elm, TwoNodeLink):
                     for node in loaded_elm.nodes:
                         lcase.node_loads[node.uid].add(
                             np.array(
-                                [0.00, 0.00,
-                                 -load_val * cmult / 2.00,
-                                 0.00, 0.00, 0.00]
+                                [
+                                    0.00,
+                                    0.00,
+                                    -load_val * cmult / 2.00,
+                                    0.00,
+                                    0.00,
+                                    0.00,
+                                ]
                             )
                         )
                         if not load.massless:
                             lcase.node_mass[node.uid].add(
                                 np.array(
                                     [
                                         load_val / g_const / 2.00,
```

### Comparing `osmg-0.2.4/src/osmg/sections.json` & `osmg-0.2.5/src/osmg/sections.json`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg/solver.py` & `osmg-0.2.5/src/osmg/solver.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 import platform
 import socket
 import sys
 from time import perf_counter
 import os
 import pickle
 import logging
-import textwrap
 from tqdm import tqdm
 import numpy as np
 import numpy.typing as npt
 from scipy import integrate
 from scipy.interpolate import interp1d
 import pandas as pd
 import matplotlib.pyplot as plt
@@ -437,49 +436,25 @@
                 ops.uniaxialMaterial(*mat.ops_args())
                 defined_materials[mat.uid] = mat
 
         for elm in elms:
             sec = elm.section
             parts = sec.section_parts.values()
             if sec.uid not in defined_sections:
-                if ops.__name__ == 'openseespy.opensees':
-                    ops.section(*sec.ops_args())
-                    defined_sections[sec.uid] = sec
-                fibers = []
+                ops.section(*sec.ops_args())
+                defined_sections[sec.uid] = sec
                 for part in parts:
                     mat = part.ops_material
                     define_material(mat, defined_materials)
                     pieces = part.cut_into_tiny_little_pieces()
                     for piece in pieces:
                         area = piece.area
                         z_loc = piece.centroid.x
                         y_loc = piece.centroid.y
-                        if ops.__name__ == 'openseespy.opensees':
-                            ops.fiber(
-                                y_loc, z_loc, area, part.ops_material.uid
-                            )
-                        else:  # ops.__name__ == 'opensees.openseespy'
-                            fibers.append(
-                                [y_loc, z_loc, area, part.ops_material.uid]
-                            )
-
-                if ops.__name__ == 'opensees.openseespy':
-                    fiber_commands = ';\n     '.join(
-                        "fiber " + " ".join(map(str, fiber))
-                        for fiber in fibers
-                    )
-                    cmd = textwrap.dedent(
-                        f"""
-                    section {' '.join(map(str,sec.ops_args()))} {{
-                      {fiber_commands}
-                    }}
-                    """
-                    )
-                    ops.eval(cmd)
-                    defined_sections[sec.uid] = sec
+                        ops.fiber(y_loc, z_loc, area, part.ops_material.uid)
 
             ops.beamIntegration(*elm.integration.ops_args())
             ops.geomTransf(*elm.geomtransf.ops_args())
             ops.element(*elm.ops_args())
 
         # ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~ #
         # ZeroLength element definition #
@@ -950,15 +925,16 @@
                         .val
                     )
                     # note: modal analysis doesn't account for applied loads.
                     # this will cause issues with plotting if loads
                     # have been applied.
                     if np.linalg.norm(udl) > common.EPSILON:
                         self.warning.issue(
-                            "Loads were present in a modal load case. Ignoring them."
+                            "Loads were present in a modal load case. Ignoring"
+                            " them."
                         )
                         udl = np.zeros(3)
 
                 # global -> local transformation matrix
                 transf_global2local = transformations.transformation_matrix(
                     x_vec, y_vec, z_vec
                 )
@@ -1823,14 +1799,15 @@
         damping: dict[str, Optional[Union[str, float, int, list[float]]]] = {
             "type": None
         },
         print_progress: bool = True,
         drift_check: float = 0.00,
         time_limit: Optional[float] = None,
         dampen_out_residual: bool = False,
+        test_tolerance: float = 1e-12,
     ) -> dict[str, Union[int, str, float]]:
         """
         Run the time-history analysis
 
         Arguments:
             ag_vec_x, y, z: 1-D numpy arrays containing the fixed-step
                             ground acceleration records.
@@ -1999,21 +1976,21 @@
             # self.print(len(tags))
 
             self.log("Using modal damping")
 
             num_modes = damping["num_modes"]
             # num_modes = num_modeshapes
             damping_ratio = damping["ratio"]
-            self.log("Running eigenvalue analysis" f" with {num_modes} modes")
+            self.log(f"Running eigenvalue analysis with {num_modes} modes")
             ops.eigen(num_modes)
             # ops.systemSize()
             self.log("Eigenvalue analysis finished")
             assert isinstance(damping_ratio, float)
             ops.modalDampingQ(damping_ratio)
-            self.log(f"{damping_ratio*100.00:.2f}% " "modal damping defined")
+            self.log(f"{damping_ratio*100.00:.2f}% modal damping defined")
 
         if damping_type == "modal+stiffness":
             self.log("Using modal+stiffness damping")
 
             # stiffness-proportional contribution
             assert isinstance(damping["ratio_stiffness"], float)
             assert isinstance(damping["period"], float)
@@ -2028,24 +2005,24 @@
             self.log("modal+stiffness damping defined")
 
             # modal damping
             num_modes = damping["num_modes"]
             assert isinstance(num_modes, int)
             damping_ratio = damping["ratio_modal"]
             assert isinstance(damping_ratio, float)
-            self.log("Running eigenvalue analysis" f" with {num_modes} modes")
+            self.log(f"Running eigenvalue analysis with {num_modes} modes")
             omega_squareds = np.array(ops.eigen(num_modes))
             self.log("Eigenvalue analysis finished")
             damping_vals = (
                 damping["ratio_modal"] - alpha_1 * omega_squareds / 2.00
             )
             damping_vals[damping_vals < 0.00] = 0.00
             ops.modalDampingQ(*damping_vals)
 
-        ops.test("EnergyIncr", 1.0e-6, 100, 0)
+        ops.test("EnergyIncr", test_tolerance, 100, 0)
         ops.integrator('TRBDF2')
         ops.algorithm("KrylovNewton")
         # ops.algorithm("KrylovNewton", 'initial', 'initial')
         ops.analysis("Transient")
 
         define_lateral_load_pattern(
             ag_vec_x, ag_vec_y, ag_vec_z, ag_vec_time_incr
@@ -2068,15 +2045,14 @@
             1.0e-7,
             1.0e-8,
             1.0e-9,
             1.0e-10,
             1.0e-11,
             1e-12,
         )
-        tols = [1.0e-8] * len(scale)
         algorithms = (
             ("KrylovNewton",),
             ("KrylovNewton", "initial", "initial"),
             ("NewtonLineSearch",),
         )
 
         # progress bar
@@ -2104,15 +2080,15 @@
         self.log(f'Max time step: {analysis_time_increment}')
 
         try:
             while curr_time + common.EPSILON < target_timestamp:
                 if analysis_failed:
                     break
 
-                ops.test("EnergyIncr", tols[num_subdiv], 200, 3, 2)
+                ops.test("EnergyIncr", test_tolerance, 200, 3, 2)
                 ops.algorithm(*algorithms[algorithm_idx])
                 check = ops.analyze(
                     1, analysis_time_increment * scale[num_subdiv]
                 )
                 total_step_count += 1
 
                 if check != 0:
@@ -2144,15 +2120,17 @@
                     curr_time = float(ops.getTime())
                     testiter = ops.testIter()
 
                     # progress bar
                     if pbar is not None:
                         pbar.set_postfix(
                             {
-                                'time': f'{curr_time:.4f}/{target_timestamp:.2f} [{testiter}]'
+                                'time': (
+                                    f'{curr_time:.4f}/{target_timestamp:.2f} [{testiter}]'
+                                )
                             }
                         )
                         pbar.update(curr_time - prev_time)
                     # log entry for analysis status
                     if perf_counter() - the_time > 5.00 * 60.00:  # 5 min
                         the_time = perf_counter()
                         # total time running
@@ -2292,15 +2270,15 @@
             ops.rayleigh(0.00, 0.0, 0.0, 0.60 / np.pi)
             last_time = curr_time
             curr_time = 0.00
             ops.setTime(curr_time)
             target_timestamp = 10.00
 
             while curr_time + common.EPSILON < target_timestamp:
-                ops.test("EnergyIncr", tols[0], 200, 3, 2)
+                ops.test("EnergyIncr", test_tolerance, 200, 3, 2)
                 ops.algorithm(*algorithms[0])
                 check = ops.analyze(1, analysis_time_increment)
 
                 if check != 0:
                     self.log(
                         "Failed to dampen out residual motion, skipping..."
                     )
```

### Comparing `osmg-0.2.4/src/osmg/transformations.py` & `osmg-0.2.5/src/osmg/transformations.py`

 * *Files identical despite different names*

### Comparing `osmg-0.2.4/src/osmg.egg-info/PKG-INFO` & `osmg-0.2.5/src/osmg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmg
-Version: 0.2.4
+Version: 0.2.5
 Summary: OpenSees Model Generator
 Home-page: https://github.com/ioannis-vm/OpenSees_Model_Generator
 Author: John Vouvakis Manousakis
 License: GPL
 Platform: unix
 Platform: linux
 Platform: osx
```

### Comparing `osmg-0.2.4/src/osmg.egg-info/SOURCES.txt` & `osmg-0.2.5/src/osmg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

