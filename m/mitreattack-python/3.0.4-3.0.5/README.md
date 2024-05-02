# Comparing `tmp/mitreattack-python-3.0.4.tar.gz` & `tmp/mitreattack-python-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mitreattack-python-3.0.4.tar", last modified: Tue Apr 23 14:32:24 2024, max compression
+gzip compressed data, was "mitreattack-python-3.0.5.tar", last modified: Thu May  2 15:02:49 2024, max compression
```

## Comparing `mitreattack-python-3.0.4.tar` & `mitreattack-python-3.0.5.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/NOTICE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/attackToExcel/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/attackToExcel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/attackToExcel/attackToExcel.py
--rw-r--r--   0 runner    (1001) docker     (127)    47062 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/attackToExcel/stixToDf.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/collections/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/collection_to_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/index_to_markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/collections/stix_to_collection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.044119 mitreattack-python-3.0.4/mitreattack/diffStix/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/diffStix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    89466 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/diffStix/changelog_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/download_stix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.048119 mitreattack-python-3.0.4/mitreattack/navlayers/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.048119 mitreattack-python-3.0.4/mitreattack/navlayers/core/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/gradient.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/layer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/layerobj.py
--rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/legenditem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/objlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/technique.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/core/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.048119 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/excel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   358460 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/monospace.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   317968 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    85240 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/serif.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/matrix_gen.py
--rw-r--r--   0 runner    (1001) docker     (127)    18606 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_excel.py
--rw-r--r--   0 runner    (1001) docker     (127)    18858 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_svg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/navlayers/generators/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/gen_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/overview_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/generators/usage_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/layerExporter_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/layerGenerator_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13317 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/layerops.py
--rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/release_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack/stix20/
--rw-r--r--   0 runner    (1001) docker     (127)    67572 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/stix20/MitreAttackData.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/stix20/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/mitreattack/stix20/custom_attack_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.052120 mitreattack-python-3.0.4/mitreattack_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-04-23 14:32:24.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-23 14:32:23.000000 mitreattack-python-3.0.4/mitreattack_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:32:24.056120 mitreattack-python-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_mass.py
--rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_mitreattackdata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_stix20.py
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-04-23 14:23:51.000000 mitreattack-python-3.0.4/tests/test_to_excel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.072570 mitreattack-python-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/NOTICE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-02 15:02:49.072570 mitreattack-python-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5868 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.060570 mitreattack-python-3.0.5/mitreattack/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.060570 mitreattack-python-3.0.5/mitreattack/attackToExcel/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/attackToExcel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15827 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/attackToExcel/attackToExcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47062 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/attackToExcel/stixToDf.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.060570 mitreattack-python-3.0.5/mitreattack/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9165 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/collections/collection_to_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/collections/index_to_markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6247 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/collections/stix_to_collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.060570 mitreattack-python-3.0.5/mitreattack/diffStix/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/diffStix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89466 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/diffStix/changelog_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/download_stix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.064570 mitreattack-python-3.0.5/mitreattack/navlayers/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.064570 mitreattack-python-3.0.5/mitreattack/navlayers/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3714 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/layer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19763 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/layerobj.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6800 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/legenditem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/objlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8964 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/technique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2775 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/core/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.064570 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6610 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/excel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.068570 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   358460 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/monospace.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   317968 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/sans-serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    85240 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/serif.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    18380 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/matrix_gen.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18606 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/svg_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19777 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/svg_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8042 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/to_excel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18858 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/exporters/to_svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.068570 mitreattack-python-3.0.5/mitreattack/navlayers/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/generators/gen_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12860 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/generators/overview_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/generators/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7125 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/generators/usage_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/layerExporter_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/layerGenerator_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.068570 mitreattack-python-3.0.5/mitreattack/navlayers/manipulators/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/manipulators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13463 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/navlayers/manipulators/layerops.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16899 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/release_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.068570 mitreattack-python-3.0.5/mitreattack/stix20/
+-rw-r--r--   0 runner    (1001) docker     (127)    68256 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/stix20/MitreAttackData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/stix20/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8753 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/mitreattack/stix20/custom_attack_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.068570 mitreattack-python-3.0.5/mitreattack_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-02 15:02:49.000000 mitreattack-python-3.0.5/mitreattack_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2546 2024-05-02 15:02:49.000000 mitreattack-python-3.0.5/mitreattack_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 15:02:49.000000 mitreattack-python-3.0.5/mitreattack_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-05-02 15:02:49.000000 mitreattack-python-3.0.5/mitreattack_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 15:02:49.000000 mitreattack-python-3.0.5/mitreattack_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 15:02:49.000000 mitreattack-python-3.0.5/mitreattack_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 15:02:49.072570 mitreattack-python-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 15:02:49.072570 mitreattack-python-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-05-02 14:54:07.000000 mitreattack-python-3.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8158 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10892 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6621 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4733 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9058 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_mitreattackdata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_stix20.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-02 14:54:08.000000 mitreattack-python-3.0.5/tests/test_to_excel.py
```

### Comparing `mitreattack-python-3.0.4/LICENSE.txt` & `mitreattack-python-3.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/NOTICE.txt` & `mitreattack-python-3.0.5/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/PKG-INFO` & `mitreattack-python-3.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 3.0.4
+Version: 3.0.5
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-3.0.4/README.md` & `mitreattack-python-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/attackToExcel/attackToExcel.py` & `mitreattack-python-3.0.5/mitreattack/attackToExcel/attackToExcel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/attackToExcel/stixToDf.py` & `mitreattack-python-3.0.5/mitreattack/attackToExcel/stixToDf.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/collections/collection_to_index.py` & `mitreattack-python-3.0.5/mitreattack/collections/collection_to_index.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/collections/index_to_markdown.py` & `mitreattack-python-3.0.5/mitreattack/collections/index_to_markdown.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/collections/stix_to_collection.py` & `mitreattack-python-3.0.5/mitreattack/collections/stix_to_collection.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/constants.py` & `mitreattack-python-3.0.5/mitreattack/constants.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/diffStix/changelog_helper.py` & `mitreattack-python-3.0.5/mitreattack/diffStix/changelog_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -1048,16 +1048,16 @@
             legendItems = []
             for section, description in self.section_descriptions.items():
                 legendItems.append({"color": colors[section], "label": f"{section}: {description}"})
 
             # build layer structure
             layer_json = {
                 "versions": {
-                    "layer": "4.4",
-                    "navigator": "4.8.0",
+                    "layer": "4.5",
+                    "navigator": "5.0.0",
                     "attack": self.data["new"][domain]["attack_release_version"],
                 },
                 "name": f"{thedate} {self.domain_to_domain_label[domain]} Updates",
                 "description": f"{self.domain_to_domain_label[domain]} updates for the {thedate} release of ATT&CK",
                 "domain": domain,
                 "techniques": techniques,
                 "sorting": 0,
```

### Comparing `mitreattack-python-3.0.4/mitreattack/download_stix.py` & `mitreattack-python-3.0.5/mitreattack/download_stix.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/exceptions.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/filter.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/filter.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/gradient.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/gradient.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/helpers.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/layer.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/layer.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/layerobj.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/layerobj.py`

 * *Files 0% similar despite different names*

```diff
@@ -458,15 +458,15 @@
         """
         if field == "description":
             self.description = data
         elif field.startswith("version"):
             if not field.endswith("s"):
                 # force upgrade
                 print("[Version] - V3 version field detected. Upgrading to V4 Versions object.")
-                ver_obj = dict(layer="4.0", navigator="4.0")
+                ver_obj = dict(layer="4.5", navigator="5.0.0")
                 self.versions = ver_obj
             else:
                 self.versions = data
         elif field == "filters":
             self.filters = data
         elif field == "sorting":
             self.sorting = data
```

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/layout.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/layout.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/legenditem.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/legenditem.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/metadata.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/metadata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/objlink.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/objlink.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/technique.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/technique.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/core/versions.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/core/versions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Contains Versions class."""
 
 from mitreattack.navlayers.core.exceptions import typeChecker, categoryChecker, UNSETVALUE, BadInput
 
-defaults = dict(layer="4.5", navigator="4.9.0")
+defaults = dict(layer="4.5", navigator="5.0.0")
 
 
 class Versions:
     """A Versions object."""
 
     def __init__(self, layer=defaults["layer"], attack=UNSETVALUE, navigator=defaults["navigator"]):
         """Initialize - Creates a v4 Versions object.
@@ -38,17 +38,17 @@
         """Getter for navigator."""
         return self.__navigator
 
     @navigator.setter
     def navigator(self, navigator):
         """Setter for navigator."""
         typeChecker(type(self).__name__, navigator, str, "navigator")
-        if not navigator.startswith("4."):
+        if not navigator.startswith("5."):
             print(
-                f"[WARNING] - unrecognized navigator version {navigator}. Defaulting to the 4.X schema, "
+                f"[WARNING] - unrecognized navigator version {navigator}. Defaulting to the 5.X.X schema, "
                 f"this may result in unexpected behavior."
             )
             navigator = defaults["navigator"]
         self.__navigator = navigator
 
     @property
     def layer(self):
```

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/excel_templates.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/excel_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/monospace.ttf` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/monospace.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/sans-serif.ttf` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/sans-serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/fonts/serif.ttf` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/fonts/serif.ttf`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/matrix_gen.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/matrix_gen.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_objects.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/svg_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/svg_templates.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/svg_templates.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_excel.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/to_excel.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/exporters/to_svg.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/exporters/to_svg.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/generators/gen_helpers.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/generators/gen_helpers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/generators/overview_generator.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/generators/overview_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/generators/sum_generator.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/generators/sum_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/generators/usage_generator.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/generators/usage_generator.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/layerExporter_cli.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/layerExporter_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/layerGenerator_cli.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/layerGenerator_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/navlayers/manipulators/layerops.py` & `mitreattack-python-3.0.5/mitreattack/navlayers/manipulators/layerops.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,17 +177,19 @@
             for x in data:
                 collide.append(x)
         key_space = data[key].layer._enumerate()
         _raw = data[key].layer.get_dict()
         for entry in key_space:
             if entry != "techniques":
                 standard = _raw[entry]
-                if any(y != standard for y in [getattr(x.layer, entry) for x in collide]):
+                layer_entries = [getattr(x.layer, entry) for x in collide]
+                layer_entries = [y.get_dict() if hasattr(y, 'get_dict') else y for y in layer_entries]
+                if any(y != standard for y in layer_entries):
                     if entry == "domain":
-                        print("FATAL ERROR! Layer mis-match on domain. " "Exiting.")
+                        print("FATAL ERROR! Layer mis-match on domain. Exiting.")
                         raise MismatchedDomain
                     print(f"Warning! Layer mis-match detected for {entry}. Defaulting to {key}'s value")
                 out[entry] = standard
         return out
 
     def _build_template(self, data):
         """Build a base template by combining available technique listings from each layer.
```

### Comparing `mitreattack-python-3.0.4/mitreattack/release_info.py` & `mitreattack-python-3.0.5/mitreattack/release_info.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack/stix20/MitreAttackData.py` & `mitreattack-python-3.0.5/mitreattack/stix20/MitreAttackData.py`

 * *Files 1% similar despite different names*

```diff
@@ -486,14 +486,36 @@
         all_tactics = self.get_tactics()
         technique_tactics = []
         for tactic in all_tactics:
             if tactic.get_shortname() in shortnames:
                 technique_tactics.append(tactic)
 
         return technique_tactics
+    
+    def get_procedure_examples_by_technique(self, stix_id) -> list:
+        """Retrieve the list of procedure examples by technique.
+
+        Parameters
+        ----------
+        stix_id : str
+            the stix id of the technique.
+
+        Returns
+        -------
+        list
+            a list of stix2.v20.Relationship objects describing the software, groups, and campaigns using the technique.
+        """
+        procedures = self.src.query(
+            [
+                Filter("type", "=", "relationship"),
+                Filter("relationship_type", "=", "uses"),
+                Filter("target_ref", "=", stix_id),
+            ]
+        )
+        return procedures
 
     def get_objects_created_after(self, timestamp: str, remove_revoked_deprecated=False) -> list:
         """Retrieve objects which have been created after a given time.
 
         Parameters
         ----------
         timestamp : str
```

### Comparing `mitreattack-python-3.0.4/mitreattack/stix20/custom_attack_objects.py` & `mitreattack-python-3.0.5/mitreattack/stix20/custom_attack_objects.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack_python.egg-info/PKG-INFO` & `mitreattack-python-3.0.5/mitreattack_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mitreattack-python
-Version: 3.0.4
+Version: 3.0.5
 Summary: MITRE ATT&CK python library
 Home-page: https://github.com/mitre-attack/mitreattack-python/
 Author: MITRE ATT&CK, MITRE Corporation
 Author-email: attack@mitre.org
 Maintainer: Jared Ondricek
 Maintainer-email: jondricek@mitre.org
 License: Apache 2.0
```

### Comparing `mitreattack-python-3.0.4/mitreattack_python.egg-info/SOURCES.txt` & `mitreattack-python-3.0.5/mitreattack_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/mitreattack_python.egg-info/entry_points.txt` & `mitreattack-python-3.0.5/mitreattack_python.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/setup.py` & `mitreattack-python-3.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mitreattack-python",
-    version="3.0.4",
+    version="3.0.5",
     author="MITRE ATT&CK, MITRE Corporation",
     author_email="attack@mitre.org",
     description="MITRE ATT&CK python library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     maintainer="Jared Ondricek",
     maintainer_email="jondricek@mitre.org",
```

### Comparing `mitreattack-python-3.0.4/tests/conftest.py` & `mitreattack-python-3.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_cli.py` & `mitreattack-python-3.0.5/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_collections.py` & `mitreattack-python-3.0.5/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_layers.py` & `mitreattack-python-3.0.5/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_mass.py` & `mitreattack-python-3.0.5/tests/test_mass.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_mitreattackdata.py` & `mitreattack-python-3.0.5/tests/test_mitreattackdata.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_stix20.py` & `mitreattack-python-3.0.5/tests/test_stix20.py`

 * *Files identical despite different names*

### Comparing `mitreattack-python-3.0.4/tests/test_to_excel.py` & `mitreattack-python-3.0.5/tests/test_to_excel.py`

 * *Files identical despite different names*

