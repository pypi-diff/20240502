# Comparing `tmp/lsst-daf-butler-26.2024.900.tar.gz` & `tmp/lsst_daf_butler-27.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lsst-daf-butler-26.2024.900.tar", last modified: Thu Feb 29 10:30:36 2024, max compression
+gzip compressed data, was "lsst_daf_butler-27.0.0rc1.tar", last modified: Wed May  1 21:29:36 2024, max compression
```

## Comparing `lsst-daf-butler-26.2024.900.tar` & `lsst_daf_butler-27.0.0rc1.tar`

### file list

```diff
@@ -1,405 +1,444 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/bsd_license.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.942124 lsst-daf-butler-26.2024.900/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.950123 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/
--rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/concreteStorageClasses.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/configuring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/datastores.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/dimensions.rst
--rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/formatters.rst
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/organizing.rst
--rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/queries.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/use-in-tests.rst
--rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/writing-subcommands.rst
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/gpl-v3.0.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6487 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.946123 lsst-daf-butler-26.2024.900/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.950123 lsst-daf-butler-26.2024.900/python/lsst/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.950123 lsst-daf-butler-26.2024.900/python/lsst/daf/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.958124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    73722 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_instance_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_repo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_categorization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_type_info.py
--rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_association.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_existence.py
--rw-r--r--   0 runner    (1001) docker     (127)    32097 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_ref.py
--rw-r--r--   0 runner    (1001) docker     (127)    30001 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_deferredDatasetHandle.py
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_labeled_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_limited_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_location.py
--rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_named.py
--rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum_backed.py
--rw-r--r--   0 runner    (1001) docker     (127)    11783 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    27865 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_registry_shim.py
--rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class.py
--rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class_delegate.py
--rw-r--r--   0 runner    (1001) docker     (127)    23419 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     5904 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_topology.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.958124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/locked_object.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/named_locks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/thread_safe_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    16416 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/arrow_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.958124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cliLog.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_runs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/commands.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/optionGroups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)    44064 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     8692 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/column_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastore.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.962123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/composites.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5423 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/formatters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/dimensions.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/registry.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    14810 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/storageClasses.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    57431 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/cache_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/composites.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    31187 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/file_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/generic_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/record_data.py
--rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/stored_file_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/chainedDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastoreClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/get.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/inMemoryDatastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/ddl.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.966123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowastropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpydict.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowtable.py
--rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/dataframe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.970124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    55439 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_coordinate.py
--rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
--rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_elements.py
--rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_governor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22849 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    20363 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_packer.py
--rw-r--r--   0 runner    (1001) docker     (127)    18140 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_table.py
--rw-r--r--   0 runner    (1001) docker     (127)    19854 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_skypix.py
--rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_universe.py
--rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/construction.py
--rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/record_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    97583 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4318 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    11513 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_query_results.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.970124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/astropyTable.py
--rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/matplotlib.py
--rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    42219 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/pickle.py
--rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     5271 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/json.py
--rw-r--r--   0 runner    (1001) docker     (127)    18310 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    10673 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/mapping_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/persistence_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/progress.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    10226 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/pydantic_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.974124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/
--rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_caching_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     5865 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_record_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     9657 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_dataset_type_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     5538 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    60805 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/attributes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/ephemeral.py
--rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/monolithic.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17921 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    11212 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/nameKey.py
--rw-r--r--   0 runner    (1001) docker     (127)    11866 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/synthIntKey.py
--rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/connectionString.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22479 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24029 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    40134 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
--rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.978124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/
--rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    42986 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/static.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.982123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    21076 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    79781 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    13309 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_opaque.py
--rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_versioning.py
--rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/managers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3700 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/nameShrinker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.982123 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_records.py
--rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/default_spatial.py
--rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/pgsphere.py
--rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/opaque.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_builder.py
--rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query.py
--rw-r--r--   0 runner    (1001) docker     (127)    33946 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_readers.py
--rw-r--r--   0 runner    (1001) docker     (127)    39207 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_results.py
--rw-r--r--   0 runner    (1001) docker     (127)    16320 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    25438 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10141 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)    13757 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/categorize.py
--rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/check.py
--rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
--rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.986124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
--rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/find_first_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)   114994 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/sql_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    64443 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_database.py
--rw-r--r--   0 runner    (1001) docker     (127)   174129 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/versions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/wildcards.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3909 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_collection_args.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4715 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    11891 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)    30211 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_remote_butler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.990124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/repo_relocation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.994124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_associate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_pruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/butlerImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/certifyCalibrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5364 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/collectionChain.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/createRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/exportCalibs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/ingest_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/register_dataset_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeDatasetType.py
--rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/retrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/transferDatasets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.998124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_datasetsHelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_dummyRegistry.py
--rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_examplePythonTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)    67398 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/butler_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliCmdTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliLogTestBase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/deferredFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/dict_convertible_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    14137 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler_registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/testFormatters.py
--rw-r--r--   0 runner    (1001) docker     (127)    13168 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    24816 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/timespan_database_representation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:35.998124 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16954 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)    23380 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst/daf/butler/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16019 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 10:30:35.000000 lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 10:30:36.014124 lsst-daf-butler-26.2024.900/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_astropyTableFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)   116669 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_butler_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     5255 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_butler_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdAssociate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigDump.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigValidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdCreate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdImport.py
--rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdIngestFiles.py
--rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdPruneDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    12885 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDataIds.py
--rw-r--r--   0 runner    (1001) docker     (127)    10198 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasetTypes.py
--rw-r--r--   0 runner    (1001) docker     (127)    20536 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     9376 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDimensionRecords.py
--rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveCollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveRuns.py
--rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliCmdRetrieveArtifacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliLog.py
--rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliPluginLoader.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitCommas.py
--rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitKv.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtilToUpper.py
--rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_cliUtils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_composites.py
--rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_connectionString.py
--rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    82916 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_ddl.py
--rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_dimension_record_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    45092 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_dimensions.py
--rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_exprParserLex.py
--rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_exprParserYacc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_logFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_matplotlibFormatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_nonempty_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_normalFormExpression.py
--rw-r--r--   0 runner    (1001) docker     (127)    26817 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_obscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    80609 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4205 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_pydantic_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_quantum.py
--rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_quantumBackedButler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_query_relations.py
--rw-r--r--   0 runner    (1001) docker     (127)     5375 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_remote_butler.py
--rw-r--r--   0 runner    (1001) docker     (127)    17539 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)    33656 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_simpleButler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_storageClass.py
--rw-r--r--   0 runner    (1001) docker     (127)    17542 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_testRepo.py
--rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_time_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    11676 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_timespan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-02-29 10:30:26.000000 lsst-daf-butler-26.2024.900/tests/test_versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.793144 lsst_daf_butler-27.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 21:29:36.793144 lsst_daf_butler-27.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/bsd_license.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.717144 lsst_daf_butler-27.0.0rc1/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.725144 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/
+-rw-r--r--   0 runner    (1001) docker     (127)    54247 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/concreteStorageClasses.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5626 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/configuring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8442 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/datastores.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10776 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/dimensions.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    22653 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/formatters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     6841 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10031 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/organizing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/queries.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3753 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/use-in-tests.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    16372 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/writing-subcommands.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/gpl-v3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6590 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.721144 lsst_daf_butler-27.0.0rc1/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.725144 lsst_daf_butler-27.0.0rc1/python/lsst/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.725144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.733144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75038 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9619 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_instance_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8466 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_repo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_column_categorization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6058 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_column_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7162 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_column_type_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52100 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14135 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_config_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2360 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_association.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_existence.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_ref.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30028 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_deferredDatasetHandle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6622 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_exceptions_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3399 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_file_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3505 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_file_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30151 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7435 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_labeled_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15147 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_limited_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10451 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19541 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_named.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25574 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32289 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_quantum_backed.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14915 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_registry_shim.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37492 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_storage_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14504 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_storage_class_delegate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23377 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5961 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_topology.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.733144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/locked_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/named_locks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/thread_safe_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16594 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/arrow_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.733144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14768 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16861 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cliLog.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.737144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3925 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/_remove_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5664 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/_remove_runs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29911 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/commands.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.737144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3872 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/optionGroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10099 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3600 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44081 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9480 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/column_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.737144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastore.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.737144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/composites.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5497 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/formatters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/dimensions.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.737144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/old_dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)    15088 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15094 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    15382 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/registry.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/repo_transfer_formats.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    14860 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/storageClasses.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.741144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57426 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41721 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/cache_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6068 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31187 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/file_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/generic_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9556 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/record_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13279 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/stored_file_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.741144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49806 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/chainedDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120549 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/fileDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/fileDatastoreClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.741144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22032 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27060 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/inMemoryDatastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23666 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/ddl.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.741144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrowastropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3005 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrownumpy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrownumpydict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrowtable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6195 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/dataframe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.745144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25254 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55578 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_coordinate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35795 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15002 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23173 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_elements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5963 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_governor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22884 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20362 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_packer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18368 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_record_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9725 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_record_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19888 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_skypix.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24448 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_universe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6905 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/construction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/record_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.745144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96587 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_butler/_direct_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.745144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/
+-rw-r--r--   0 runner    (1001) docker     (127)     1436 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56254 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/_driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8273 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23214 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/_query_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14516 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/_query_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10552 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.749144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/astropyTable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13339 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2079 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/matplotlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5009 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42716 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4063 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/pickle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6330 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18319 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10643 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/mapping_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/name_shrinker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3812 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8270 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/persistence_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19630 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/pydantic_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.749144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10234 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/_data_coordinate_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4927 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/_dataset_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4822 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/_dimension_record_query_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26172 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11185 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/convert_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14730 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19203 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/expression_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18228 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/overlaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10648 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/result_specs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.753144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6132 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8156 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_column_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10167 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_column_literal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5516 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_column_reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13642 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_column_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22448 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11675 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/_query_tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17181 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/visitors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.753144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_caching_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_record_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10735 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3196 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_summary_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4456 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_dataset_type_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7437 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60805 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_registry_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5921 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/attributes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.757144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/ephemeral.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16738 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/monolithic.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.757144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27734 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11833 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/nameKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12717 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/synthIntKey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/connectionString.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.757144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22475 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18122 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.757144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.757144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24042 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51063 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16706 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19243 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.757144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/dimensions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/dimensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54687 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/dimensions/static.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.761144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7258 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15351 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26746 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79984 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16907 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10902 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10371 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_opaque.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11950 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_versioning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/managers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/nameShrinker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.761144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16298 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11748 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_records.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10114 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6478 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4002 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/default_spatial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8129 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/pgsphere.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9639 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/opaque.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.765144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12630 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49430 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33980 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18361 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12089 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_readers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39215 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_results.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16320 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_sql_query_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25440 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_sql_query_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20955 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10143 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/butler_sql_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.765144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22509 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/categorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22911 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41024 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/normalForm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.765144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12944 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6624 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14359 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.765144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/ply/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/ply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43384 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137077 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8492 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/find_first_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114891 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/sql_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.765144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64445 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/_database.py
+-rw-r--r--   0 runner    (1001) docker     (127)   182650 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/wildcards.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.769144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_collection_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4817 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8256 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_http_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5164 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_ref_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12924 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22910 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_remote_butler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.769144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4304 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.769144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8811 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/handlers/_external.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/repo_relocation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.773144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/_associate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10265 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/_pruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/butlerImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3761 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/certifyCalibrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6166 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/collectionChain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2617 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/configDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/configValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/createRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6829 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/exportCalibs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8760 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/ingest_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7960 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8702 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3987 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/register_dataset_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/removeCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/removeDatasetType.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5286 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/removeRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/retrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/transferDatasets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.777144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1506 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8152 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_datasetsHelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_dummyRegistry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12966 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_examplePythonTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23754 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37730 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/butler_queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6994 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/cliCmdTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17098 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/cliLogTestBase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/deferredFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/dict_convertible_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14769 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/hybrid_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12712 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/hybrid_butler_registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6311 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2765 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/server_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9020 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/testFormatters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13344 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10120 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24302 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/timespan_database_representation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.777144 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16952 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6919 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/_interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32431 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.789144 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:29:36.000000 lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-01 21:29:36.793144 lsst_daf_butler-27.0.0rc1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:29:36.789144 lsst_daf_butler-27.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_astropyTableFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)   125454 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_butler_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdAssociate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9241 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdConfigDump.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdConfigValidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2884 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdCreate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2685 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdImport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4926 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdIngestFiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21626 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdPruneDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13078 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7706 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDataIds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10209 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDatasetTypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20652 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDatasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDimensionRecords.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10886 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdRemoveCollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdRemoveRuns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6048 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliCmdRetrieveArtifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliLog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6747 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliPluginLoader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliUtilSplitCommas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12494 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliUtilSplitKv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliUtilToUpper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16133 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_cliUtils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_composites.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25806 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_connectionString.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8403 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29972 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84810 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_ddl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17831 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_dimension_record_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45224 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_dimensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12157 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_exprParserLex.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24938 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_exprParserYacc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16014 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11208 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_logFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12245 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_matplotlibFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_nonempty_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7974 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_normalFormExpression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27146 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_obscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    83786 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11743 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11121 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_pydantic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8079 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_quantum.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18384 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_quantumBackedButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_query_direct_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_query_direct_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90560 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_query_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15859 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_query_relations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24397 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_query_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6876 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_remote_butler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17850 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38553 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_simpleButler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13698 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14764 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_storageClass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17643 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10862 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_testRepo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3050 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7187 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_time_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13053 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_timespan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8312 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9830 2024-05-01 21:29:30.000000 lsst_daf_butler-27.0.0rc1/tests/test_versioning.py
```

### Comparing `lsst-daf-butler-26.2024.900/PKG-INFO` & `lsst_daf_butler-27.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-daf-butler-26.2024.900/README.md` & `lsst_daf_butler-27.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/bsd_license.txt` & `lsst_daf_butler-27.0.0rc1/bsd_license.txt`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/CHANGES.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/CHANGES.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/concreteStorageClasses.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/concreteStorageClasses.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/configuring.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/configuring.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/datastores.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/datastores.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/formatters.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/formatters.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/index.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/index.rst`

 * *Files 26% similar despite different names*

```diff
@@ -97,56 +97,67 @@
 .. _lsst.daf.butler-pyapi:
 
 Python API reference
 ====================
 
 .. automodapi:: lsst.daf.butler
    :no-main-docstr:
+   :no-inherited-members:
    :skip: RegistryConfig
 
 Example datastores
 ------------------
 
 .. automodapi:: lsst.daf.butler.datastores.chainedDatastore
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.datastores.inMemoryDatastore
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.datastores.fileDatastore
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 Example formatters
 ------------------
 
 .. automodapi:: lsst.daf.butler.formatters.file
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.formatters.json
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.formatters.matplotlib
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.formatters.parquet
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.formatters.pickle
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 .. automodapi:: lsst.daf.butler.formatters.yaml
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 Test utilities
 --------------
 
 .. automodapi:: lsst.daf.butler.tests
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
    :no-inheritance-diagram:
 
 Middleware-Internal API
 =======================
 
 .. warning::
@@ -154,107 +165,128 @@
    These symbols are used throughout the middleware system and may be used in advanced middleware extensions (e.g. third-party `Datastore` implementations), but are not considered fully public interfaces in terms of stability guarantees.
 
 Datastore utilities
 -------------------
 
 .. automodapi:: lsst.daf.butler.datastore
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
    :skip: Datastore
 
 Registry utilities and interfaces
 ---------------------------------
 
 .. automodapi:: lsst.daf.butler.registry
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
    :skip: Registry
    :skip: CollectionType
 
 .. automodapi:: lsst.daf.butler.registry.interfaces
    :headings: ^"
+   :no-inherited-members:
    :no-main-docstr:
 
 .. automodapi:: lsst.daf.butler.registry.queries
    :headings: ^"
+   :no-inherited-members:
    :no-main-docstr:
 
 .. automodapi:: lsst.daf.butler.registry.wildcards
    :headings: ^"
+   :no-inherited-members:
    :no-main-docstr:
 
 Database backends
 -----------------
 
 .. automodapi:: lsst.daf.butler.registry.databases.sqlite
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.registry.databases.postgresql
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 General utilities
 -----------------
 
 .. automodapi:: lsst.daf.butler.arrow_utils
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.column_spec
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.ddl
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.json
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.logging
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.mapping_factory
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.nonempty_mapping
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.persistence_context
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.progress
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.pydantic_utils
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.repo_relocation
    :no-main-docstr:
    :headings: ^"
+   :no-inherited-members:
    :include-all-objects:
 
 .. automodapi:: lsst.daf.butler.time_utils
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.timespan_database_representation
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 .. automodapi:: lsst.daf.butler.utils
    :no-main-docstr:
+   :no-inherited-members:
    :headings: ^"
 
 Command-Line Interface Utilities
 --------------------------------
 
 .. automodapi:: lsst.daf.butler.cli.butler
    :no-main-docstr:
```

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/organizing.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/organizing.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/queries.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/queries.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/use-in-tests.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/use-in-tests.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/doc/lsst.daf.butler/writing-subcommands.rst` & `lsst_daf_butler-27.0.0rc1/doc/lsst.daf.butler/writing-subcommands.rst`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/gpl-v3.0.txt` & `lsst_daf_butler-27.0.0rc1/gpl-v3.0.txt`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/pyproject.toml` & `lsst_daf_butler-27.0.0rc1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -158,19 +158,23 @@
     "raise AssertionError",
     "raise NotImplementedError",
     "if __name__ == .__main__.:",
     "if TYPE_CHECKING:",
 ]
 
 [tool.ruff]
+line-length = 110
+target-version = "py311"
 exclude = [
     "__init__.py",
     "lex.py",
     "yacc.py",
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
@@ -179,38 +183,38 @@
     "D105",
     "D102",
     "D104",
     "D100",
     "D200",
     "D205",
     "D400",
+    "UP007",  # Allow UNION in type annotation
 ]
-line-length = 110
 select = [
     "E",  # pycodestyle
     "F",  # pycodestyle
     "N",  # pep8-naming
     "W",  # pycodestyle
     "D",  # pydocstyle
+    "UP",  # pyupgrade
 ]
-target-version = "py311"
 # Commented out to suppress "unused noqa" in jenkins which has older ruff not
 # generating E721.
 #extend-select = [
 #    "RUF100", # Warn about unused noqa
 #]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 # parserYacc docstrings can not be fixed. Docstrings are used to define grammar.
 "python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py" = ["D401", "D403"]
 
-[tool.ruff.pycodestyle]
+[tool.ruff.lint.pycodestyle]
 max-doc-length = 79
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "numpy"
 
 [tool.numpydoc_validation]
 checks = [
     "all",  # All except the rules listed below.
     "SA01",  # See Also section.
     "EX01",  # Example section.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 # Some components are not auto-imported since they can have additional runtime
 # dependencies.
 
 from . import logging  # most symbols are helpers only
 from . import progress  # most symbols are only used by handler implementors
 from . import ddl, time_utils
 from ._butler import *
+from ._butler_collections import *
 from ._butler_config import *
 from ._butler_repo_index import *
 from ._column_categorization import *
 from ._column_tags import *
 from ._column_type_info import *
 from ._config import *
 from ._config_support import LookupKey
@@ -56,16 +57,14 @@
 
 # Do not import 'json' at all by default.
 from ._limited_butler import *
 from ._location import *
 from ._named import *
 from ._quantum import *
 from ._quantum_backed import *
-from ._query import *
-from ._query_results import *
 from ._storage_class import *
 from ._storage_class_delegate import *
 from ._timespan import *
 from ._topology import *
 
 # Only lift 'Datastore' itself to this scope.
 from .datastore import Datastore
@@ -73,26 +72,28 @@
 
 # Only export 'ButlerLogRecords' from 'logging', import the module as-is for
 # other symbols. ButlerLogRecords is the fundamental type stored in datastores.
 from .logging import ButlerLogRecords
 
 # Do not import or lift symbols from mapping_factory and persistence_content,
 # as those are internal.
-# Only lift 'Progress' from 'progess'; the module is imported as-is above
+# Only lift 'Progress' from 'progress'; the module is imported as-is above
 from .progress import Progress
 
 # Do not import or lift symbols from 'server' or 'server_models'.
 # Import the registry subpackage directly for other symbols.
 from .registry import (
     CollectionType,
     MissingCollectionError,
-    MissingDatasetTypeError,
     NoDefaultCollectionError,
     Registry,
     RegistryConfig,
 )
 from .transfers import RepoExportContext, YamlRepoExportBackend, YamlRepoImportBackend
 from .version import *
 
+# Do not import or lift symbols from 'queries' until they are public.
+
+
 # Do not import or lift symbols from 'repo_relocation'.
 
 # Do not export the utility routines from utils.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,38 +32,41 @@
 from abc import abstractmethod
 from collections.abc import Collection, Iterable, Mapping, Sequence
 from contextlib import AbstractContextManager
 from typing import TYPE_CHECKING, Any, TextIO
 
 from lsst.resources import ResourcePath, ResourcePathExpression
 from lsst.utils import doImportType
+from lsst.utils.iteration import ensure_iterable
 from lsst.utils.logging import getLogger
 
+from ._butler_collections import ButlerCollections
 from ._butler_config import ButlerConfig, ButlerType
 from ._butler_instance_options import ButlerInstanceOptions
 from ._butler_repo_index import ButlerRepoIndex
 from ._config import Config, ConfigSubset
+from ._exceptions import EmptyQueryResultError
 from ._limited_butler import LimitedButler
 from .datastore import Datastore
 from .dimensions import DimensionConfig
 from .registry import RegistryConfig, _RegistryFactory
 from .repo_relocation import BUTLER_ROOT_TAG
 
 if TYPE_CHECKING:
     from ._dataset_existence import DatasetExistence
     from ._dataset_ref import DatasetId, DatasetRef
     from ._dataset_type import DatasetType
     from ._deferredDatasetHandle import DeferredDatasetHandle
     from ._file_dataset import FileDataset
-    from ._query import Query
     from ._storage_class import StorageClass
     from ._timespan import Timespan
     from .datastore import DatasetRefURIs
     from .dimensions import DataCoordinate, DataId, DimensionGroup, DimensionRecord
-    from .registry import CollectionArgType, Registry
+    from .queries import Query
+    from .registry import Registry
     from .transfers import RepoExportContext
 
 _LOG = getLogger(__name__)
 
 
 class Butler(LimitedButler):  # numpydoc ignore=PR02
     """Interface for data butler and factory for Butler instances.
@@ -582,14 +585,15 @@
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
         parameters: dict | None = None,
         collections: Any = None,
         storageClass: str | StorageClass | None = None,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> DeferredDatasetHandle:
         """Create a `DeferredDatasetHandle` which can later retrieve a dataset,
         after an immediate registry lookup.
 
         Parameters
         ----------
@@ -609,14 +613,19 @@
             to butler construction.
         storageClass : `StorageClass` or `str`, optional
             The storage class to be used to override the Python type
             returned by this method. By default the returned type matches
             the dataset type definition for this dataset. Specifying a
             read `StorageClass` can force a different type to be returned.
             This type must be compatible with the original type.
+        timespan : `Timespan` or `None`, optional
+            A timespan that the validity range of the dataset must overlap.
+            If not provided and this is a calibration dataset type, an attempt
+            will be made to find the timespan from any temporal coordinate
+            in the data ID.
         **kwargs
             Additional keyword arguments used to augment or construct a
             `DataId`.  See `DataId` parameters.
 
         Returns
         -------
         obj : `DeferredDatasetHandle`
@@ -641,14 +650,15 @@
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
         parameters: dict[str, Any] | None = None,
         collections: Any = None,
         storageClass: StorageClass | str | None = None,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> Any:
         """Retrieve a stored dataset.
 
         Parameters
         ----------
         datasetRefOrType : `DatasetRef`, `DatasetType`, or `str`
@@ -669,14 +679,19 @@
             to butler construction.
         storageClass : `StorageClass` or `str`, optional
             The storage class to be used to override the Python type
             returned by this method. By default the returned type matches
             the dataset type definition for this dataset. Specifying a
             read `StorageClass` can force a different type to be returned.
             This type must be compatible with the original type.
+        timespan : `Timespan` or `None`, optional
+            A timespan that the validity range of the dataset must overlap.
+            If not provided and this is a calibration dataset type, an attempt
+            will be made to find the timespan from any temporal coordinate
+            in the data ID.
         **kwargs
             Additional keyword arguments used to augment or construct a
             `DataCoordinate`.  See `DataCoordinate.standardize`
             parameters.
 
         Returns
         -------
@@ -1391,14 +1406,20 @@
             Raised if there is some inconsistency with how this Butler
             is configured.
         """
         raise NotImplementedError()
 
     @property
     @abstractmethod
+    def collection_chains(self) -> ButlerCollections:
+        """Object with methods for modifying collection chains."""
+        raise NotImplementedError()
+
+    @property
+    @abstractmethod
     def collections(self) -> Sequence[str]:
         """The collections to search by default, in order
         (`~collections.abc.Sequence` [ `str` ]).
         """
         raise NotImplementedError()
 
     @property
@@ -1424,26 +1445,24 @@
     @abstractmethod
     def _query(self) -> AbstractContextManager[Query]:
         """Context manager returning a `Query` object used for construction
         and execution of complex queries.
         """
         raise NotImplementedError()
 
-    @abstractmethod
     def _query_data_ids(
         self,
         dimensions: DimensionGroup | Iterable[str] | str,
         *,
         data_id: DataId | None = None,
         where: str = "",
         bind: Mapping[str, Any] | None = None,
-        expanded: bool = False,
+        with_dimension_records: bool = False,
         order_by: Iterable[str] | str | None = None,
         limit: int | None = None,
-        offset: int = 0,
         explain: bool = True,
         **kwargs: Any,
     ) -> list[DataCoordinate]:
         """Query for data IDs matching user-provided criteria.
 
         Parameters
         ----------
@@ -1462,27 +1481,23 @@
             :ref:`daf_butler_dimension_expressions` for more information.
         bind : `~collections.abc.Mapping`, optional
             Mapping containing literal values that should be injected into the
             ``where`` expression, keyed by the identifiers they replace.
             Values of collection type can be expanded in some cases; see
             :ref:`daf_butler_dimension_expressions_identifiers` for more
             information.
-        expanded : `bool`, optional
+        with_dimension_records : `bool`, optional
             If `True` (default is `False`) then returned data IDs will have
             dimension records.
         order_by : `~collections.abc.Iterable` [`str`] or `str`, optional
             Names of the columns/dimensions to use for ordering returned data
             IDs. Column name can be prefixed with minus (``-``) to use
             descending ordering.
         limit : `int`, optional
             Upper limit on the number of returned records.
-        offset : `int`, optional
-            The number of records to skip before returning at most ``limit``
-            records. If ``offset`` is specified then ``limit`` must be
-            specified as well.
         explain : `bool`, optional
             If `True` (default) then `EmptyQueryResultError` exception is
             raised when resulting list is empty. The exception contains
             non-empty list of strings explaining possible causes for empty
             result.
         **kwargs
             Additional keyword arguments are forwarded to
@@ -1504,72 +1519,76 @@
             dimensions or values, or when they contain inconsistent values.
         lsst.daf.butler.registry.UserExpressionError
             Raised when ``where`` expression is invalid.
         lsst.daf.butler.EmptyQueryResultError
             Raised when query generates empty result and ``explain`` is set to
             `True`.
         TypeError
-            Raised when the arguments are incompatible, e.g. ``offset`` is
-            specified, but ``limit`` is not.
+            Raised when the arguments are incompatible.
         """
-        raise NotImplementedError()
+        if data_id is None:
+            data_id = DataCoordinate.make_empty(self.dimensions)
+        with self._query() as query:
+            result = (
+                query.where(data_id, where, bind=bind, **kwargs)
+                .data_ids(dimensions)
+                .order_by(*ensure_iterable(order_by))
+                .limit(limit)
+            )
+            if with_dimension_records:
+                result = result.with_dimension_records()
+            data_ids = list(result)
+        if explain and not data_ids:
+            raise EmptyQueryResultError(list(result.explain_no_results()))
+        return data_ids
 
-    @abstractmethod
     def _query_datasets(
         self,
-        dataset_type: Any,
-        collections: CollectionArgType | None = None,
+        dataset_type: str | DatasetType,
+        collections: str | Iterable[str] | None = None,
         *,
         find_first: bool = True,
         data_id: DataId | None = None,
         where: str = "",
         bind: Mapping[str, Any] | None = None,
-        expanded: bool = False,
+        with_dimension_records: bool = False,
         explain: bool = True,
         **kwargs: Any,
     ) -> list[DatasetRef]:
         """Query for dataset references matching user-provided criteria.
 
         Parameters
         ----------
-        dataset_type : dataset type expression
-            An expression that fully or partially identifies the dataset types
-            to be queried.  Allowed types include `DatasetType`, `str`,
-            `re.Pattern`, and iterables thereof.  The special value ``...`` can
-            be used to query all dataset types.  See
-            :ref:`daf_butler_dataset_type_expressions` for more information.
+        dataset_type : `str` or `DatasetType`
+            Dataset type object or name to search for.
         collections : collection expression, optional
-            An expression that identifies the collections to search, such as a
-            `str` (for full matches or partial matches via globs), `re.Pattern`
-            (for partial matches), or iterable thereof.  ``...`` can be used to
-            search all collections (actually just all `~CollectionType.RUN`
-            collections, because this will still find all datasets).
-            If not provided, the default collections are used.  See
+            A collection name or iterable of collection names to search. If not
+            provided, the default collections are used.  See
             :ref:`daf_butler_collection_expressions` for more information.
         find_first : `bool`, optional
             If `True` (default), for each result data ID, only yield one
             `DatasetRef` of each `DatasetType`, from the first collection in
             which a dataset of that dataset type appears (according to the
             order of ``collections`` passed in).  If `True`, ``collections``
             must not contain regular expressions and may not be ``...``.
         data_id : `dict` or `DataCoordinate`, optional
-            A data ID whose key-value pairs are used as equality constraints
-            in the query.
+            A data ID whose key-value pairs are used as equality constraints in
+            the query.
         where : `str`, optional
-            A string expression similar to a SQL WHERE clause.  May involve
-            any column of a dimension table or (as a shortcut for the primary
-            key column of a dimension table) dimension name.  See
+            A string expression similar to a SQL WHERE clause.  May involve any
+            column of a dimension table or (as a shortcut for the primary key
+            column of a dimension table) dimension name.  See
             :ref:`daf_butler_dimension_expressions` for more information.
         bind : `~collections.abc.Mapping`, optional
             Mapping containing literal values that should be injected into the
-            ``where`` expression, keyed by the identifiers they replace.
-            Values of collection type can be expanded in some cases; see
+            ``where`` expression, keyed by the identifiers they replace. Values
+            of collection type can be expanded in some cases; see
             :ref:`daf_butler_dimension_expressions_identifiers` for more
             information.
-        expanded : `bool`, optional
+        with_dimension_records : `bool`, optional
             If `True` (default is `False`) then returned data IDs will have
             dimension records.
         explain : `bool`, optional
             If `True` (default) then `EmptyQueryResultError` exception is
             raised when resulting list is empty. The exception contains
             non-empty list of strings explaining possible causes for empty
             result.
@@ -1577,21 +1596,18 @@
             Additional keyword arguments are forwarded to
             `DataCoordinate.standardize` when processing the ``data_id``
             argument (and may be used to provide a constraining data ID even
             when the ``data_id`` argument is `None`).
 
         Returns
         -------
-        refs : `.queries.DatasetQueryResults`
+        refs : `.queries.DatasetRefQueryResults`
             Dataset references matching the given query criteria.  Nested data
             IDs are guaranteed to include values for all implied dimensions
-            (i.e. `DataCoordinate.hasFull` will return `True`), but will not
-            include dimension records (`DataCoordinate.hasRecords` will be
-            `False`) unless `~.queries.DatasetQueryResults.expanded` is
-            called on the result object (which returns a new one).
+            (i.e. `DataCoordinate.hasFull` will return `True`).
 
         Raises
         ------
         lsst.daf.butler.registry.DatasetTypeExpressionError
             Raised when ``dataset_type`` expression is invalid.
         lsst.daf.butler.registry.DataIdError
             Raised when ``data_id`` or keyword arguments specify unknown
@@ -1605,32 +1621,43 @@
             Raised when the arguments are incompatible, such as when a
             collection wildcard is passed when ``find_first`` is `True`, or
             when ``collections`` is `None` and default butler collections are
             not defined.
 
         Notes
         -----
-        When multiple dataset types are queried in a single call, the
-        results of this operation are equivalent to querying for each dataset
-        type separately in turn, and no information about the relationships
-        between datasets of different types is included.
-        """
-        raise NotImplementedError()
+        When multiple dataset types are queried in a single call, the results
+        of this operation are equivalent to querying for each dataset type
+        separately in turn, and no information about the relationships between
+        datasets of different types is included.
+        """
+        if data_id is None:
+            data_id = DataCoordinate.make_empty(self.dimensions)
+        with self._query() as query:
+            result = query.where(data_id, where, bind=bind, **kwargs).datasets(
+                dataset_type,
+                collections=collections,
+                find_first=find_first,
+            )
+            if with_dimension_records:
+                result = result.with_dimension_records()
+            refs = list(result)
+        if explain and not refs:
+            raise EmptyQueryResultError(list(result.explain_no_results()))
+        return refs
 
-    @abstractmethod
     def _query_dimension_records(
         self,
         element: str,
         *,
         data_id: DataId | None = None,
         where: str = "",
         bind: Mapping[str, Any] | None = None,
         order_by: Iterable[str] | str | None = None,
         limit: int | None = None,
-        offset: int = 0,
         explain: bool = True,
         **kwargs: Any,
     ) -> list[DimensionRecord]:
         """Query for dimension information matching user-provided criteria.
 
         Parameters
         ----------
@@ -1651,18 +1678,14 @@
             information.
         order_by : `~collections.abc.Iterable` [`str`] or `str`, optional
             Names of the columns/dimensions to use for ordering returned data
             IDs. Column name can be prefixed with minus (``-``) to use
             descending ordering.
         limit : `int`, optional
             Upper limit on the number of returned records.
-        offset : `int`, optional
-            The number of records to skip before returning at most ``limit``
-            records. If ``offset`` is specified then ``limit`` must be
-            specified as well.
         explain : `bool`, optional
             If `True` (default) then `EmptyQueryResultError` exception is
             raised when resulting list is empty. The exception contains
             non-empty list of strings explaining possible causes for empty
             result.
         **kwargs
             Additional keyword arguments are forwarded to
@@ -1687,15 +1710,27 @@
             `True`.
         TypeError
             Raised when the arguments are incompatible, such as when a
             collection wildcard is passed when ``find_first`` is `True`, or
             when ``collections`` is `None` and default butler collections are
             not defined.
         """
-        raise NotImplementedError()
+        if data_id is None:
+            data_id = DataCoordinate.make_empty(self.dimensions)
+        with self._query() as query:
+            result = (
+                query.where(data_id, where, bind=bind, **kwargs)
+                .dimension_records(element)
+                .order_by(*ensure_iterable(order_by))
+                .limit(limit)
+            )
+            dimension_records = list(result)
+        if explain and not dimension_records:
+            raise EmptyQueryResultError(list(result.explain_no_results()))
+        return dimension_records
 
     @abstractmethod
     def _clone(
         self,
         *,
         collections: Any = None,
         run: str | None = None,
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_config.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_instance_options.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_instance_options.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_butler_repo_index.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_butler_repo_index.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_categorization.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_column_categorization.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_tags.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_column_tags.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_column_type_info.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_column_type_info.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_config_support.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_config_support.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_association.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_association.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_existence.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_existence.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_ref.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_ref.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
         Datastore records to attach.
 
     Notes
     -----
     See also :ref:`daf_butler_organizing_datasets`
     """
 
-    _serializedType = SerializedDatasetRef
+    _serializedType: ClassVar[type[pydantic.BaseModel]] = SerializedDatasetRef
     __slots__ = (
         "_id",
         "datasetType",
         "dataId",
         "run",
         "_datastore_records",
     )
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_dataset_type.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_dataset_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         "_storageClass",
         "_storageClassName",
         "_parentStorageClass",
         "_parentStorageClassName",
         "_isCalibration",
     )
 
-    _serializedType = SerializedDatasetType
+    _serializedType: ClassVar[type[BaseModel]] = SerializedDatasetType
 
     VALID_NAME_REGEX = re.compile("^[a-zA-Z_][a-zA-Z0-9_]*(\\.[a-zA-Z_][a-zA-Z0-9_]*)*$")
 
     @staticmethod
     def nameWithComponent(datasetTypeName: str, componentName: str) -> str:
         """Form a valid DatasetTypeName from a parent and component.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_deferredDatasetHandle.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_deferredDatasetHandle.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_exceptions.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdImport.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,43 +21,50 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Specialized Butler exceptions."""
-__all__ = ("DatasetTypeNotSupportedError", "EmptyQueryResultError", "ValidationError")
+"""Unit tests for daf_butler CLI config-dump command.
+"""
 
+import unittest
+import unittest.mock
 
-class DatasetTypeNotSupportedError(RuntimeError):
-    """A `DatasetType` is not handled by this routine.
+from lsst.daf.butler.cli.cmd import butler_import
+from lsst.daf.butler.tests import CliCmdTestBase
 
-    This can happen in a `Datastore` when a particular `DatasetType`
-    has no formatters associated with it.
-    """
 
-    pass
+class ImportTestCase(CliCmdTestBase, unittest.TestCase):
+    """Test the butler import command-line."""
 
+    mockFuncName = "lsst.daf.butler.cli.cmd.commands.script.butlerImport"
 
-class ValidationError(RuntimeError):
-    """Some sort of validation error has occurred."""
+    @staticmethod
+    def defaultExpected():
+        return dict(repo=None, transfer="auto", directory=None, skip_dimensions=(), export_file=None)
 
-    pass
+    @staticmethod
+    def command():
+        return butler_import
 
+    def test_minimal(self):
+        """Test only required parameters, and omit optional parameters."""
+        self.run_test(["import", "here", "foo"], self.makeExpected(repo="here", directory="foo"))
 
-class EmptyQueryResultError(Exception):
-    """Exception raised when query methods return an empty result and `explain`
-    flag is set.
+    def test_all(self):
+        """Test all the parameters."""
+        self.run_test(
+            ["import", "here", "foo", "--transfer", "symlink", "--export-file", "file"],
+            self.makeExpected(repo="here", directory="foo", transfer="symlink", export_file="file"),
+        )
 
-    Parameters
-    ----------
-    reasons : `list` [`str`]
-        List of possible reasons for an empty query result.
-    """
+    def test_missingArgument(self):
+        """Verify the command fails if either of the positional arguments,
+        REPO or DIRECTORY, is missing.
+        """
+        self.run_missing(["import", "foo"], r"Error: Missing argument ['\"]DIRECTORY['\"].")
 
-    def __init__(self, reasons: list[str]):
-        self.reasons = reasons
 
-    def __str__(self) -> str:
-        # There may be multiple reasons, format them into multiple lines.
-        return "Possible reasons for empty result:\n" + "\n".join(self.reasons)
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_dataset.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_file_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_file_descriptor.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_file_descriptor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_formatter.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_labeled_butler_factory.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_labeled_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_limited_butler.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_limited_butler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_location.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_location.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_named.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_named.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_quantum.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_quantum_backed.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_quantum_backed.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_summary.py`

 * *Files 22% similar despite different names*

```diff
@@ -20,235 +20,252 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-
 from __future__ import annotations
 
-__all__ = ("Query",)
+__all__ = ("CollectionSummary", "SerializedCollectionSummary")
 
-from abc import ABC, abstractmethod
-from collections.abc import Iterable, Mapping
-from typing import TYPE_CHECKING, Any
+import dataclasses
+from collections.abc import Generator, Iterable, Mapping, Set
+from typing import cast
 
-if TYPE_CHECKING:
-    from ._query_results import DataCoordinateQueryResults, DatasetQueryResults, DimensionRecordQueryResults
-    from .dimensions import DataId, DimensionGroup
-    from .registry._registry import CollectionArgType
+import pydantic
 
+from .._dataset_ref import DatasetRef
+from .._dataset_type import DatasetType, SerializedDatasetType
+from .._named import NamedValueSet
+from ..dimensions import DataCoordinate, DimensionUniverse
 
-class Query(ABC):
-    """Interface for construction and execution of complex queries."""
 
-    @abstractmethod
-    def data_ids(
-        self,
-        dimensions: DimensionGroup | Iterable[str] | str,
-        *,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> DataCoordinateQueryResults:
-        """Query for data IDs matching user-provided criteria.
+@dataclasses.dataclass
+class CollectionSummary:
+    """A summary of the datasets that can be found in a collection."""
 
-        Parameters
-        ----------
-        dimensions : `DimensionGroup`, `str`, or \
-                `~collections.abc.Iterable` [`str`]
-            The dimensions of the data IDs to yield, as either `DimensionGroup`
-            instances or `str`.  Will be automatically expanded to a complete
-            `DimensionGroup`.
-        data_id : `dict` or `DataCoordinate`, optional
-            A data ID whose key-value pairs are used as equality constraints
-            in the query.
-        where : `str`, optional
-            A string expression similar to a SQL WHERE clause.  May involve
-            any column of a dimension table or (as a shortcut for the primary
-            key column of a dimension table) dimension name.  See
-            :ref:`daf_butler_dimension_expressions` for more information.
-        bind : `~collections.abc.Mapping`, optional
-            Mapping containing literal values that should be injected into the
-            ``where`` expression, keyed by the identifiers they replace.
-            Values of collection type can be expanded in some cases; see
-            :ref:`daf_butler_dimension_expressions_identifiers` for more
-            information.
-        **kwargs
-            Additional keyword arguments are forwarded to
-            `DataCoordinate.standardize` when processing the ``data_id``
-            argument (and may be used to provide a constraining data ID even
-            when the ``data_id`` argument is `None`).
+    def copy(self) -> CollectionSummary:
+        """Return a deep copy of this object.
 
         Returns
         -------
-        dataIds : `DataCoordinateQueryResults`
-            Data IDs matching the given query parameters.  These are guaranteed
-            to identify all dimensions (`DataCoordinate.hasFull` returns
-            `True`), but will not contain `DimensionRecord` objects
-            (`DataCoordinate.hasRecords` returns `False`).  Call
-            `~DataCoordinateQueryResults.expanded` on the
-            returned object to fetch those (and consider using
-            `~DataCoordinateQueryResults.materialize` on the
-            returned object first if the expected number of rows is very
-            large). See documentation for those methods for additional
-            information.
+        copy : `CollectionSummary`
+            A copy of ``self`` that can be modified without modifying ``self``
+            at all.
+        """
+        return CollectionSummary(
+            dataset_types=self.dataset_types.copy(), governors=_copy_governors(self.governors)
+        )
+
+    def add_datasets_generator(self, refs: Iterable[DatasetRef]) -> Generator[DatasetRef, None, None]:
+        """Include the given datasets in the summary, yielding them back as a
+        generator.
 
-        Raises
+        Parameters
+        ----------
+        refs : `~collections.abc.Iterable` [ `DatasetRef` ]
+            Datasets to include.
+
+        Yields
         ------
-        lsst.daf.butler.registry.DataIdError
-            Raised when ``data_id`` or keyword arguments specify unknown
-            dimensions or values, or when they contain inconsistent values.
-        lsst.daf.butler.registry.UserExpressionError
-            Raised when ``where`` expression is invalid.
+        ref : `DatasetRef`
+            The same dataset references originally passed in.
+
+        Notes
+        -----
+        As a generator, this method does nothing if its return iterator is not
+        used.  Call `add_datasets` instead to avoid this; this method is
+        intended for the case where the given iterable may be single-pass and a
+        copy is not desired, but other processing needs to be done on its
+        elements.
         """
-        raise NotImplementedError()
+        for ref in refs:
+            self.dataset_types.add(ref.datasetType)
+            for gov in ref.dataId.dimensions.governors:
+                self.governors.setdefault(gov, set()).add(cast(str, ref.dataId[gov]))
+            yield ref
 
-    @abstractmethod
-    def datasets(
-        self,
-        dataset_type: Any,
-        collections: CollectionArgType | None = None,
-        *,
-        find_first: bool = True,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> DatasetQueryResults:
-        """Query for and iterate over dataset references matching user-provided
-        criteria.
+    def add_datasets(self, refs: Iterable[DatasetRef]) -> None:
+        """Include the given datasets in the summary.
 
         Parameters
         ----------
-        dataset_type : dataset type expression
-            An expression that fully or partially identifies the dataset types
-            to be queried.  Allowed types include `DatasetType`, `str`,
-            `re.Pattern`, and iterables thereof.  The special value ``...`` can
-            be used to query all dataset types.  See
-            :ref:`daf_butler_dataset_type_expressions` for more information.
-        collections : collection expression, optional
-            An expression that identifies the collections to search, such as a
-            `str` (for full matches or partial matches via globs), `re.Pattern`
-            (for partial matches), or iterable thereof.  ``...`` can be used to
-            search all collections (actually just all `~CollectionType.RUN`
-            collections, because this will still find all datasets).
-            If not provided, the default collections are used.  See
-            :ref:`daf_butler_collection_expressions` for more information.
-        find_first : `bool`, optional
-            If `True` (default), for each result data ID, only yield one
-            `DatasetRef` of each `DatasetType`, from the first collection in
-            which a dataset of that dataset type appears (according to the
-            order of ``collections`` passed in).  If `True`, ``collections``
-            must not contain regular expressions and may not be ``...``.
-        data_id : `dict` or `DataCoordinate`, optional
-            A data ID whose key-value pairs are used as equality constraints
-            in the query.
-        where : `str`, optional
-            A string expression similar to a SQL WHERE clause.  May involve
-            any column of a dimension table or (as a shortcut for the primary
-            key column of a dimension table) dimension name.  See
-            :ref:`daf_butler_dimension_expressions` for more information.
-        bind : `~collections.abc.Mapping`, optional
-            Mapping containing literal values that should be injected into the
-            ``where`` expression, keyed by the identifiers they replace.
-            Values of collection type can be expanded in some cases; see
-            :ref:`daf_butler_dimension_expressions_identifiers` for more
-            information.
-        **kwargs
-            Additional keyword arguments are forwarded to
-            `DataCoordinate.standardize` when processing the ``data_id``
-            argument (and may be used to provide a constraining data ID even
-            when the ``data_id`` argument is `None`).
+        refs : `~collections.abc.Iterable` [ `DatasetRef` ]
+            Datasets to include.
+        """
+        for _ in self.add_datasets_generator(refs):
+            pass
 
-        Returns
-        -------
-        refs : `.queries.DatasetQueryResults`
-            Dataset references matching the given query criteria.  Nested data
-            IDs are guaranteed to include values for all implied dimensions
-            (i.e. `DataCoordinate.hasFull` will return `True`), but will not
-            include dimension records (`DataCoordinate.hasRecords` will be
-            `False`) unless `~.queries.DatasetQueryResults.expanded` is
-            called on the result object (which returns a new one).
+    def add_data_ids_generator(
+        self, dataset_type: DatasetType, data_ids: Iterable[DataCoordinate]
+    ) -> Generator[DataCoordinate, None, None]:
+        """Include the given dataset type and data IDs in the summary, yielding
+        them back as a generator.
 
-        Raises
+        Parameters
+        ----------
+        dataset_type : `DatasetType`
+            Dataset type to include.
+        data_ids : `~collections.abc.Iterable` [ `DataCoordinate` ]
+            Data IDs to include.
+
+        Yields
         ------
-        lsst.daf.butler.registry.DatasetTypeExpressionError
-            Raised when ``dataset_type`` expression is invalid.
-        TypeError
-            Raised when the arguments are incompatible, such as when a
-            collection wildcard is passed when ``find_first`` is `True`, or
-            when ``collections`` is `None` and default butler collections are
-            not defined.
-        lsst.daf.butler.registry.DataIdError
-            Raised when ``data_id`` or keyword arguments specify unknown
-            dimensions or values, or when they contain inconsistent values.
-        lsst.daf.butler.registry.UserExpressionError
-            Raised when ``where`` expression is invalid.
+        data_id : `DataCoordinate`
+            The same data IDs originally passed in.
 
         Notes
         -----
-        When multiple dataset types are queried in a single call, the
-        results of this operation are equivalent to querying for each dataset
-        type separately in turn, and no information about the relationships
-        between datasets of different types is included.
+        As a generator, this method does nothing if its return iterator is not
+        used.  Call `add_data_ids` instead to avoid this; this method is
+        intended for the case where the given iterable may be single-pass and a
+        copy is not desired, but other processing needs to be done on its
+        elements.
         """
-        raise NotImplementedError()
+        self.dataset_types.add(dataset_type)
+        for data_id in data_ids:
+            for gov in data_id.dimensions.governors:
+                self.governors.setdefault(gov, set()).add(cast(str, data_id[gov]))
+            yield data_id
 
-    @abstractmethod
-    def dimension_records(
-        self,
-        element: str,
-        *,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        **kwargs: Any,
-    ) -> DimensionRecordQueryResults:
-        """Query for dimension information matching user-provided criteria.
+    def add_data_ids(self, dataset_type: DatasetType, data_ids: Iterable[DataCoordinate]) -> None:
+        """Include the given dataset type and data IDs in the summary.
+
+        Parameters
+        ----------
+        dataset_type : `DatasetType`
+            Dataset type to include.
+        data_ids : `~collections.abc.Iterable` [ `DataCoordinate` ]
+            Data IDs to include.
+        """
+        for _ in self.add_data_ids_generator(dataset_type, data_ids):
+            pass
+
+    def update(self, *args: CollectionSummary) -> None:
+        """Update this summary with dataset types and governor dimension values
+        from other summaries.
+
+        Parameters
+        ----------
+        *args : `CollectionSummary`
+            Summaries to include in ``self``.
+        """
+        for arg in args:
+            self.dataset_types.update(arg.dataset_types)
+            for gov, values in arg.governors.items():
+                self.governors.setdefault(gov, set()).update(values)
+
+    def union(*args: CollectionSummary) -> CollectionSummary:
+        """Construct a summary that contains all dataset types and governor
+        dimension values in any of the inputs.
 
         Parameters
         ----------
-        element : `str`
-            The name of a dimension element to obtain records for.
-        data_id : `dict` or `DataCoordinate`, optional
-            A data ID whose key-value pairs are used as equality constraints
-            in the query.
-        where : `str`, optional
-            A string expression similar to a SQL WHERE clause.  See
-            `queryDataIds` and :ref:`daf_butler_dimension_expressions` for more
-            information.
-        bind : `~collections.abc.Mapping`, optional
-            Mapping containing literal values that should be injected into the
-            ``where`` expression, keyed by the identifiers they replace.
-            Values of collection type can be expanded in some cases; see
-            :ref:`daf_butler_dimension_expressions_identifiers` for more
-            information.
-        **kwargs
-            Additional keyword arguments are forwarded to
-            `DataCoordinate.standardize` when processing the ``data_id``
-            argument (and may be used to provide a constraining data ID even
-            when the ``data_id`` argument is `None`).
+        *args : `CollectionSummary`
+            Summaries to combine.
 
         Returns
         -------
-        records : `.queries.DimensionRecordQueryResults`
-            Data IDs matching the given query parameters.
+        unioned : `CollectionSummary`
+            New summary object that represents the union of the given ones.
+        """
+        result = CollectionSummary()
+        result.update(*args)
+        return result
 
-        Raises
-        ------
-        lsst.daf.butler.registry.NoDefaultCollectionError
-            Raised if ``collections`` is `None` and
-            ``self.defaults.collections`` is `None`.
-        lsst.daf.butler.registry.CollectionExpressionError
-            Raised when ``collections`` expression is invalid.
-        lsst.daf.butler.registry.DataIdError
-            Raised when ``data_id`` or keyword arguments specify unknown
-            dimensions or values, or when they contain inconsistent values.
-        lsst.daf.butler.registry.DatasetTypeExpressionError
-            Raised when ``datasetType`` expression is invalid.
-        lsst.daf.butler.registry.UserExpressionError
-            Raised when ``where`` expression is invalid.
+    def is_compatible_with(
+        self,
+        dataset_type: DatasetType,
+        dimensions: Mapping[str, Set[str]],
+        rejections: list[str] | None = None,
+        name: str | None = None,
+    ) -> bool:
+        """Test whether the collection summarized by this object should be
+        queried for a given dataset type and governor dimension values.
+
+        Parameters
+        ----------
+        dataset_type : `DatasetType`
+            Dataset type being queried.  If this collection has no instances of
+            this dataset type (or its parent dataset type, if it is a
+            component), `False` will always be returned.
+        dimensions : `~collections.abc.Mapping`
+            Bounds on the values governor dimensions can take in the query,
+            usually from a WHERE expression, as a mapping from dimension name
+            to a set of `str` governor dimension values.
+        rejections : `list` [ `str` ], optional
+            If provided, a list that will be populated with a log- or
+            exception-friendly message explaining why this dataset is
+            incompatible with this collection when `False` is returned.
+        name : `str`, optional
+            Name of the collection this object summarizes, for use in messages
+            appended to ``rejections``.  Ignored if ``rejections`` is `None`.
+
+        Returns
+        -------
+        compatible : `bool`
+            `True` if the dataset query described by this summary and the given
+            arguments might yield non-empty results; `False` if the result from
+            such a query is definitely empty.
         """
-        raise NotImplementedError()
+        parent = dataset_type if not dataset_type.isComponent() else dataset_type.makeCompositeDatasetType()
+        if parent.name not in self.dataset_types.names:
+            if rejections is not None:
+                rejections.append(f"No datasets of type {parent.name} in collection {name!r}.")
+            return False
+        for gov_name in self.governors.keys() & dataset_type.dimensions.names & dimensions.keys():
+            values_in_collection = self.governors[gov_name]
+            values_given = dimensions[gov_name]
+            if values_in_collection.isdisjoint(values_given):
+                if rejections is not None:
+                    rejections.append(
+                        f"No datasets with {gov_name} in {values_given} in collection {name!r}."
+                    )
+                return False
+        return True
+
+    def to_simple(self) -> SerializedCollectionSummary:
+        return SerializedCollectionSummary(
+            dataset_types=[x.to_simple() for x in self.dataset_types],
+            governors=_copy_governors(self.governors),
+        )
+
+    @staticmethod
+    def from_simple(simple: SerializedCollectionSummary, universe: DimensionUniverse) -> CollectionSummary:
+        summary = CollectionSummary()
+        summary.dataset_types = NamedValueSet(
+            [DatasetType.from_simple(x, universe) for x in simple.dataset_types]
+        )
+        summary.governors = _copy_governors(simple.governors)
+        return summary
+
+    dataset_types: NamedValueSet[DatasetType] = dataclasses.field(default_factory=NamedValueSet)
+    """Dataset types that may be present in the collection
+    (`NamedValueSet` [ `DatasetType` ]).
+
+    A dataset type not in this set is definitely not in the collection, but
+    the converse is not necessarily true.
+    """
+
+    governors: dict[str, set[str]] = dataclasses.field(default_factory=dict)
+    """Governor data ID values that are present in the collection's dataset
+    data IDs (`dict` [ `str`, `set` [ `str` ] ]).
+
+    A data ID value not in this restriction is not necessarily inconsistent
+    with a query in the collection; such a search may only involve dataset
+    types that do not include one or more governor dimensions in their data
+    IDs, and hence the values of those data IDs are unconstrained by this
+    collection in the query.
+    """
+
+
+def _copy_governors(governors: dict[str, set[str]]) -> dict[str, set[str]]:
+    """Make an independent copy of the 'governors' data structure."""
+    return {k: v.copy() for k, v in governors.items()}
+
+
+class SerializedCollectionSummary(pydantic.BaseModel):
+    """Serialized version of CollectionSummary."""
+
+    dataset_types: list[SerializedDatasetType]
+    governors: dict[str, set[str]]
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_query_results.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_testRepo.py`

 * *Files 20% similar despite different names*

```diff
@@ -23,706 +23,570 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
-__all__ = (
-    "DataCoordinateQueryResults",
-    "DatasetQueryResults",
-    "DimensionRecordQueryResults",
-    "SingleTypeDatasetQueryResults",
-)
+__all__ = [
+    "makeTestRepo",
+    "makeTestCollection",
+    "addDatasetType",
+    "expandUniqueId",
+    "DatastoreMock",
+    "addDataIdValue",
+]
 
-from abc import abstractmethod
-from collections.abc import Iterable, Iterator
-from contextlib import AbstractContextManager
+import random
+from collections.abc import Iterable, Mapping
 from typing import TYPE_CHECKING, Any
+from unittest.mock import MagicMock
 
-from ._dataset_ref import DatasetRef
-from .dimensions import DataCoordinate, DimensionRecord
+import sqlalchemy
+from lsst.daf.butler import (
+    Butler,
+    Config,
+    DataCoordinate,
+    DatasetRef,
+    DatasetType,
+    Dimension,
+    DimensionUniverse,
+    FileDataset,
+    StorageClass,
+)
 
 if TYPE_CHECKING:
-    from ._dataset_type import DatasetType
-    from .dimensions import DimensionElement, DimensionGroup
-
-
-class DataCoordinateQueryResults(Iterable[DataCoordinate]):
-    """An interface for objects that represent the results of queries for
-    data IDs.
-    """
-
-    @property
-    @abstractmethod
-    def dimensions(self) -> DimensionGroup:
-        """The dimensions of the data IDs returned by this query."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def has_full(self) -> bool:
-        """Indicate if all data IDs in this iterable identify all dimensions,
-        not just required dimensions.
-
-        Returns
-        -------
-        state : `bool`
-            If `True`, ``all(d.hasFull() for d in self)`` is guaranteed.
-            If `False`, no guarantees are made.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def has_records(self) -> bool:
-        """Return whether all data IDs in this iterable contain records.
-
-        Returns
-        -------
-        state : `bool`
-            If `True`, ``all(d.hasRecords() for d in self)`` is guaranteed.
-            If `False`, no guarantees are made.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def materialize(self) -> AbstractContextManager[DataCoordinateQueryResults]:
-        """Insert this query's results into a temporary table.
-
-        Returns
-        -------
-        context : `typing.ContextManager` [ `DataCoordinateQueryResults` ]
-            A context manager that ensures the temporary table is created and
-            populated in ``__enter__`` (returning a results object backed by
-            that table), and dropped in ``__exit__``.  If ``self`` is already
-            materialized, the context manager may do nothing (reflecting the
-            fact that an outer context manager should already take care of
-            everything else).
-
-        Notes
-        -----
-        When using a very large result set to perform multiple queries (e.g.
-        multiple calls to `subset` with different arguments, or even a single
-        call to `expanded`), it may be much more efficient to start by
-        materializing the query and only then performing the follow up queries.
-        It may also be less efficient, depending on how well database engine's
-        query optimizer can simplify those particular follow-up queries and
-        how efficiently it caches query results even when the are not
-        explicitly inserted into a temporary table.  See `expanded` and
-        `subset` for examples.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def expanded(self) -> DataCoordinateQueryResults:
-        """Return a results object for which `has_records` returns `True`.
-
-        This method may involve actually executing database queries to fetch
-        `DimensionRecord` objects.
-
-        Returns
-        -------
-        results : `DataCoordinateQueryResults`
-            A results object for which `has_records` returns `True`.  May be
-            ``self`` if that is already the case.
-
-        Notes
-        -----
-        For very result sets, it may be much more efficient to call
-        `materialize` before calling `expanded`, to avoid performing the
-        original query multiple times (as a subquery) in the follow-up queries
-        that fetch dimension records.  For example::
-
-            with butler.query() as query:
-                with query.data_ids(...).materialize() as tempDataIds:
-                    dataIdsWithRecords = tempDataIds.expanded()
-                    for dataId in dataIdsWithRecords:
-                        ...
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def subset(
-        self,
-        dimensions: DimensionGroup | Iterable[str] | None = None,
-        *,
-        unique: bool = False,
-    ) -> DataCoordinateQueryResults:
-        """Return a results object containing a subset of the dimensions of
-        this one, and/or a unique near-subset of its rows.
-
-        This method may involve actually executing database queries to fetch
-        `DimensionRecord` objects.
-
-        Parameters
-        ----------
-        dimensions : `DimensionGroup` or \
-                `~collections.abc.Iterable` [ `str`], optional
-            Dimensions to include in the new results object.  If `None`,
-            ``self.dimensions`` is used.
-        unique : `bool`, optional
-            If `True` (`False` is default), the query should only return unique
-            data IDs.  This is implemented in the database; to obtain unique
-            results via Python-side processing (which may be more efficient in
-            some cases), use `toSet` to construct a `DataCoordinateSet` from
-            this results object instead.
-
-        Returns
-        -------
-        results : `DataCoordinateQueryResults`
-            A results object corresponding to the given criteria.  May be
-            ``self`` if it already qualifies.
-
-        Raises
-        ------
-        ValueError
-            Raised when ``dimensions`` is not a subset of the dimensions in
-            this result.
-
-        Notes
-        -----
-        This method can only return a "near-subset" of the original result rows
-        in general because of subtleties in how spatial overlaps are
-        implemented; see `Query.projected` for more information.
-
-        When calling `subset` multiple times on the same very large result set,
-        it may be much more efficient to call `materialize` first.  For
-        example::
-
-            dimensions1 = DimensionGroup(...)
-            dimensions2 = DimensionGroup(...)
-            with butler.query(...)as query:
-                with query.data_ids(...).materialize() as data_ids:
-                    for dataId1 in data_ids.subset(dimensions1, unique=True):
-                        ...
-                    for dataId2 in data_ids.subset(dimensions2, unique=True):
-                        ...
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def find_datasets(
-        self, dataset_type: DatasetType | str, collections: Any, *, find_first: bool = True
-    ) -> DatasetQueryResults:
-        """Find datasets using the data IDs identified by this query.
-
-        Parameters
-        ----------
-        dataset_type : `DatasetType` or `str`
-            Dataset type or the name of one to search for.  Must have
-            dimensions that are a subset of ``self.dimensions``.
-        collections : `Any`
-            An expression that fully or partially identifies the collections
-            to search for the dataset, such as a `str`, `re.Pattern`, or
-            iterable  thereof.  ``...`` can be used to return all collections.
-            See :ref:`daf_butler_collection_expressions` for more information.
-        find_first : `bool`, optional
-            If `True` (default), for each result data ID, only yield one
-            `DatasetRef`, from the first collection in which a dataset of that
-            dataset type appears (according to the order of ``collections``
-            passed in).  If `True`, ``collections`` must not contain regular
-            expressions and may not be ``...``.
-
-        Returns
-        -------
-        datasets : `ParentDatasetQueryResults`
-            A lazy-evaluation object representing dataset query results,
-            iterable over `DatasetRef` objects.  If ``self.has_records()``, all
-            nested data IDs in those dataset references will have records as
-            well.
-
-        Raises
-        ------
-        MissingDatasetTypeError
-            Raised if the given dataset type is not registered.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def find_related_datasets(
-        self,
-        dataset_type: DatasetType | str,
-        collections: Any,
-        *,
-        find_first: bool = True,
-        dimensions: DimensionGroup | Iterable[str] | None = None,
-    ) -> Iterable[tuple[DataCoordinate, DatasetRef]]:
-        """Find datasets using the data IDs identified by this query, and
-        return them along with the original data IDs.
-
-        This is a variant of `find_datasets` that is often more useful when
-        the target dataset type does not have all of the dimensions of the
-        original data ID query, as is generally the case with calibration
-        lookups.
-
-        Parameters
-        ----------
-        dataset_type : `DatasetType` or `str`
-            Dataset type or the name of one to search for.  Must have
-            dimensions that are a subset of ``self.dimensions``.
-        collections : `Any`
-            An expression that fully or partially identifies the collections
-            to search for the dataset, such as a `str`, `re.Pattern`, or
-            iterable  thereof.  ``...`` can be used to return all collections.
-            See :ref:`daf_butler_collection_expressions` for more information.
-        find_first : `bool`, optional
-            If `True` (default), for each data ID in ``self``, only yield one
-            `DatasetRef`, from the first collection in which a dataset of that
-            dataset type appears (according to the order of ``collections``
-            passed in).  If `True`, ``collections`` must not contain regular
-            expressions and may not be ``...``.  Note that this is not the
-            same as yielding one `DatasetRef` for each yielded data ID if
-            ``dimensions`` is not `None`.
-        dimensions : `DimensionGroup`, or \
-                `~collections.abc.Iterable` [ `str` ], optional
-            The dimensions of the data IDs returned.  Must be a subset of
-            ``self.dimensions``.
-
-        Returns
-        -------
-        pairs : `~collections.abc.Iterable` [ `tuple` [ `DataCoordinate`, \
-                `DatasetRef` ] ]
-            An iterable of (data ID, dataset reference) pairs.
-
-        Raises
-        ------
-        MissingDatasetTypeError
-            Raised if the given dataset type is not registered.
-        """
-        raise NotImplementedError()
+    from lsst.daf.butler import DatasetId
 
-    @abstractmethod
-    def count(self, *, exact: bool = True, discard: bool = False) -> int:
-        """Count the number of rows this query would return.
 
-        Parameters
-        ----------
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed to account for that filtering in the count.  If `False`, the
-            result may be an upper bound.
-        discard : `bool`, optional
-            If `True`, compute the exact count even if it would require running
-            the full query and then throwing away the result rows after
-            counting them.  If `False`, this is an error, as the user would
-            usually be better off executing the query first to fetch its rows
-            into a new query (or passing ``exact=False``).  Ignored if
-            ``exact=False``.
-
-        Returns
-        -------
-        count : `int`
-            The number of rows the query would return, or an upper bound if
-            ``exact=False``.
-
-        Notes
-        -----
-        This counts the number of rows returned, not the number of unique rows
-        returned, so even with ``exact=True`` it may provide only an upper
-        bound on the number of *deduplicated* result rows.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def any(self, *, execute: bool = True, exact: bool = True) -> bool:
-        """Test whether this query returns any results.
-
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True`, execute at least a ``LIMIT 1`` query if it cannot be
-            determined prior to execution that the query would return no rows.
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed, until at least one result row is found.  If `False`, the
-            returned result does not account for post-query filtering, and
-            hence may be `True` even when all result rows would be filtered
-            out.
-
-        Returns
-        -------
-        any : `bool`
-            `True` if the query would (or might, depending on arguments) yield
-            result rows.  `False` if it definitely would not.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def explain_no_results(self, execute: bool = True) -> Iterable[str]:
-        """Return human-readable messages that may help explain why the query
-        yields no results.
-
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True` (default) execute simplified versions (e.g. ``LIMIT 1``)
-            of aspects of the tree to more precisely determine where rows were
-            filtered out.
-
-        Returns
-        -------
-        messages : `~collections.abc.Iterable` [ `str` ]
-            String messages that describe reasons the query might not yield any
-            results.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def order_by(self, *args: str) -> DataCoordinateQueryResults:
-        """Make the iterator return ordered results.
-
-        Parameters
-        ----------
-        *args : `str`
-            Names of the columns/dimensions to use for ordering. Column name
-            can be prefixed with minus (``-``) to use descending ordering.
-
-        Returns
-        -------
-        result : `DataCoordinateQueryResults`
-            Returns ``self`` instance which is updated to return ordered
-            result.
-
-        Notes
-        -----
-        This method modifies the iterator in place and returns the same
-        instance to support method chaining.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def limit(self, limit: int | None = None, offset: int = 0) -> DataCoordinateQueryResults:
-        """Make the iterator return limited number of records.
-
-        Parameters
-        ----------
-        limit : `int` or `None`, optional
-            Upper limit on the number of returned records.  `None` (default) is
-            no limit.
-        offset : `int`, optional
-            The number of records to skip before returning at most ``limit``
-            records.
-
-        Returns
-        -------
-        result : `DataCoordinateQueryResults`
-            Returns ``self`` instance which is updated to return limited set
-            of records.
-
-        Notes
-        -----
-        This method modifies the iterator in place and returns the same
-        instance to support method chaining. Normally this method is used
-        together with `order_by` method.
-        """
-        raise NotImplementedError()
-
-
-class DatasetQueryResults(Iterable[DatasetRef]):
-    """An interface for objects that represent the results of queries for
-    datasets.
+def makeTestRepo(
+    root: str, dataIds: Mapping[str, Iterable] | None = None, *, config: Config | None = None, **kwargs: Any
+) -> Butler:
+    """Create an empty test repository.
+
+    Parameters
+    ----------
+    root : `str`
+        The location of the root directory for the repository.
+    dataIds : `~collections.abc.Mapping` [`str`, `iterable`], optional
+        A mapping keyed by the dimensions used in the test. Each value is an
+        iterable of names for that dimension (e.g., detector IDs for
+        `"detector"`). Related dimensions (e.g., instruments and detectors) are
+        linked arbitrarily, with values created for implied dimensions only
+        when needed. This parameter is provided for compatibility with old
+        code; newer code should make the repository, then call
+        `~lsst.daf.butler.tests.addDataIdValue`.
+    config : `lsst.daf.butler.Config`, optional
+        A configuration for the repository (for details, see
+        `lsst.daf.butler.Butler.makeRepo`). If omitted, creates a repository
+        with default dataset and storage types, but optimized for speed.  The
+        defaults set ``.datastore.cls``, ``.datastore.checksum`` and
+        ``.registry.db``.  If a supplied config does not specify these values
+        the internal defaults will be used to ensure that we have a usable
+        configuration.
+    **kwargs
+        Extra arguments to `lsst.daf.butler.Butler.makeRepo`.
+
+    Returns
+    -------
+    butler : `lsst.daf.butler.Butler`
+        A Butler referring to the new repository. This Butler is provided only
+        for additional setup; to keep test cases isolated, it is highly
+        recommended that each test create its own Butler with a unique
+        run/collection. See `makeTestCollection`.
+
+    Notes
+    -----
+    This function provides a "quick and dirty" repository for simple unit tests
+    that don't depend on complex data relationships. It is ill-suited for tests
+    where the structure of the data matters. If you need such a dataset, create
+    it directly or use a saved test dataset.
     """
-
-    @abstractmethod
-    def by_dataset_type(self) -> Iterator[SingleTypeDatasetQueryResults]:
-        """Group results by dataset type.
-
-        Returns
-        -------
-        iter : `~collections.abc.Iterator` [ `SingleTypeDatasetQueryResults` ]
-            An iterator over `DatasetQueryResults` instances that are each
-            responsible for a single dataset type.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def materialize(self) -> AbstractContextManager[DatasetQueryResults]:
-        """Insert this query's results into a temporary table.
-
-        Returns
-        -------
-        context : `typing.ContextManager` [ `DatasetQueryResults` ]
-            A context manager that ensures the temporary table is created and
-            populated in ``__enter__`` (returning a results object backed by
-            that table), and dropped in ``__exit__``.  If ``self`` is already
-            materialized, the context manager may do nothing (reflecting the
-            fact that an outer context manager should already take care of
-            everything else).
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def expanded(self) -> DatasetQueryResults:
-        """Return a `DatasetQueryResults` for which `DataCoordinate.hasRecords`
-        returns `True` for all data IDs in returned `DatasetRef` objects.
-
-        Returns
-        -------
-        expanded : `DatasetQueryResults`
-            Either a new `DatasetQueryResults` instance or ``self``, if it is
-            already expanded.
-
-        Notes
-        -----
-        As with `DataCoordinateQueryResults.expanded`, it may be more efficient
-        to call `materialize` before expanding data IDs for very large result
-        sets.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def count(self, *, exact: bool = True, discard: bool = False) -> int:
-        """Count the number of rows this query would return.
-
-        Parameters
-        ----------
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed to account for that filtering in the count.  If `False`, the
-            result may be an upper bound.
-        discard : `bool`, optional
-            If `True`, compute the exact count even if it would require running
-            the full query and then throwing away the result rows after
-            counting them.  If `False`, this is an error, as the user would
-            usually be better off executing the query first to fetch its rows
-            into a new query (or passing ``exact=False``).  Ignored if
-            ``exact=False``.
-
-        Returns
-        -------
-        count : `int`
-            The number of rows the query would return, or an upper bound if
-            ``exact=False``.
-
-        Notes
-        -----
-        This counts the number of rows returned, not the number of unique rows
-        returned, so even with ``exact=True`` it may provide only an upper
-        bound on the number of *deduplicated* result rows.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def any(self, *, execute: bool = True, exact: bool = True) -> bool:
-        """Test whether this query returns any results.
-
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True`, execute at least a ``LIMIT 1`` query if it cannot be
-            determined prior to execution that the query would return no rows.
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed, until at least one result row is found.  If `False`, the
-            returned result does not account for post-query filtering, and
-            hence may be `True` even when all result rows would be filtered
-            out.
-
-        Returns
-        -------
-        any : `bool`
-            `True` if the query would (or might, depending on arguments) yield
-            result rows.  `False` if it definitely would not.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def explain_no_results(self, execute: bool = True) -> Iterable[str]:
-        """Return human-readable messages that may help explain why the query
-        yields no results.
-
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True` (default) execute simplified versions (e.g. ``LIMIT 1``)
-            of aspects of the tree to more precisely determine where rows were
-            filtered out.
-
-        Returns
-        -------
-        messages : `~collections.abc.Iterable` [ `str` ]
-            String messages that describe reasons the query might not yield any
-            results.
-        """
-        raise NotImplementedError()
-
-
-class SingleTypeDatasetQueryResults(DatasetQueryResults):
-    """An object that represents results from a query for datasets with a
-    single parent `DatasetType`.
+    defaults = Config()
+    defaults["datastore", "cls"] = "lsst.daf.butler.datastores.inMemoryDatastore.InMemoryDatastore"
+    defaults["datastore", "checksum"] = False  # In case of future changes
+    defaults["registry", "db"] = "sqlite:///<butlerRoot>/gen3.sqlite3"
+
+    if config:
+        defaults.update(config)
+
+    if not dataIds:
+        dataIds = {}
+
+    # Disable config root by default so that our registry override will
+    # not be ignored.
+    # newConfig guards against location-related keywords like outfile
+    newConfig = Butler.makeRepo(root, config=defaults, forceConfigRoot=False, **kwargs)
+    butler = Butler.from_config(newConfig, writeable=True)
+    dimensionRecords = _makeRecords(dataIds, butler.dimensions)
+    for dimension, records in dimensionRecords.items():
+        if butler.dimensions[dimension].has_own_table:
+            butler.registry.insertDimensionData(dimension, *records)
+    return butler
+
+
+def makeTestCollection(repo: Butler, uniqueId: str | None = None) -> Butler:
+    """Create a read/write Butler to a fresh collection.
+
+    Parameters
+    ----------
+    repo : `lsst.daf.butler.Butler`
+        A previously existing Butler to a repository, such as that returned by
+        `~lsst.daf.butler.Butler.makeRepo` or `makeTestRepo`.
+    uniqueId : `str`, optional
+        A collection ID guaranteed by external code to be unique across all
+        calls to ``makeTestCollection`` for the same repository.
+
+    Returns
+    -------
+    butler : `lsst.daf.butler.Butler`
+        A Butler referring to a new collection in the repository at ``root``.
+        The collection is (almost) guaranteed to be new.
+
+    Notes
+    -----
+    This function creates a single run collection that does not necessarily
+    conform to any repository conventions. It is only suitable for creating an
+    isolated test area, and not for repositories intended for real data
+    processing or analysis.
     """
-
-    @abstractmethod
-    def materialize(self) -> AbstractContextManager[SingleTypeDatasetQueryResults]:
-        # Docstring inherited from DatasetQueryResults.
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def dataset_type(self) -> DatasetType:
-        """The parent dataset type for all datasets in this iterable
-        (`DatasetType`).
-        """
-        raise NotImplementedError()
-
-    @property
-    @abstractmethod
-    def data_ids(self) -> DataCoordinateQueryResults:
-        """A lazy-evaluation object representing a query for just the data
-        IDs of the datasets that would be returned by this query
-        (`DataCoordinateQueryResults`).
-
-        The returned object is not in general `zip`-iterable with ``self``;
-        it may be in a different order or have (or not have) duplicates.
-        """
-        raise NotImplementedError()
-
-    def expanded(self) -> SingleTypeDatasetQueryResults:
-        # Docstring inherited from DatasetQueryResults.
-        raise NotImplementedError()
-
-
-class DimensionRecordQueryResults(Iterable[DimensionRecord]):
-    """An interface for objects that represent the results of queries for
-    dimension records.
+    if not uniqueId:
+        # Create a "random" collection name
+        # Speed matters more than cryptographic guarantees
+        uniqueId = str(random.randrange(1_000_000_000))
+    collection = "test_" + uniqueId
+    return Butler.from_config(butler=repo, run=collection)
+
+
+def _makeRecords(dataIds: Mapping[str, Iterable], universe: DimensionUniverse) -> Mapping[str, Iterable]:
+    """Create cross-linked dimension records from a collection of
+    data ID values.
+
+    Parameters
+    ----------
+    dataIds : `~collections.abc.Mapping` [`str`, `iterable`]
+        A mapping keyed by the dimensions of interest. Each value is an
+        iterable of names for that dimension (e.g., detector IDs for
+        `"detector"`).
+    universe : lsst.daf.butler.DimensionUniverse
+        Set of all known dimensions and their relationships.
+
+    Returns
+    -------
+    dataIds : `~collections.abc.Mapping` [`str`, `iterable`]
+        A mapping keyed by the dimensions of interest, giving one
+        `~lsst.daf.butler.DimensionRecord` for each input name. Related
+        dimensions (e.g., instruments and detectors) are linked arbitrarily.
     """
+    # Create values for all dimensions that are (recursive) required or implied
+    # dependencies of the given ones.
+    complete_data_id_values = {}
+    for dimension_name in universe.conform(dataIds.keys()).names:
+        if dimension_name in dataIds:
+            complete_data_id_values[dimension_name] = list(dataIds[dimension_name])
+        if dimension_name not in complete_data_id_values:
+            complete_data_id_values[dimension_name] = [
+                _makeRandomDataIdValue(universe.dimensions[dimension_name])
+            ]
+
+    # Start populating dicts that will become DimensionRecords by providing
+    # alternate keys like detector names
+    record_dicts_by_dimension_name: dict[str, list[dict[str, str | int | bytes]]] = {}
+    for name, values in complete_data_id_values.items():
+        record_dicts_by_dimension_name[name] = []
+        dimension_el = universe[name]
+        for value in values:
+            # _fillAllKeys wants Dimension and not DimensionElement.
+            # universe.__getitem__ says it returns DimensionElement but this
+            # really does also seem to be a Dimension here.
+            record_dicts_by_dimension_name[name].append(
+                _fillAllKeys(dimension_el, value)  # type: ignore[arg-type]
+            )
+
+    # Pick cross-relationships arbitrarily
+    for name, record_dicts in record_dicts_by_dimension_name.items():
+        dimension_el = universe[name]
+        for record_dict in record_dicts:
+            for other in dimension_el.dimensions:
+                if other != dimension_el:
+                    relation = record_dicts_by_dimension_name[other.name][0]
+                    record_dict[other.name] = relation[other.primaryKey.name]
+
+    return {
+        dimension: [universe[dimension].RecordClass(**record_dict) for record_dict in record_dicts]
+        for dimension, record_dicts in record_dicts_by_dimension_name.items()
+    }
+
+
+def _fillAllKeys(dimension: Dimension, value: str | int) -> dict[str, str | int | bytes]:
+    """Create an arbitrary mapping of all required keys for a given dimension
+    that do not refer to other dimensions.
+
+    Parameters
+    ----------
+    dimension : `lsst.daf.butler.Dimension`
+        The dimension for which to generate a set of keys (e.g., detector).
+    value
+        The value assigned to ``dimension`` (e.g., detector ID).
+
+    Returns
+    -------
+    expandedValue : `dict` [`str`]
+        A mapping of dimension keys to values. ``dimension's`` primary key
+        maps to ``value``, but all other mappings (e.g., detector name)
+        are arbitrary.
+    """
+    expandedValue: dict[str, str | int | bytes] = {}
+    for key in dimension.uniqueKeys:
+        if key.nbytes:
+            # For `bytes` fields, we want something that casts at least `str`
+            # and `int` values to bytes and yields b'' when called with no
+            # arguments (as in the except block below).  Unfortunately, the
+            # `bytes` type itself fails for both `str` and `int`, but this
+            # lambda does what we need.  This particularly important for the
+            # skymap dimensions' bytes 'hash' field, which has a unique
+            # constraint; without this, all skymaps would get a hash of b''
+            # and end up conflicting.
+            castType = lambda *args: str(*args).encode()  # noqa: E731
+        else:
+            castType = key.dtype().python_type
+        try:
+            castValue = castType(value)
+        except TypeError:
+            castValue = castType()
+        expandedValue[key.name] = castValue
+    for key in dimension.metadata:
+        if not key.nullable:
+            expandedValue[key.name] = key.dtype().python_type(value)
+    return expandedValue
+
+
+def _makeRandomDataIdValue(dimension: Dimension) -> int | str:
+    """Generate a random value of the appropriate type for a data ID key.
+
+    Parameters
+    ----------
+    dimension : `Dimension`
+        Dimension the value corresponds to.
+
+    Returns
+    -------
+    value : `int` or `str`
+        Random value.
+    """
+    if dimension.primaryKey.getPythonType() is str:
+        return str(random.randrange(1000))
+    else:
+        return random.randrange(1000)
+
+
+def expandUniqueId(butler: Butler, partialId: Mapping[str, Any]) -> DataCoordinate:
+    """Return a complete data ID matching some criterion.
+
+    Parameters
+    ----------
+    butler : `lsst.daf.butler.Butler`
+        The repository to query.
+    partialId : `~collections.abc.Mapping` [`str`]
+        A mapping of known dimensions and values.
+
+    Returns
+    -------
+    dataId : `lsst.daf.butler.DataCoordinate`
+        The unique data ID that matches ``partialId``.
+
+    Raises
+    ------
+    ValueError
+        Raised if ``partialId`` does not uniquely identify a data ID.
+
+    Notes
+    -----
+    This method will only work correctly if all dimensions attached to the
+    target dimension (eg., "physical_filter" for "visit") are known to the
+    repository, even if they're not needed to identify a dataset. This function
+    is only suitable for certain kinds of test repositories, and not for
+    repositories intended for real data processing or analysis.
+
+    Examples
+    --------
+    .. code-block:: py
+
+       >>> butler = makeTestRepo(
+               "testdir", {"instrument": ["notACam"], "detector": [1]})
+       >>> expandUniqueId(butler, {"detector": 1})
+       DataCoordinate({instrument, detector}, ('notACam', 1))
+    """
+    # The example is *not* a doctest because it requires dangerous I/O
+    registry = butler.registry
+    dimensions = registry.dimensions.conform(partialId.keys()).required
+
+    query = " AND ".join(f"{dimension} = {value!r}" for dimension, value in partialId.items())
+
+    # Much of the purpose of this function is to do something we explicitly
+    # reject most of the time: query for a governor dimension (e.g. instrument)
+    # given something that depends on it (e.g. visit), hence check=False.
+    dataId = list(registry.queryDataIds(dimensions, where=query, check=False))
+    if len(dataId) == 1:
+        return dataId[0]
+    else:
+        raise ValueError(f"Found {len(dataId)} matches for {partialId}, expected 1.")
+
+
+def _findOrInventDataIdValue(
+    butler: Butler, data_id: dict[str, str | int], dimension: Dimension
+) -> tuple[str | int, bool]:
+    """Look up an arbitrary value for a dimension that is consistent with a
+    partial data ID that does not specify that dimension, or invent one if no
+    such value exists.
+
+    Parameters
+    ----------
+    butler : `Butler`
+        Butler to use to look up data ID values.
+    data_id : `dict` [ `str`, `str` or `int` ]
+        Dictionary of possibly-related data ID values.
+    dimension : `Dimension`
+        Dimension to obtain a value for.
+
+    Returns
+    -------
+    value : `int` or `str`
+        Value for this dimension.
+    invented : `bool`
+        `True` if the value had to be invented, `False` if a compatible value
+        already existed.
+    """
+    # No values given by caller for this dimension.  See if any exist
+    # in the registry that are consistent with the values of dimensions
+    # we do have:
+    match_data_id = {key: data_id[key] for key in data_id.keys() & dimension.dimensions.names}
+    matches = list(butler.registry.queryDimensionRecords(dimension, dataId=match_data_id).limit(1))
+    if not matches:
+        # Nothing in the registry matches: invent a data ID value
+        # with the right type (actual value does not matter).
+        # We may or may not actually make a record with this; that's
+        # easier to check later.
+        dimension_value = _makeRandomDataIdValue(dimension)
+        return dimension_value, True
+    else:
+        # A record does exist in the registry.  Use its data ID value.
+        dim_value = matches[0].dataId[dimension.name]
+        assert dim_value is not None
+        return dim_value, False
+
+
+def _makeDimensionRecordDict(data_id: dict[str, str | int], dimension: Dimension) -> dict[str, Any]:
+    """Create a dictionary that can be used to build a `DimensionRecord` that
+    is consistent with the given data ID.
+
+    Parameters
+    ----------
+    data_id : `dict` [ `str`, `str` or `int` ]
+        Dictionary that contains values for at least all of
+        ``dimension.dimensions.names`` (the main dimension, its recursive
+        required dependencies, and its non-recursive implied dependencies).
+    dimension : `Dimension`
+        Dimension to build a record dictionary for.
+
+    Returns
+    -------
+    record_dict : `dict` [ `str`, `object` ]
+        Dictionary that can be passed as ``**kwargs`` to this dimensions
+        record class constructor.
+    """
+    # Add the primary key field for this dimension.
+    record_dict: dict[str, Any] = {dimension.primaryKey.name: data_id[dimension.name]}
+    # Define secondary keys (e.g., detector name given detector id)
+    record_dict.update(_fillAllKeys(dimension, data_id[dimension.name]))
+    # Set the foreign key values for any related dimensions that should
+    # appear in the record.
+    for related_dimension in dimension.dimensions:
+        if related_dimension.name != dimension.name:
+            record_dict[related_dimension.name] = data_id[related_dimension.name]
+    return record_dict
+
+
+def addDataIdValue(butler: Butler, dimension: str, value: str | int, **related: str | int) -> None:
+    """Add the records that back a new data ID to a repository.
+
+    Parameters
+    ----------
+    butler : `lsst.daf.butler.Butler`
+        The repository to update.
+    dimension : `str`
+        The name of the dimension to gain a new value.
+    value : `str` or `int`
+        The value to register for the dimension.
+    **related : `typing.Any`
+        Any existing dimensions to be linked to ``value``.
+
+    Notes
+    -----
+    Related dimensions (e.g., the instrument associated with a detector) may be
+    specified using ``related``, which requires a value for those dimensions to
+    have been added to the repository already (generally with a previous call
+    to `addDataIdValue`.  Any dependencies of the given dimension that are not
+    included in ``related`` will be linked to existing values arbitrarily, and
+    (for implied dependencies only) created and also inserted into the registry
+    if they do not exist.  Values for required dimensions and those given in
+    ``related`` are never created.
+
+    Because this function creates filler data, it is only suitable for test
+    repositories. It should not be used for repositories intended for real data
+    processing or analysis, which have known dimension values.
+
+    Examples
+    --------
+    See the guide on :ref:`using-butler-in-tests-make-repo` for usage examples.
+    """
+    # Example is not doctest, because it's probably unsafe to create even an
+    # in-memory butler in that environment.
+    try:
+        full_dimension = butler.dimensions[dimension]
+    except KeyError as e:
+        raise ValueError from e
+    # Bad keys ignored by registry code
+    extra_keys = related.keys() - full_dimension.minimal_group.names
+    if extra_keys:
+        raise ValueError(
+            f"Unexpected keywords {extra_keys} not found in {full_dimension.minimal_group.names}"
+        )
+
+    # Assemble a dictionary data ID holding the given primary dimension value
+    # and all of the related ones.
+    data_id: dict[str, int | str] = {dimension: value}
+    data_id.update(related)
+
+    # Compute the set of all dimensions that these recursively depend on.
+    all_dimensions = butler.dimensions.conform(data_id.keys())
+
+    # Create dicts that will become DimensionRecords for all of these data IDs.
+    # This iteration is guaranteed to be in topological order, so we can count
+    # on new data ID values being invented before they are needed.
+    record_dicts_by_dimension: dict[Dimension, dict[str, Any]] = {}
+    for dimension_name in all_dimensions.names:
+        dimension_obj = butler.dimensions.dimensions[dimension_name]
+        dimension_value = data_id.get(dimension_name)
+        if dimension_value is None:
+            data_id[dimension_name], invented = _findOrInventDataIdValue(butler, data_id, dimension_obj)
+            if not invented:
+                # No need to make a new record; one already exists.
+                continue
+        if dimension_name in related:
+            # Caller passed in a value of this dimension explicitly, but it
+            # isn't the primary dimension they asked to have a record created
+            # for.  That means they expect this record to already exist.
+            continue
+        if dimension_name != dimension and dimension_name in all_dimensions.required:
+            # We also don't want to automatically create new dimension records
+            # for required dimensions (except for the main dimension the caller
+            # asked for); those are also asserted by the caller to already
+            # exist.
+            continue
+        if not dimension_obj.has_own_table:
+            # Don't need to bother generating full records for dimensions whose
+            # records are not actually stored.
+            continue
+        record_dicts_by_dimension[dimension_obj] = _makeDimensionRecordDict(data_id, dimension_obj)
+
+    # Sync those dimension record dictionaries with the database.
+    for dimension_obj, record_dict in record_dicts_by_dimension.items():
+        record = dimension_obj.RecordClass(**record_dict)
+        try:
+            butler.registry.syncDimensionData(dimension_obj, record)
+        except sqlalchemy.exc.IntegrityError as e:
+            raise RuntimeError(
+                "Could not create data ID value. Automatic relationship generation "
+                "may have failed; try adding keywords to assign a specific instrument, "
+                "physical_filter, etc. based on the nested exception message."
+            ) from e
+
+
+def addDatasetType(butler: Butler, name: str, dimensions: set[str], storageClass: str) -> DatasetType:
+    """Add a new dataset type to a repository.
+
+    Parameters
+    ----------
+    butler : `lsst.daf.butler.Butler`
+        The repository to update.
+    name : `str`
+        The name of the dataset type.
+    dimensions : `set` [`str`]
+        The dimensions of the new dataset type.
+    storageClass : `str`
+        The storage class the dataset will use.
+
+    Returns
+    -------
+    datasetType : `lsst.daf.butler.DatasetType`
+        The new type.
+
+    Raises
+    ------
+    ValueError
+        Raised if the dimensions or storage class is invalid.
+
+    Notes
+    -----
+    Dataset types are shared across all collections in a repository, so this
+    function does not need to be run for each collection.
+    """
+    try:
+        datasetType = DatasetType(name, dimensions, storageClass, universe=butler.dimensions)
+        butler.registry.registerDatasetType(datasetType)
+        return datasetType
+    except KeyError as e:
+        raise ValueError from e
 
-    @property
-    @abstractmethod
-    def element(self) -> DimensionElement:
-        """Dimension element for this result (`DimensionElement`)."""
-        raise NotImplementedError()
-
-    @abstractmethod
-    def run(self) -> DimensionRecordQueryResults:
-        """Execute the query and return an instance with data held in memory.
-
-        Returns
-        -------
-        result : `DimensionRecordQueryResults`
-            Query results, may return ``self`` if it has all data in memory
-            already.
-        """
-        raise NotImplementedError()
-
-    @abstractmethod
-    def count(self, *, exact: bool = True, discard: bool = False) -> int:
-        """Count the number of rows this query would return.
 
-        Parameters
-        ----------
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed to account for that filtering in the count.  If `False`, the
-            result may be an upper bound.
-        discard : `bool`, optional
-            If `True`, compute the exact count even if it would require running
-            the full query and then throwing away the result rows after
-            counting them.  If `False`, this is an error, as the user would
-            usually be better off executing the query first to fetch its rows
-            into a new query (or passing ``exact=False``).  Ignored if
-            ``exact=False``.
-
-        Returns
-        -------
-        count : `int`
-            The number of rows the query would return, or an upper bound if
-            ``exact=False``.
-
-        Notes
-        -----
-        This counts the number of rows returned, not the number of unique rows
-        returned, so even with ``exact=True`` it may provide only an upper
-        bound on the number of *deduplicated* result rows.
-        """
-        raise NotImplementedError()
+class DatastoreMock:
+    """Mocks a butler datastore.
+
+    Has functions that mock the datastore in a butler. Provides an `apply`
+    function to replace the relevent butler datastore functions with the mock
+    functions.
+    """
 
-    @abstractmethod
-    def any(self, *, execute: bool = True, exact: bool = True) -> bool:
-        """Test whether this query returns any results.
+    @staticmethod
+    def apply(butler: Butler) -> None:
+        """Apply datastore mocks to a butler.
 
         Parameters
         ----------
-        execute : `bool`, optional
-            If `True`, execute at least a ``LIMIT 1`` query if it cannot be
-            determined prior to execution that the query would return no rows.
-        exact : `bool`, optional
-            If `True`, run the full query and perform post-query filtering if
-            needed, until at least one result row is found.  If `False`, the
-            returned result does not account for post-query filtering, and
-            hence may be `True` even when all result rows would be filtered
-            out.
-
-        Returns
-        -------
-        any : `bool`
-            `True` if the query would (or might, depending on arguments) yield
-            result rows.  `False` if it definitely would not.
+        butler : `~lsst.daf.butler.Butler`
+            Butler to be modified.
         """
-        raise NotImplementedError()
+        butler._datastore.export = DatastoreMock._mock_export  # type: ignore
+        butler._datastore.get = DatastoreMock._mock_get  # type: ignore
+        butler._datastore.ingest = MagicMock()  # type: ignore
 
-    @abstractmethod
-    def order_by(self, *args: str) -> DimensionRecordQueryResults:
-        """Make the iterator return ordered result.
+    @staticmethod
+    def _mock_export(
+        refs: Iterable[DatasetRef], *, directory: str | None = None, transfer: str | None = None
+    ) -> Iterable[FileDataset]:
+        """Mock of `Datastore.export` that satisfies the requirement that
+        the refs passed in are included in the `FileDataset` objects
+        returned.
 
-        Parameters
-        ----------
-        *args : `str`
-            Names of the columns/dimensions to use for ordering. Column name
-            can be prefixed with minus (``-``) to use descending ordering.
-
-        Returns
-        -------
-        result : `DimensionRecordQueryResults`
-            Returns ``self`` instance which is updated to return ordered
-            result.
-
-        Notes
-        -----
-        This method can modify the iterator in place and return the same
-        instance.
-        """
-        raise NotImplementedError()
+        This can be used to construct a `Datastore` mock that can be used
+        in repository export via::
 
-    @abstractmethod
-    def limit(self, limit: int | None = None, offset: int = 0) -> DimensionRecordQueryResults:
-        """Make the iterator return limited number of records.
+            datastore = unittest.mock.Mock(spec=Datastore)
+            datastore.export = DatastoreMock._mock_export
 
-        Parameters
-        ----------
-        limit : `int` or `None`, optional
-            Upper limit on the number of returned records.
-        offset : `int`, optional
-            The number of records to skip before returning at most ``limit``
-            records.
-
-        Returns
-        -------
-        result : `DimensionRecordQueryResults`
-            Returns ``self`` instance which is updated to return limited set of
-            records.
-
-        Notes
-        -----
-        This method can modify the iterator in place and return the same
-        instance. Normally this method is used together with `order_by` method.
         """
-        raise NotImplementedError()
+        for ref in refs:
+            yield FileDataset(
+                refs=[ref], path="mock/path", formatter="lsst.daf.butler.formatters.json.JsonFormatter"
+            )
 
-    @abstractmethod
-    def explain_no_results(self, execute: bool = True) -> Iterable[str]:
-        """Return human-readable messages that may help explain why the query
-        yields no results.
-
-        Parameters
-        ----------
-        execute : `bool`, optional
-            If `True` (default) execute simplified versions (e.g. ``LIMIT 1``)
-            of aspects of the tree to more precisely determine where rows were
-            filtered out.
-
-        Returns
-        -------
-        messages : `~collections.abc.Iterable` [ `str` ]
-            String messages that describe reasons the query might not yield any
-            results.
+    @staticmethod
+    def _mock_get(
+        ref: DatasetRef,
+        parameters: Mapping[str, Any] | None = None,
+        storageClass: StorageClass | str | None = None,
+    ) -> tuple[DatasetId, Mapping[str, Any] | None]:
+        """Mock of `Datastore.get` that just returns the integer dataset ID
+        value and parameters it was given.
         """
-        raise NotImplementedError()
+        return (ref.id, parameters)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_registry_shim.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_registry_shim.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_storage_class.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_storage_class_delegate.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_storage_class_delegate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_timespan.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_timespan.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,44 +22,38 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-__all__ = (
-    "SerializedTimespan",
-    "Timespan",
-)
+__all__ = ("Timespan",)
 
 import enum
 import warnings
 from collections.abc import Generator
-from typing import TYPE_CHECKING, Annotated, Any, ClassVar, Union
+from typing import Any, ClassVar, TypeAlias
 
 import astropy.time
 import astropy.utils.exceptions
+import pydantic
 import yaml
-from pydantic import Field
 
 # As of astropy 4.2, the erfa interface is shipped independently and
 # ErfaWarning is no longer an AstropyWarning
 try:
     import erfa
 except ImportError:
     erfa = None
 
 from lsst.utils.classes import cached_getter
 
-from .json import from_json_generic, to_json_generic
 from .time_utils import TimeConverter
 
-if TYPE_CHECKING:  # Imports needed only for type annotations; may be circular.
-    from .dimensions import DimensionUniverse
-    from .registry import Registry
+_ONE_DAY = astropy.time.TimeDelta("1d", scale="tai")
 
 
 class _SpecialTimespanBound(enum.Enum):
     """Enumeration to provide a singleton value for empty timespan bounds.
 
     This enum's only member should generally be accessed via the
     `Timespan.EMPTY` alias.
@@ -67,23 +61,18 @@
 
     EMPTY = enum.auto()
     """The value used for both `Timespan.begin` and `Timespan.end` for empty
     Timespans that contain no points.
     """
 
 
-TimespanBound = Union[astropy.time.Time, _SpecialTimespanBound, None]
+TimespanBound: TypeAlias = astropy.time.Time | _SpecialTimespanBound | None
 
-SerializedTimespan = Annotated[list[int], Field(min_length=2, max_length=2)]
-"""JSON-serializable representation of the Timespan class, as a list of two
-integers ``[begin, end]`` in nanoseconds since the epoch.
-"""
 
-
-class Timespan:
+class Timespan(pydantic.BaseModel):
     """A half-open time interval with nanosecond precision.
 
     Parameters
     ----------
     begin : `astropy.time.Time`, `Timespan.EMPTY`, or `None`
         Minimum timestamp in the interval (inclusive).  `None` indicates that
         the timespan has no lower bound.  `Timespan.EMPTY` indicates that the
@@ -189,22 +178,30 @@
                         )
             _nsec = (begin_nsec, end_nsec)
         if _nsec[0] >= _nsec[1]:
             # Standardizing all empty timespans to the same underlying values
             # here simplifies all other operations (including interactions
             # with TimespanDatabaseRepresentation implementations).
             _nsec = (converter.max_nsec, converter.min_nsec)
-        self._nsec = _nsec
+        super().__init__(nsec=_nsec)
+
+    nsec: tuple[int, int] = pydantic.Field(frozen=True)
 
-    __slots__ = ("_nsec", "_cached_begin", "_cached_end")
+    model_config = pydantic.ConfigDict(
+        json_schema_extra={
+            "description": (
+                "A [begin, end) TAI timespan with bounds as integer nanoseconds since 1970-01-01 00:00:00."
+            )
+        }
+    )
 
     EMPTY: ClassVar[_SpecialTimespanBound] = _SpecialTimespanBound.EMPTY
 
     # YAML tag name for Timespan
-    yaml_tag = "!lsst.daf.butler.Timespan"
+    yaml_tag: ClassVar[str] = "!lsst.daf.butler.Timespan"
 
     @classmethod
     def makeEmpty(cls) -> Timespan:
         """Construct an empty timespan.
 
         Returns
         -------
@@ -239,49 +236,86 @@
         nsec = converter.astropy_to_nsec(time)
         if nsec == converter.max_nsec - 1:
             raise ValueError(
                 f"Cannot construct near-instantaneous timespan at {time}; within one ns of maximum time."
             )
         return Timespan(None, None, _nsec=(nsec, nsec + 1))
 
+    @classmethod
+    def from_day_obs(cls, day_obs: int, offset: int = 0) -> Timespan:
+        """Construct a timespan for a 24-hour period based on the day of
+        observation.
+
+        Parameters
+        ----------
+        day_obs : `int`
+            The day of observation as an integer of the form YYYYMMDD.
+            The year must be at least 1970 since these are converted to TAI.
+        offset : `int`, optional
+            Offset in seconds from TAI midnight to be applied.
+
+        Returns
+        -------
+        day_span : `Timespan`
+            A timespan corresponding to a full day of observing.
+
+        Notes
+        -----
+        If the observing day is 20240229 and the offset is 12 hours the
+        resulting time span will be 2024-02-29T12:00 to 2024-03-01T12:00.
+        """
+        if day_obs < 1970_00_00 or day_obs > 1_0000_00_00:
+            raise ValueError(f"day_obs must be in form yyyyMMDD and be newer than 1970, not {day_obs}.")
+
+        ymd = str(day_obs)
+        t1 = astropy.time.Time(f"{ymd[0:4]}-{ymd[4:6]}-{ymd[6:8]}T00:00:00", format="isot", scale="tai")
+
+        if offset != 0:
+            t_delta = astropy.time.TimeDelta(offset, format="sec", scale="tai")
+            t1 += t_delta
+
+        t2 = t1 + _ONE_DAY
+
+        return Timespan(t1, t2)
+
     @property
     @cached_getter
     def begin(self) -> TimespanBound:
         """Minimum timestamp in the interval, inclusive.
 
         If this bound is finite, this is an `astropy.time.Time` instance.
         If the timespan is unbounded from below, this is `None`.
         If the timespan is empty, this is the special value `Timespan.EMPTY`.
         """
         if self.isEmpty():
             return self.EMPTY
-        elif self._nsec[0] == TimeConverter().min_nsec:
+        elif self.nsec[0] == TimeConverter().min_nsec:
             return None
         else:
-            return TimeConverter().nsec_to_astropy(self._nsec[0])
+            return TimeConverter().nsec_to_astropy(self.nsec[0])
 
     @property
     @cached_getter
     def end(self) -> TimespanBound:
         """Maximum timestamp in the interval, exclusive.
 
         If this bound is finite, this is an `astropy.time.Time` instance.
         If the timespan is unbounded from above, this is `None`.
         If the timespan is empty, this is the special value `Timespan.EMPTY`.
         """
         if self.isEmpty():
             return self.EMPTY
-        elif self._nsec[1] == TimeConverter().max_nsec:
+        elif self.nsec[1] == TimeConverter().max_nsec:
             return None
         else:
-            return TimeConverter().nsec_to_astropy(self._nsec[1])
+            return TimeConverter().nsec_to_astropy(self.nsec[1])
 
     def isEmpty(self) -> bool:
         """Test whether ``self`` is the empty timespan (`bool`)."""
-        return self._nsec[0] >= self._nsec[1]
+        return self.nsec[0] >= self.nsec[1]
 
     def __str__(self) -> str:
         if self.isEmpty():
             return "(empty)"
         fmt = "%Y-%m-%dT%H:%M:%S"
         # Trap dubious year warnings in case we have timespans from
         # simulated data in the future
@@ -312,23 +346,23 @@
         return f"Timespan(begin={begin}, end={end})"
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Timespan):
             return False
         # Correctness of this simple implementation depends on __init__
         # standardizing all empty timespans to a single value.
-        return self._nsec == other._nsec
+        return self.nsec == other.nsec
 
     def __hash__(self) -> int:
         # Correctness of this simple implementation depends on __init__
         # standardizing all empty timespans to a single value.
-        return hash(self._nsec)
+        return hash(self.nsec)
 
     def __reduce__(self) -> tuple:
-        return (Timespan, (None, None, False, self._nsec))
+        return (Timespan, (None, None, False, self.nsec))
 
     def __lt__(self, other: astropy.time.Time | Timespan) -> bool:
         """Test if a Timespan's bounds are strictly less than the given time.
 
         Parameters
         ----------
         other : `Timespan` or `astropy.time.Time`.
@@ -345,17 +379,17 @@
         # the second uses a strict inequality to make sure inf == inf isn't in
         # play, and it's okay for the second to use a strict inequality only
         # because we know non-empty Timespans have nonzero duration, and hence
         # the second term is never false for non-empty timespans unless the
         # first term is also false.
         if isinstance(other, astropy.time.Time):
             nsec = TimeConverter().astropy_to_nsec(other)
-            return self._nsec[1] <= nsec and self._nsec[0] < nsec
+            return self.nsec[1] <= nsec and self.nsec[0] < nsec
         else:
-            return self._nsec[1] <= other._nsec[0] and self._nsec[0] < other._nsec[1]
+            return self.nsec[1] <= other.nsec[0] and self.nsec[0] < other.nsec[1]
 
     def __gt__(self, other: astropy.time.Time | Timespan) -> bool:
         """Test if a Timespan's bounds are strictly greater than given time.
 
         Parameters
         ----------
         other : `Timespan` or `astropy.time.Time`.
@@ -372,17 +406,17 @@
         # the second uses a strict inequality to make sure inf == inf isn't in
         # play, and it's okay for the second to use a strict inequality only
         # because we know non-empty Timespans have nonzero duration, and hence
         # the second term is never false for non-empty timespans unless the
         # first term is also false.
         if isinstance(other, astropy.time.Time):
             nsec = TimeConverter().astropy_to_nsec(other)
-            return self._nsec[0] > nsec and self._nsec[1] > nsec
+            return self.nsec[0] > nsec and self.nsec[1] > nsec
         else:
-            return self._nsec[0] >= other._nsec[1] and self._nsec[1] > other._nsec[0]
+            return self.nsec[0] >= other.nsec[1] and self.nsec[1] > other.nsec[0]
 
     def overlaps(self, other: Timespan | astropy.time.Time) -> bool:
         """Test if the intersection of this Timespan with another is empty.
 
         Parameters
         ----------
         other : `Timespan` or `astropy.time.Time`
@@ -398,15 +432,15 @@
         -----
         If either ``self`` or ``other`` is empty, the result is always `False`.
         In all other cases, ``self.contains(other)`` being `True` implies that
         ``self.overlaps(other)`` is also `True`.
         """
         if isinstance(other, astropy.time.Time):
             return self.contains(other)
-        return self._nsec[1] > other._nsec[0] and other._nsec[1] > self._nsec[0]
+        return self.nsec[1] > other.nsec[0] and other.nsec[1] > self.nsec[0]
 
     def contains(self, other: astropy.time.Time | Timespan) -> bool:
         """Test if the supplied timespan is within this one.
 
         Tests whether the intersection of this timespan with another timespan
         or point is equal to the other one.
 
@@ -431,17 +465,17 @@
         `Timespan.fromInstant`, because Timespan cannot exactly represent
         zero-duration intervals.  In particular, ``[a, b)`` contains the time
         ``b``, but not the timespan ``[b, b + 1ns)`` that would be returned
         by `Timespan.fromInstant(b)``.
         """
         if isinstance(other, astropy.time.Time):
             nsec = TimeConverter().astropy_to_nsec(other)
-            return self._nsec[0] <= nsec and self._nsec[1] > nsec
+            return self.nsec[0] <= nsec and self.nsec[1] > nsec
         else:
-            return self._nsec[0] <= other._nsec[0] and self._nsec[1] >= other._nsec[1]
+            return self.nsec[0] <= other.nsec[0] and self.nsec[1] >= other.nsec[1]
 
     def intersection(self, *args: Timespan) -> Timespan:
         """Return a new `Timespan` that is contained by all of the given ones.
 
         Parameters
         ----------
         *args
@@ -450,18 +484,18 @@
         Returns
         -------
         intersection : `Timespan`
             The intersection timespan.
         """
         if not args:
             return self
-        lowers = [self._nsec[0]]
-        lowers.extend(ts._nsec[0] for ts in args)
-        uppers = [self._nsec[1]]
-        uppers.extend(ts._nsec[1] for ts in args)
+        lowers = [self.nsec[0]]
+        lowers.extend(ts.nsec[0] for ts in args)
+        uppers = [self.nsec[1]]
+        uppers.extend(ts.nsec[1] for ts in args)
         nsec = (max(*lowers), min(*uppers))
         return Timespan(begin=None, end=None, _nsec=nsec)
 
     def difference(self, other: Timespan) -> Generator[Timespan, None, None]:
         """Return the one or two timespans that cover the interval(s).
 
         The interval is defined as one that is in ``self`` but not ``other``.
@@ -483,67 +517,18 @@
         """
         intersection = self.intersection(other)
         if intersection.isEmpty():
             yield self
         elif intersection == self:
             yield from ()
         else:
-            if intersection._nsec[0] > self._nsec[0]:
-                yield Timespan(None, None, _nsec=(self._nsec[0], intersection._nsec[0]))
-            if intersection._nsec[1] < self._nsec[1]:
-                yield Timespan(None, None, _nsec=(intersection._nsec[1], self._nsec[1]))
-
-    def to_simple(self, minimal: bool = False) -> SerializedTimespan:
-        """Return simple python type form suitable for serialization.
-
-        Parameters
-        ----------
-        minimal : `bool`, optional
-            Use minimal serialization. Has no effect on for this class.
-
-        Returns
-        -------
-        simple : `list` of `int`
-            The internal span as integer nanoseconds.
-        """
-        # Return the internal nanosecond form rather than astropy ISO string
-        return list(self._nsec)
-
-    @classmethod
-    def from_simple(
-        cls,
-        simple: SerializedTimespan | None,
-        universe: DimensionUniverse | None = None,
-        registry: Registry | None = None,
-    ) -> Timespan | None:
-        """Construct a new object from simplified form.
-
-        Designed to use the data returned from the `to_simple` method.
-
-        Parameters
-        ----------
-        simple : `list` of `int`, or `None`
-            The values returned by `to_simple()`.
-        universe : `DimensionUniverse`, optional
-            Unused.
-        registry : `lsst.daf.butler.Registry`, optional
-            Unused.
-
-        Returns
-        -------
-        result : `Timespan` or `None`
-            Newly-constructed object.
-        """
-        if simple is None:
-            return None
-        nsec1, nsec2 = simple  # for mypy
-        return cls(begin=None, end=None, _nsec=(nsec1, nsec2))
-
-    to_json = to_json_generic
-    from_json: ClassVar = classmethod(from_json_generic)
+            if intersection.nsec[0] > self.nsec[0]:
+                yield Timespan(None, None, _nsec=(self.nsec[0], intersection.nsec[0]))
+            if intersection.nsec[1] < self.nsec[1]:
+                yield Timespan(None, None, _nsec=(intersection.nsec[1], self.nsec[1]))
 
     @classmethod
     def to_yaml(cls, dumper: yaml.Dumper, timespan: Timespan) -> Any:
         """Convert Timespan into YAML format.
 
         This produces a scalar node with a tag "!_SpecialTimespanBound" and
         value being a name of _SpecialTimespanBound enum.
@@ -583,14 +568,27 @@
             return None
         elif node.value == "EMPTY":
             return Timespan.makeEmpty()
         else:
             d = loader.construct_mapping(node)
             return Timespan(d["begin"], d["end"])
 
+    @pydantic.model_validator(mode="before")
+    @classmethod
+    def _validate(cls, value: Any) -> Any:
+        if isinstance(value, Timespan):
+            return value
+        if isinstance(value, dict):
+            return value
+        return {"nsec": value}
+
+    @pydantic.model_serializer(mode="plain")
+    def _serialize(self) -> tuple[int, int]:
+        return self.nsec
+
 
 # Register Timespan -> YAML conversion method with Dumper class
 yaml.Dumper.add_representer(Timespan, Timespan.to_yaml)
 
 # Register YAML -> Timespan conversion method with Loader, for our use case we
 # only need SafeLoader.
 yaml.SafeLoader.add_constructor(Timespan.yaml_tag, Timespan.from_yaml)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_topology.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_topology.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,14 +102,17 @@
 
     def __hash__(self) -> int:
         return hash(self.name)
 
     def __contains__(self, other: TopologicalRelationshipEndpoint) -> bool:
         return other.topology.get(self.space) == self
 
+    def __repr__(self) -> str:
+        return self.name
+
     @abstractmethod
     def choose(self, endpoints: Set[str], universe: DimensionUniverse) -> TopologicalRelationshipEndpoint:
         """Select the best member of this family to use.
 
         These are to be used in a query join or data ID when more than one
         is present.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/locked_object.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/locked_object.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/named_locks.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/named_locks.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/_utilities/thread_safe_cache.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_utilities/thread_safe_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/arrow_utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/arrow_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -299,17 +299,17 @@
         return self._nullable
 
     @property
     def data_type(self) -> pa.DataType:
         # Docstring inherited.
         return UUIDArrowType()
 
-    def append(self, value: uuid.UUID, column: list[bytes]) -> None:
+    def append(self, value: uuid.UUID | None, column: list[bytes | None]) -> None:
         # Docstring inherited.
-        column.append(value.bytes)
+        column.append(value.bytes if value is not None else None)
 
     def finish(self, column: list[Any]) -> pa.Array:
         # Docstring inherited.
         storage_array = pa.array(column, self.storage_type)
         return pa.ExtensionArray.from_storage(UUIDArrowType(), storage_array)
 
 
@@ -336,17 +336,17 @@
         return self._nullable
 
     @property
     def data_type(self) -> pa.DataType:
         # Docstring inherited.
         return RegionArrowType()
 
-    def append(self, value: Region, column: list[bytes]) -> None:
+    def append(self, value: Region | None, column: list[bytes | None]) -> None:
         # Docstring inherited.
-        column.append(value.encode())
+        column.append(value.encode() if value is not None else None)
 
     def finish(self, column: list[Any]) -> pa.Array:
         # Docstring inherited.
         storage_array = pa.array(column, self.storage_type)
         return pa.ExtensionArray.from_storage(RegionArrowType(), storage_array)
 
 
@@ -378,17 +378,17 @@
         return self._nullable
 
     @property
     def data_type(self) -> pa.DataType:
         # Docstring inherited.
         return TimespanArrowType()
 
-    def append(self, value: Timespan, column: list[pa.StructScalar]) -> None:
+    def append(self, value: Timespan | None, column: list[pa.StructScalar | None]) -> None:
         # Docstring inherited.
-        column.append({"begin_nsec": value._nsec[0], "end_nsec": value._nsec[1]})
+        column.append({"begin_nsec": value.nsec[0], "end_nsec": value.nsec[1]} if value is not None else None)
 
     def finish(self, column: list[Any]) -> pa.Array:
         # Docstring inherited.
         storage_array = pa.array(column, self.storage_type)
         return pa.ExtensionArray.from_storage(TimespanArrowType(), storage_array)
 
 
@@ -415,17 +415,17 @@
         return self._nullable
 
     @property
     def data_type(self) -> pa.DataType:
         # Docstring inherited.
         return DateTimeArrowType()
 
-    def append(self, value: astropy.time.Time, column: list[int]) -> None:
+    def append(self, value: astropy.time.Time | None, column: list[int | None]) -> None:
         # Docstring inherited.
-        column.append(TimeConverter().astropy_to_nsec(value))
+        column.append(TimeConverter().astropy_to_nsec(value) if value is not None else None)
 
     def finish(self, column: list[Any]) -> pa.Array:
         # Docstring inherited.
         storage_array = pa.array(column, self.storage_type)
         return pa.ExtensionArray.from_storage(DateTimeArrowType(), storage_array)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/butler.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/butler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cliLog.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cliLog.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_collections.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/_remove_collections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/_remove_runs.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/_remove_runs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/cmd/commands.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/cmd/commands.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/arguments.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/arguments.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/optionGroups.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/optionGroups.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/opt/options.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/opt/options.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/progress.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/progress.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/cli/utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
     was done with the CliLog interface.
 
     lsst.log modules can not be set back to an uninitialized state (python
     logging modules can be set back to NOTSET), instead they are set to
     `CliLog.defaultLsstLogLevel`.
     """
 
-    def invoke(self, *args: Any, **kwargs: Any) -> Any:
+    def invoke(self, *args: Any, **kwargs: Any) -> click.testing.Result:
         result = super().invoke(*args, **kwargs)
         CliLog.resetLog()
         return result
 
 
 def clickResultMsg(result: click.testing.Result) -> str:
     """Get a standard assert message from a click result.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/column_spec.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/column_spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,62 +34,76 @@
     "HashColumnSpec",
     "FloatColumnSpec",
     "BoolColumnSpec",
     "UUIDColumnSpec",
     "RegionColumnSpec",
     "TimespanColumnSpec",
     "ColumnType",
+    "COLLECTION_NAME_MAX_LENGTH",
 )
 
 import textwrap
 import uuid
 from abc import ABC, abstractmethod
 from typing import Annotated, Any, ClassVar, Literal, TypeAlias, Union, final
 
 import astropy.time
 import pyarrow as pa
 import pydantic
 from lsst.sphgeom import Region
 
 from . import arrow_utils, ddl
 from ._timespan import Timespan
+from .name_shrinker import NameShrinker
 
 ColumnType: TypeAlias = Literal[
     "int", "string", "hash", "float", "datetime", "bool", "uuid", "timespan", "region"
 ]
 
 
+COLLECTION_NAME_MAX_LENGTH = 64
+# TODO: DM-42541 would bee a good opportunity to move this constant to a
+# better home; this file is the least-bad home I can think of for now.  Note
+# that actually changing the value is a (minor) schema change.
+
+
 class _BaseColumnSpec(pydantic.BaseModel, ABC):
     """Base class for descriptions of table columns."""
 
     name: str = pydantic.Field(description="""Name of the column.""")
 
     doc: str = pydantic.Field(default="", description="Documentation for the column.")
 
     type: ColumnType
 
     nullable: bool = pydantic.Field(
         default=True,
         description="Whether the column may be ``NULL``.",
     )
 
-    def to_sql_spec(self, **kwargs: Any) -> ddl.FieldSpec:
+    def to_sql_spec(self, name_shrinker: NameShrinker | None = None, **kwargs: Any) -> ddl.FieldSpec:
         """Convert this specification to a SQL-specific one.
 
         Parameters
         ----------
+        name_shrinker : `NameShrinker`, optional
+            Object that should be used to shrink the field name to ensure it
+            fits within database-specific limits.
         **kwargs
             Forwarded to `ddl.FieldSpec`.
 
         Returns
         -------
         sql_spec : `ddl.FieldSpec`
             A SQL-specific version of this specification.
         """
-        return ddl.FieldSpec(name=self.name, dtype=ddl.VALID_CONFIG_COLUMN_TYPES[self.type], **kwargs)
+        name = self.name
+        if name_shrinker is not None:
+            name = name_shrinker.shrink(name)
+        return ddl.FieldSpec(name=name, dtype=ddl.VALID_CONFIG_COLUMN_TYPES[self.type], **kwargs)
 
     @abstractmethod
     def to_arrow(self) -> arrow_utils.ToArrow:
         """Return an object that converts values of this column to a column in
         an Arrow table.
 
         Returns
@@ -151,17 +165,17 @@
     pytype: ClassVar[type] = str
 
     type: Literal["string"] = "string"
 
     length: int
     """Maximum length of strings."""
 
-    def to_sql_spec(self, **kwargs: Any) -> ddl.FieldSpec:
+    def to_sql_spec(self, name_shrinker: NameShrinker | None = None, **kwargs: Any) -> ddl.FieldSpec:
         # Docstring inherited.
-        return super().to_sql_spec(length=self.length, **kwargs)
+        return super().to_sql_spec(length=self.length, name_shrinker=name_shrinker, **kwargs)
 
     def to_arrow(self) -> arrow_utils.ToArrow:
         # Docstring inherited.
         return arrow_utils.ToArrow.for_primitive(self.name, pa.string(), nullable=self.nullable)
 
 
 @final
@@ -171,17 +185,17 @@
     pytype: ClassVar[type] = bytes
 
     type: Literal["hash"] = "hash"
 
     nbytes: int
     """Number of bytes for the hash."""
 
-    def to_sql_spec(self, **kwargs: Any) -> ddl.FieldSpec:
+    def to_sql_spec(self, name_shrinker: NameShrinker | None = None, **kwargs: Any) -> ddl.FieldSpec:
         # Docstring inherited.
-        return super().to_sql_spec(nbytes=self.nbytes, **kwargs)
+        return super().to_sql_spec(nbytes=self.nbytes, name_shrinker=name_shrinker, **kwargs)
 
     def to_arrow(self) -> arrow_utils.ToArrow:
         # Docstring inherited.
         return arrow_utils.ToArrow.for_primitive(
             self.name,
             # The size for Arrow binary columns is a fixed size, not a maximum
             # as in SQL, so we use a variable-size column.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/composites.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/composites.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/fileDatastore.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/formatters.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/formatters.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 Defects: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 IsrCalib: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 QECurve: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 CrosstalkCalib: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 PhotonTransferCurveDataset: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 Linearizer: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 BrighterFatterKernel: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
+MatchingKernel: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 FiberSpectrum: lsst.obs.base.formatters.fitsGeneric.FitsGenericFormatter
 Image: lsst.obs.base.formatters.fitsExposure.FitsImageFormatter
 ImageF: lsst.obs.base.formatters.fitsExposure.FitsImageFormatter
 ImageU: lsst.obs.base.formatters.fitsExposure.FitsImageFormatter
 DecoratedImageU: lsst.obs.base.formatters.fitsExposure.FitsExposureFormatter
 Mask: lsst.obs.base.formatters.fitsExposure.FitsMaskFormatter
 MaskX: lsst.obs.base.formatters.fitsExposure.FitsMaskFormatter
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/datastores/writeRecipes.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/dimensions.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/registry.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/registry.yaml`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/configs/storageClasses.yaml` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/configs/storageClasses.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -244,21 +244,23 @@
   QECurve:
     pytype: lsst.meas.algorithms.Curve
   CrosstalkCalib:
     pytype: lsst.ip.isr.CrosstalkCalib
   Linearizer:
     pytype: lsst.ip.isr.Linearizer
   FiberSpectrum:
-    pytype: lsst.obs.fiberSpectrograph.FiberSpectrum
+    pytype: lsst.obs.fiberspectrograph.FiberSpectrum
   PhotonTransferCurveDataset:
     pytype: lsst.ip.isr.PhotonTransferCurveDataset
   StrayLightData:
     pytype: lsst.ip.isr.StrayLightData
   BrighterFatterKernel:
     pytype: lsst.ip.isr.BrighterFatterKernel
+  MatchingKernel:
+    ptype: lsst.afw.math.Kernel
   FilterLabel:
     pytype: lsst.afw.image.FilterLabel
   Exposure:
     pytype: lsst.afw.image.Exposure
     delegate: lsst.obs.base.exposureAssembler.ExposureAssembler
     parameters:
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/_datastore.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/_datastore.py`

 * *Files 1% similar despite different names*

```diff
@@ -949,18 +949,18 @@
         missing_refs = []
         for ref in refs:
             try:
                 uris[ref] = self.getURIs(ref, predict=predict)
             except FileNotFoundError:
                 missing_refs.append(ref)
         if missing_refs and not allow_missing:
+            num_missing = len(missing_refs)
             raise FileNotFoundError(
-                "Missing {} refs from datastore out of {} and predict=False.".format(
-                    num_missing := len(missing_refs), num_missing + len(uris)
-                )
+                f"Missing {num_missing} refs from datastore out of "
+                f"{num_missing + len(uris)} and predict=False."
             )
         return uris
 
     @abstractmethod
     def getURIs(self, datasetRef: DatasetRef, predict: bool = False) -> DatasetRefURIs:
         """Return URIs associated with dataset.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/cache_manager.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/cache_manager.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/composites.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/composites.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/constraints.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/constraints.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/file_templates.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/file_templates.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/generic_base.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/generic_base.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/record_data.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/record_data.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastore/stored_file_info.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastore/stored_file_info.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/chainedDatastore.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/chainedDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastore.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/fileDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/fileDatastoreClient.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/fileDatastoreClient.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/get.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/get.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/file_datastore/retrieve_artifacts.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/datastores/inMemoryDatastore.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/datastores/inMemoryDatastore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/ddl.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/ddl.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowastropy.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrowastropy.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpy.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrownumpy.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrownumpydict.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrownumpydict.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/arrowtable.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/arrowtable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/delegates/dataframe.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/delegates/dataframe.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_config.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_coordinate.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_coordinate.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,14 +48,15 @@
 from typing import TYPE_CHECKING, Any, ClassVar, cast
 
 import pydantic
 from deprecated.sphinx import deprecated
 from lsst.sphgeom import IntersectionRegion, Region
 from lsst.utils.introspection import find_outside_stacklevel
 
+from .._exceptions import DimensionNameError
 from .._named import NamedKeyMapping, NamedValueAbstractSet, NameLookupMapping
 from .._timespan import Timespan
 from ..json import from_json_pydantic, to_json_pydantic
 from ..persistence_context import PersistenceContextVars
 from ._elements import Dimension, DimensionElement
 from ._graph import DimensionGraph
 from ._group import DimensionGroup
@@ -162,15 +163,15 @@
     attribute).
 
     See also :ref:`lsst.daf.butler-dimensions_data_ids`
     """
 
     __slots__ = ()
 
-    _serializedType = SerializedDataCoordinate
+    _serializedType: ClassVar[type[pydantic.BaseModel]] = SerializedDataCoordinate
 
     @staticmethod
     def standardize(
         mapping: NameLookupMapping[Dimension, DataIdValue] | None = None,
         *,
         dimensions: Iterable[str] | DimensionGroup | DimensionGraph | None = None,
         graph: DimensionGraph | None = None,
@@ -214,15 +215,15 @@
         coordinate : `DataCoordinate`
             A validated `DataCoordinate` instance.
 
         Raises
         ------
         TypeError
             Raised if the set of optional arguments provided is not supported.
-        KeyError
+        DimensionNameError
             Raised if a key-value pair for a required dimension is missing.
         """
         universe = (
             universe
             or getattr(dimensions, "universe", None)
             or getattr(graph, "universe", None)
             or getattr(mapping, "universe", None)
@@ -290,15 +291,17 @@
             return DataCoordinate.from_full_values(
                 dimensions, tuple(new_mapping[name] for name in dimensions.data_coordinate_keys)
             )
         else:
             try:
                 values = tuple(new_mapping[name] for name in dimensions.required)
             except KeyError as err:
-                raise KeyError(f"No value in data ID ({mapping}) for required dimension {err}.") from err
+                raise DimensionNameError(
+                    f"No value in data ID ({mapping}) for required dimension {err}."
+                ) from err
             return DataCoordinate.from_required_values(dimensions, values)
 
     @property
     @abstractmethod
     def mapping(self) -> Mapping[str, DataIdValue]:
         """A mapping view of the data ID with keys for all dimensions it has
         values for.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_data_coordinate_iterable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_database.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_database.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_elements.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_elements.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_governor.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_governor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_graph.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
     contexts where a collection of dimensions is required and a
     `DimensionUniverse` is available.  Exceptions include cases where order
     matters (and is different from the consistent ordering defined by the
     `DimensionUniverse`), or complete `~collection.abc.Set` semantics are
     required.
     """
 
-    _serializedType = SerializedDimensionGraph
+    _serializedType: ClassVar[type[pydantic.BaseModel]] = SerializedDimensionGraph
 
     def __new__(
         cls,
         universe: DimensionUniverse,
         dimensions: Iterable[Dimension] | None = None,
         names: Iterable[str] | None = None,
         conform: bool = True,
@@ -491,15 +491,15 @@
         is_superset : `bool`
             Returns `True` if ``other`` is empty.
         """
         return self._group >= other.as_group()
 
     def __eq__(self, other: Any) -> bool:
         """Test the arguments have exactly the same dimensions & elements."""
-        if isinstance(other, (DimensionGraph, DimensionGroup)):
+        if isinstance(other, DimensionGraph | DimensionGroup):
             return self._group == other.as_group()
         return False
 
     def __hash__(self) -> int:
         return hash(self.as_group())
 
     def __le__(self, other: DimensionGroup | DimensionGraph) -> bool:
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_group.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,15 @@
         """
         return self.names >= other.names
 
     def __eq__(self, other: Any) -> bool:
         from ._graph import DimensionGraph
 
         # TODO: Drop DimensionGraph support here on DM-41326.
-        if isinstance(other, (DimensionGroup, DimensionGraph)):
+        if isinstance(other, DimensionGroup | DimensionGraph):
             return self.names == other.names
         else:
             return False
 
     def __hash__(self) -> int:
         return hash(self.required._seq)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_packer.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_packer.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_set.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_record_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,14 +173,21 @@
         if not isinstance(other, DimensionRecordSet):
             return False
         return (
             self._record_type is other._record_type
             and self._by_required_values.keys() == other._by_required_values.keys()
         )
 
+    def __repr__(self) -> str:
+        lines = [f"DimensionRecordSet({self.element.name}, {{"]
+        for record in self:
+            lines.append(f"    {record!r},")
+        lines.append("})")
+        return "\n".join(lines)
+
     def issubset(self, other: DimensionRecordSet) -> bool:
         """Test whether all elements in ``self`` are in ``other``.
 
         Parameters
         ----------
         other : `DimensionRecordSet`
             Another record set with the same record type.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_record_table.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_record_table.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_records.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_records.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = ("DimensionRecord", "SerializedDimensionRecord")
 
 from collections.abc import Hashable
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Tuple
+from typing import TYPE_CHECKING, Any, ClassVar
 
 import lsst.sphgeom
 from lsst.utils.classes import immutable
 from pydantic import BaseModel, Field, StrictBool, StrictFloat, StrictInt, StrictStr, create_model
 
 from .._timespan import Timespan
 from ..json import from_json_pydantic, to_json_pydantic
@@ -101,24 +101,27 @@
         int: StrictInt,
     }
 
     for field in fields.standard:
         field_type = field.getPythonType()
         field_type = type_map.get(field_type, field_type)
         if field.nullable:
-            field_type = Optional[field_type]  # type: ignore
+            field_type = field_type | None  # type: ignore
         members[field.name] = (field_type, ...)
     if definition.temporal:
-        members["timespan"] = (Optional[Tuple[int, int]], ...)  # type: ignore
+        members["timespan"] = (Timespan | None, ...)  # type: ignore
     if definition.spatial:
         members["region"] = (str, ...)
 
-    # mypy does not seem to like create_model
+    # For the new derived class name need to convert to camel case.
+    # so "day_obs" -> "DayObs".
+    derived_name = "".join([part.capitalize() for part in definition.name.split("_")])
+
     model = create_model(
-        f"SpecificSerializedDimensionRecord{definition.name.capitalize()}",
+        f"SpecificSerializedDimensionRecord{derived_name}",
         __base__=SpecificSerializedDimensionRecord,
         **members,  # type: ignore
     )
 
     _SIMPLE_RECORD_CLASS_CACHE[cache_key] = model
     return model
 
@@ -147,15 +150,15 @@
     definition: str = Field(
         ...,
         title="Name of dimension associated with this record.",
         examples=["exposure"],
     )
 
     # Use strict types to prevent casting
-    record: dict[str, None | StrictBool | StrictInt | StrictFloat | StrictStr | tuple[int, int]] = Field(
+    record: dict[str, None | StrictBool | StrictInt | StrictFloat | StrictStr | Timespan] = Field(
         ...,
         title="Dimension record keys and values.",
         examples=[
             {
                 "definition": "exposure",
                 "record": {
                     "instrument": "LATISS",
@@ -171,15 +174,15 @@
     }
 
     @classmethod
     def direct(
         cls,
         *,
         definition: str,
-        record: dict[str, None | StrictFloat | StrictStr | StrictBool | StrictInt | tuple[int, int]],
+        record: dict[str, Any],
     ) -> SerializedDimensionRecord:
         """Construct a `SerializedDimensionRecord` directly without validators.
 
         Parameters
         ----------
         definition : `str`
             The name of the record.
@@ -197,17 +200,20 @@
         are explicitly what the model requires, and it will recurse through
         members, constructing them from their corresponding `direct` methods.
 
         This method should only be called when the inputs are trusted.
         """
         # This method requires tuples as values of the mapping, but JSON
         # readers will read things in as lists. Be kind and transparently
-        # transform to tuples
+        # transform to tuples.
         _recItems = {
-            k: v if type(v) != list else tuple(v) for k, v in record.items()  # type: ignore # noqa: E721
+            k: (
+                v if type(v) is not list else Timespan(begin=None, end=None, _nsec=tuple(v))  # noqa: E721
+            )  # type: ignore
+            for k, v in record.items()
         }
 
         # Type ignore because the ternary statement seems to confuse mypy
         # based on conflicting inferred types of v.
         key = (
             definition,
             frozenset(_recItems.items()),
@@ -258,15 +264,15 @@
     """
 
     # Derived classes are required to define __slots__ as well, and it's those
     # derived-class slots that other methods on the base class expect to see
     # when they access self.__slots__.
     __slots__ = ("dataId",)
 
-    _serializedType = SerializedDimensionRecord
+    _serializedType: ClassVar[type[BaseModel]] = SerializedDimensionRecord
 
     def __init__(self, **kwargs: Any):
         # Accept either the dimension name or the actual name of its primary
         # key field; ensure both are present in the dict for convenience below.
         if isinstance(self.definition, Dimension):
             v = kwargs.get(self.definition.primaryKey.name)
             if v is None:
@@ -367,29 +373,25 @@
         # For now do not implement minimal form.
         key = (id(self.definition), self.dataId)
         cache = PersistenceContextVars.serializedDimensionRecordMapping.get()
         if cache is not None and (result := cache.get(key)) is not None:
             return result
 
         mapping = {name: getattr(self, name) for name in self.__slots__}
-        # If the item in mapping supports simplification update it
         for k, v in mapping.items():
-            try:
-                mapping[k] = v.to_simple(minimal=minimal)
-            except AttributeError:
-                if isinstance(v, lsst.sphgeom.Region):
-                    # YAML serialization specifies the class when it
-                    # doesn't have to. This is partly for explicitness
-                    # and also history. Here use a different approach.
-                    # This code needs to be migrated to sphgeom
-                    mapping[k] = v.encode().hex()
-                if isinstance(v, bytes):
-                    # We actually can't handle serializing out to bytes for
-                    # hash objects, encode it here to a hex string
-                    mapping[k] = v.hex()
+            if isinstance(v, lsst.sphgeom.Region):
+                # YAML serialization specifies the class when it
+                # doesn't have to. This is partly for explicitness
+                # and also history. Here use a different approach.
+                # This code needs to be migrated to sphgeom
+                mapping[k] = v.encode().hex()
+            if isinstance(v, bytes):
+                # We actually can't handle serializing out to bytes for
+                # hash objects, encode it here to a hex string
+                mapping[k] = v.hex()
         definition = self.definition.to_simple(minimal=minimal)
         dimRec = SerializedDimensionRecord(definition=definition, record=mapping)
         if cache is not None:
             cache[key] = dimRec
         return dimRec
 
     @classmethod
@@ -447,27 +449,27 @@
         # Create a specialist subclass model with type validation.
         # This allows us to do simple checks of external data (possibly
         # sent as JSON) since for now _reconstructDimensionRecord does not
         # do any validation.
         record_model_cls = _createSimpleRecordSubclass(definition)
         record_model = record_model_cls(**simple.record)
 
-        # Timespan and region have to be converted to native form
-        # for now assume that those keys are special
-        rec = record_model.model_dump()
-
-        if (ts := "timespan") in rec:
-            rec[ts] = Timespan.from_simple(rec[ts], universe=universe, registry=registry)
-        if (reg := "region") in rec:
-            encoded = bytes.fromhex(rec[reg])
-            rec[reg] = lsst.sphgeom.Region.decode(encoded)
-        if (hsh := "hash") in rec:
-            rec[hsh] = bytes.fromhex(rec[hsh].decode())
+        # Region and hash have to be converted to native form; for now assume
+        # that the keys are special.  We make the mapping we need to pass to
+        # the DimensionRecord constructor via getattr, because we don't
+        # model_dump re-disassembling things like Timespans that we've already
+        # assembled.
+        mapping = {k: getattr(record_model, k) for k in definition.schema.names}
+
+        if "region" in mapping:
+            mapping["region"] = lsst.sphgeom.Region.decode(bytes.fromhex(mapping["region"]))
+        if "hash" in mapping:
+            mapping["hash"] = bytes.fromhex(mapping["hash"].decode())
 
-        dimRec = _reconstructDimensionRecord(definition, rec)
+        dimRec = _reconstructDimensionRecord(definition, mapping)
         if cache is not None:
             cache[key] = dimRec
         return dimRec
 
     to_json = to_json_pydantic
     from_json: ClassVar = classmethod(from_json_pydantic)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_schema.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_skypix.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_skypix.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/_universe.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/_universe.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/construction.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/construction.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/dimensions/record_cache.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/dimensions/record_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/direct_butler.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_butler/_direct_butler.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,68 +39,61 @@
 import io
 import itertools
 import logging
 import numbers
 import os
 import warnings
 from collections import Counter, defaultdict
-from collections.abc import Iterable, Iterator, Mapping, MutableMapping, Sequence
+from collections.abc import Iterable, Iterator, MutableMapping, Sequence
 from typing import TYPE_CHECKING, Any, ClassVar, TextIO, cast
 
 from lsst.resources import ResourcePath, ResourcePathExpression
 from lsst.utils.introspection import get_class_of
-from lsst.utils.iteration import ensure_iterable
 from lsst.utils.logging import VERBOSE, getLogger
 from sqlalchemy.exc import IntegrityError
 
-from ._butler import Butler
-from ._butler_config import ButlerConfig
-from ._butler_instance_options import ButlerInstanceOptions
-from ._dataset_existence import DatasetExistence
-from ._dataset_ref import DatasetRef
-from ._dataset_type import DatasetType
-from ._deferredDatasetHandle import DeferredDatasetHandle
-from ._exceptions import EmptyQueryResultError, ValidationError
-from ._limited_butler import LimitedButler
-from ._registry_shim import RegistryShim
-from ._storage_class import StorageClass, StorageClassFactory
-from ._timespan import Timespan
-from .datastore import Datastore, NullDatastore
-from .dimensions import DataCoordinate, Dimension
-from .direct_query import DirectQuery
-from .progress import Progress
-from .registry import (
+from .._butler import Butler
+from .._butler_config import ButlerConfig
+from .._butler_instance_options import ButlerInstanceOptions
+from .._dataset_existence import DatasetExistence
+from .._dataset_ref import DatasetRef
+from .._dataset_type import DatasetType
+from .._deferredDatasetHandle import DeferredDatasetHandle
+from .._exceptions import DatasetNotFoundError, DimensionValueError, ValidationError
+from .._limited_butler import LimitedButler
+from .._registry_shim import RegistryShim
+from .._storage_class import StorageClass, StorageClassFactory
+from .._timespan import Timespan
+from ..datastore import Datastore, NullDatastore
+from ..dimensions import DataCoordinate, Dimension
+from ..direct_query_driver import DirectQueryDriver
+from ..progress import Progress
+from ..queries import Query
+from ..registry import (
     CollectionType,
     ConflictingDefinitionError,
     DataIdError,
     MissingDatasetTypeError,
     RegistryDefaults,
     _RegistryFactory,
 )
-from .registry.sql_registry import SqlRegistry
-from .transfers import RepoExportContext
-from .utils import transactional
+from ..registry.sql_registry import SqlRegistry
+from ..transfers import RepoExportContext
+from ..utils import transactional
+from ._direct_butler_collections import DirectButlerCollections
 
 if TYPE_CHECKING:
     from lsst.resources import ResourceHandleProtocol
 
-    from ._dataset_ref import DatasetId
-    from ._file_dataset import FileDataset
-    from ._query import Query
-    from .datastore import DatasetRefURIs
-    from .dimensions import (
-        DataId,
-        DataIdValue,
-        DimensionElement,
-        DimensionGroup,
-        DimensionRecord,
-        DimensionUniverse,
-    )
-    from .registry import CollectionArgType, Registry
-    from .transfers import RepoImportBackend
+    from .._dataset_ref import DatasetId
+    from .._file_dataset import FileDataset
+    from ..datastore import DatasetRefURIs
+    from ..dimensions import DataId, DataIdValue, DimensionElement, DimensionRecord, DimensionUniverse
+    from ..registry import Registry
+    from ..transfers import RepoImportBackend
 
 _LOG = getLogger(__name__)
 
 
 class ButlerValidationError(ValidationError):
     """There is a problem with the Butler configuration."""
 
@@ -307,16 +300,17 @@
                 self.run,
                 dict(self._registry.defaults.dataId.required),
                 self._registry.isWriteable(),
             ),
         )
 
     def __str__(self) -> str:
-        return "Butler(collections={}, run={}, datastore='{}', registry='{}')".format(
-            self.collections, self.run, self._datastore, self._registry
+        return (
+            f"Butler(collections={self.collections}, run={self.run}, "
+            f"datastore='{self._datastore}', registry='{self._registry}')"
         )
 
     def isWriteable(self) -> bool:
         # Docstring inherited.
         return self._registry.isWriteable()
 
     def _caching_context(self) -> contextlib.AbstractContextManager[None]:
@@ -600,15 +594,15 @@
                         assigned[field].add(dimensionName)
                         matched_dims.add(field)
 
             # Calculate the fields that matched nothing.
             never_found = set(not_dimensions) - matched_dims
 
             if never_found:
-                raise ValueError(f"Unrecognized keyword args given: {never_found}")
+                raise DimensionValueError(f"Unrecognized keyword args given: {never_found}")
 
             # There is a chance we have allocated a single dataId item
             # to multiple dimensions. Need to decide which should be retained.
             # For now assume that the most popular alternative wins.
             # This means that day_obs with seq_num will result in
             # exposure.day_obs and not visit.day_obs
             # Also prefer an explicitly missing dimension over an inferred
@@ -673,26 +667,26 @@
                         newDataId[dimensionName],
                         str(values),
                     )
                     # Get the actual record and compare with these values.
                     try:
                         recs = list(self._registry.queryDimensionRecords(dimensionName, dataId=newDataId))
                     except DataIdError:
-                        raise ValueError(
+                        raise DimensionValueError(
                             f"Could not find dimension '{dimensionName}'"
                             f" with dataId {newDataId} as part of comparing with"
                             f" record values {byRecord[dimensionName]}"
                         ) from None
                     if len(recs) == 1:
                         errmsg: list[str] = []
                         for k, v in values.items():
                             if (recval := getattr(recs[0], k)) != v:
                                 errmsg.append(f"{k}({recval} != {v})")
                         if errmsg:
-                            raise ValueError(
+                            raise DimensionValueError(
                                 f"Dimension {dimensionName} in dataId has explicit value"
                                 " inconsistent with records: " + ", ".join(errmsg)
                             )
                     else:
                         # Multiple matches for an explicit dimension
                         # should never happen but let downstream complain.
                         pass
@@ -754,21 +748,21 @@
                         # The ambiguity may have been resolved so check again.
                         if len(records) > 1:
                             _LOG.debug(
                                 "Received %d records from constraints of %s", len(records), str(values)
                             )
                             for r in records:
                                 _LOG.debug("- %s", str(r))
-                            raise ValueError(
+                            raise DimensionValueError(
                                 f"DataId specification for dimension {dimensionName} is not"
                                 f" uniquely constrained to a single dataset by {values}."
                                 f" Got {len(records)} results."
                             )
                     else:
-                        raise ValueError(
+                        raise DimensionValueError(
                             f"DataId specification for dimension {dimensionName} matched no"
                             f" records when constrained by {values}"
                         )
 
                 # Get the primary key from the real dimension object
                 dimension = self.dimensions.dimensions[dimensionName]
                 if not isinstance(dimension, Dimension):
@@ -784,14 +778,15 @@
         datasetRefOrType: DatasetRef | DatasetType | str,
         dataId: DataId | None = None,
         *,
         collections: Any = None,
         predict: bool = False,
         run: str | None = None,
         datastore_records: bool = False,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> DatasetRef:
         """Shared logic for methods that start with a search for a dataset in
         the registry.
 
         Parameters
         ----------
@@ -811,14 +806,19 @@
             dataset ID if finding a reference in the `Registry` fails.
             Defaults to `False`.
         run : `str`, optional
             Run collection name to use for creating `DatasetRef` for predicted
             datasets. Only used if ``predict`` is `True`.
         datastore_records : `bool`, optional
             If `True` add datastore records to returned `DatasetRef`.
+        timespan : `Timespan` or `None`, optional
+            A timespan that the validity range of the dataset must overlap.
+            If not provided and this is a calibration dataset type, an attempt
+            will be made to find the timespan from any temporal coordinate
+            in the data ID.
         **kwargs
             Additional keyword arguments used to augment or construct a
             `DataId`.  See `DataId` parameters.
 
         Returns
         -------
         ref : `DatasetRef`
@@ -841,30 +841,37 @@
         if isinstance(datasetRefOrType, DatasetRef):
             if collections is not None:
                 warnings.warn("Collections should not be specified with DatasetRef", stacklevel=3)
             # May need to retrieve datastore records if requested.
             if datastore_records and datasetRefOrType._datastore_records is None:
                 datasetRefOrType = self._registry.get_datastore_records(datasetRefOrType)
             return datasetRefOrType
-        timespan: Timespan | None = None
 
         dataId, kwargs = self._rewrite_data_id(dataId, datasetType, **kwargs)
 
         if datasetType.isCalibration():
             # Because this is a calibration dataset, first try to make a
             # standardize the data ID without restricting the dimensions to
             # those of the dataset type requested, because there may be extra
             # dimensions that provide temporal information for a validity-range
             # lookup.
             dataId = DataCoordinate.standardize(
                 dataId, universe=self.dimensions, defaults=self._registry.defaults.dataId, **kwargs
             )
-            if dataId.dimensions.temporal:
-                dataId = self._registry.expandDataId(dataId)
-                timespan = dataId.timespan
+            if timespan is None:
+                if dataId.dimensions.temporal:
+                    dataId = self._registry.expandDataId(dataId)
+                    # Use the timespan from the data ID to constrain the
+                    # calibration lookup, but only if the caller has not
+                    # specified an explicit timespan.
+                    timespan = dataId.timespan
+                else:
+                    # Try an arbitrary timespan. Downstream will fail if this
+                    # results in more than one matching dataset.
+                    timespan = Timespan(None, None)
         else:
             # Standardize the data ID to just the dimensions of the dataset
             # type instead of letting registry.findDataset do it, so we get the
             # result even if no dataset is found.
             dataId = DataCoordinate.standardize(
                 dataId,
                 dimensions=datasetType.dimensions,
@@ -886,15 +893,15 @@
                     run = self.run
                     if run is None:
                         raise TypeError("Cannot predict dataset ID/location with run=None.")
                 return DatasetRef(datasetType, dataId, run=run)
             else:
                 if collections is None:
                     collections = self._registry.defaults.collections
-                raise LookupError(
+                raise DatasetNotFoundError(
                     f"Dataset {datasetType.name} with data ID {dataId} "
                     f"could not be found in collections {collections}."
                 )
         if datasetType != ref.datasetType:
             # If they differ it is because the user explicitly specified
             # a compatible dataset type to this call rather than using the
             # registry definition. The DatasetRef must therefore be recreated
@@ -993,14 +1000,15 @@
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
         parameters: dict | None = None,
         collections: Any = None,
         storageClass: str | StorageClass | None = None,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> DeferredDatasetHandle:
         """Create a `DeferredDatasetHandle` which can later retrieve a dataset,
         after an immediate registry lookup.
 
         Parameters
         ----------
@@ -1020,14 +1028,19 @@
             to butler construction.
         storageClass : `StorageClass` or `str`, optional
             The storage class to be used to override the Python type
             returned by this method. By default the returned type matches
             the dataset type definition for this dataset. Specifying a
             read `StorageClass` can force a different type to be returned.
             This type must be compatible with the original type.
+        timespan : `Timespan` or `None`, optional
+            A timespan that the validity range of the dataset must overlap.
+            If not provided and this is a calibration dataset type, an attempt
+            will be made to find the timespan from any temporal coordinate
+            in the data ID.
         **kwargs
             Additional keyword arguments used to augment or construct a
             `DataId`.  See `DataId` parameters.
 
         Returns
         -------
         obj : `DeferredDatasetHandle`
@@ -1050,26 +1063,29 @@
             # in trust mode where there won't be a record but there will be
             # a file.
             if self._datastore.knows(datasetRefOrType) or self._datastore.exists(datasetRefOrType):
                 ref = datasetRefOrType
             else:
                 raise LookupError(f"Dataset reference {datasetRefOrType} does not exist.")
         else:
-            ref = self._findDatasetRef(datasetRefOrType, dataId, collections=collections, **kwargs)
+            ref = self._findDatasetRef(
+                datasetRefOrType, dataId, collections=collections, timespan=timespan, **kwargs
+            )
         return DeferredDatasetHandle(butler=self, ref=ref, parameters=parameters, storageClass=storageClass)
 
     def get(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
         parameters: dict[str, Any] | None = None,
         collections: Any = None,
         storageClass: StorageClass | str | None = None,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> Any:
         """Retrieve a stored dataset.
 
         Parameters
         ----------
         datasetRefOrType : `DatasetRef`, `DatasetType`, or `str`
@@ -1090,14 +1106,19 @@
             to butler construction.
         storageClass : `StorageClass` or `str`, optional
             The storage class to be used to override the Python type
             returned by this method. By default the returned type matches
             the dataset type definition for this dataset. Specifying a
             read `StorageClass` can force a different type to be returned.
             This type must be compatible with the original type.
+        timespan : `Timespan` or `None`, optional
+            A timespan that the validity range of the dataset must overlap.
+            If not provided and this is a calibration dataset type, an attempt
+            will be made to find the timespan from any temporal coordinate
+            in the data ID.
         **kwargs
             Additional keyword arguments used to augment or construct a
             `DataCoordinate`.  See `DataCoordinate.standardize`
             parameters.
 
         Returns
         -------
@@ -1119,15 +1140,20 @@
         dataset with the appropriate validity range.  For example, a "bias"
         dataset with native dimensions ``{instrument, detector}`` could be
         fetched with a ``{instrument, detector, exposure}`` data ID, because
         ``exposure`` is a temporal dimension.
         """
         _LOG.debug("Butler get: %s, dataId=%s, parameters=%s", datasetRefOrType, dataId, parameters)
         ref = self._findDatasetRef(
-            datasetRefOrType, dataId, collections=collections, datastore_records=True, **kwargs
+            datasetRefOrType,
+            dataId,
+            collections=collections,
+            datastore_records=True,
+            timespan=timespan,
+            **kwargs,
         )
         return self._datastore.get(ref, parameters=parameters, storageClass=storageClass)
 
     def getURIs(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
@@ -1724,15 +1750,16 @@
 
                     if not can_query:
                         raise RuntimeError(
                             f"Transferring populated_by records like {element.name} requires a full Butler."
                         )
 
                     records = source_butler.registry.queryDimensionRecords(  # type: ignore
-                        element.name, **data_id.mapping  # type: ignore
+                        element.name,
+                        **data_id.mapping,  # type: ignore
                     )
                     for record in records:
                         additional_records[record.definition].setdefault(record.dataId, record)
 
         # The next step is to walk back through the additional records to
         # pick up any missing content (such as visit_definition needing to
         # know the exposure). Want to ensure we do not request records we
@@ -2064,14 +2091,19 @@
                 msg += ", ".join(str(k) for k in failed)
                 messages.append(msg)
 
         if messages:
             raise ValidationError(";\n".join(messages))
 
     @property
+    def collection_chains(self) -> DirectButlerCollections:
+        """Object with methods for modifying collection chains."""
+        return DirectButlerCollections(self._registry)
+
+    @property
     def collections(self) -> Sequence[str]:
         """The collections to search by default, in order
         (`~collections.abc.Sequence` [ `str` ]).
 
         This is an alias for ``self.registry.defaults.collections``.  It cannot
         be set directly in isolation, but all defaults may be changed together
         by assigning a new `RegistryDefaults` instance to
@@ -2106,106 +2138,21 @@
     def dimensions(self) -> DimensionUniverse:
         # Docstring inherited.
         return self._registry.dimensions
 
     @contextlib.contextmanager
     def _query(self) -> Iterator[Query]:
         # Docstring inherited.
-        with self._caching_context():
-            yield DirectQuery(self._registry)
-
-    def _query_data_ids(
-        self,
-        dimensions: DimensionGroup | Iterable[str] | str,
-        *,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        expanded: bool = False,
-        order_by: Iterable[str] | str | None = None,
-        limit: int | None = None,
-        offset: int = 0,
-        explain: bool = True,
-        **kwargs: Any,
-    ) -> list[DataCoordinate]:
-        # Docstring inherited.
-        query = DirectQuery(self._registry)
-        result = query.data_ids(dimensions, data_id=data_id, where=where, bind=bind, **kwargs)
-        if expanded:
-            result = result.expanded()
-        if order_by:
-            result = result.order_by(*ensure_iterable(order_by))
-        if limit is not None:
-            result = result.limit(limit, offset)
-        else:
-            if offset:
-                raise TypeError("offset is specified without limit")
-        data_ids = list(result)
-        if explain and not data_ids:
-            raise EmptyQueryResultError(list(result.explain_no_results()))
-        return data_ids
-
-    def _query_datasets(
-        self,
-        dataset_type: Any,
-        collections: CollectionArgType | None = None,
-        *,
-        find_first: bool = True,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        expanded: bool = False,
-        explain: bool = True,
-        **kwargs: Any,
-    ) -> list[DatasetRef]:
-        # Docstring inherited.
-        query = DirectQuery(self._registry)
-        result = query.datasets(
-            dataset_type,
-            collections,
-            find_first=find_first,
-            data_id=data_id,
-            where=where,
-            bind=bind,
-            **kwargs,
+        driver = DirectQueryDriver(
+            self._registry._db, self.dimensions, self._registry._managers, self._registry.defaults
         )
-        if expanded:
-            result = result.expanded()
-        refs = list(result)
-        if explain and not refs:
-            raise EmptyQueryResultError(list(result.explain_no_results()))
-        return refs
-
-    def _query_dimension_records(
-        self,
-        element: str,
-        *,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        order_by: Iterable[str] | str | None = None,
-        limit: int | None = None,
-        offset: int = 0,
-        explain: bool = True,
-        **kwargs: Any,
-    ) -> list[DimensionRecord]:
-        # Docstring inherited.
-        query = DirectQuery(self._registry)
-        result = query.dimension_records(element, data_id=data_id, where=where, bind=bind, **kwargs)
-        if order_by:
-            result = result.order_by(*ensure_iterable(order_by))
-        if limit is not None:
-            result = result.limit(limit, offset)
-        else:
-            if offset:
-                raise TypeError("offset is specified without limit")
-        data_ids = list(result)
-        if explain and not data_ids:
-            raise EmptyQueryResultError(list(result.explain_no_results()))
-        return data_ids
+        query = Query(driver)
+        with self._caching_context():
+            with driver:
+                yield query
 
     def _preload_cache(self) -> None:
         """Immediately load caches that are used for common operations."""
         self._registry.preload_cache()
 
     _config: ButlerConfig
     """Configuration for this Butler instance."""
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/astropyTable.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/astropyTable.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/file.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/file.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/json.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/json.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/logs.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/logs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/matplotlib.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/matplotlib.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/packages.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/packages.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/parquet.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/parquet.py`

 * *Files 1% similar despite different names*

```diff
@@ -283,23 +283,32 @@
         if arrow_table[name].null_count == 0:
             # Regular non-masked column
             col = arrow_table[name].to_numpy()
         else:
             # For a masked column, we need to ask arrow to fill the null
             # values with an appropriately typed value before conversion.
             # Then we apply the mask to get a masked array of the correct type.
-
-            if t in (pa.string(), pa.binary()):
-                dummy = ""
-            else:
-                dummy = t.to_pandas_dtype()(0)
+            null_value: Any
+            match t:
+                case t if t in (pa.float64(), pa.float32(), pa.float16()):
+                    null_value = np.nan
+                case t if t in (pa.int64(), pa.int32(), pa.int16(), pa.int8()):
+                    null_value = -1
+                case t if t in (pa.bool_(),):
+                    null_value = True
+                case t if t in (pa.string(), pa.binary()):
+                    null_value = ""
+                case _:
+                    # This is the fallback for unsigned ints in particular.
+                    null_value = 0
 
             col = np.ma.masked_array(
-                data=arrow_table[name].fill_null(dummy).to_numpy(),
+                data=arrow_table[name].fill_null(null_value).to_numpy(),
                 mask=arrow_table[name].is_null().to_numpy(),
+                fill_value=null_value,
             )
 
         if t in (pa.string(), pa.binary()):
             col = col.astype(_arrow_string_to_numpy_dtype(schema, name, col))
         elif isinstance(t, pa.FixedSizeListType):
             if len(col) > 0:
                 col = np.stack(col)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/pickle.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/pickle.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/formatters/yaml.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/formatters/yaml.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/json.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/json.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,27 +26,29 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = ("to_json_generic", "from_json_generic", "to_json_pydantic", "from_json_pydantic")
 
 import json
-from typing import TYPE_CHECKING, Any, Protocol, Type
+from typing import TYPE_CHECKING, Any, ClassVar, Protocol
+
+from pydantic import BaseModel
 
 if TYPE_CHECKING:
     from .dimensions import DimensionUniverse
     from .registry import Registry
 
 
 class SupportsSimple(Protocol):
     """Protocol defining the methods required to support the standard
     serialization using "simple" methods names.
     """
 
-    _serializedType: Type
+    _serializedType: ClassVar[type[BaseModel]]
 
     def to_simple(self, minimal: bool) -> Any: ...
 
     @classmethod
     def from_simple(
         cls, simple: Any, universe: DimensionUniverse | None = None, registry: Registry | None = None
     ) -> SupportsSimple: ...
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/logging.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/logging.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,23 +21,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 __all__ = ("ButlerMDC", "ButlerLogRecords", "ButlerLogRecordHandler", "ButlerLogRecord", "JsonLogFormatter")
 
 import datetime
 import logging
 import traceback
 from collections.abc import Callable, Generator, Iterable, Iterator
 from contextlib import contextmanager
 from logging import Formatter, LogRecord, StreamHandler
-from typing import IO, Any, ClassVar, Union, overload
+from typing import IO, Any, ClassVar, overload
 
 from lsst.utils.introspection import get_full_type_name
 from lsst.utils.iteration import isplit
 from pydantic import BaseModel, ConfigDict, PrivateAttr, RootModel
 
 _LONG_LOG_FORMAT = "{levelname} {asctime} {name} {filename}:{lineno} - {message}"
 """Default format for log records."""
@@ -196,15 +198,15 @@
     processName: str
     exc_info: str | None = None
     MDC: dict[str, str]
 
     model_config = ConfigDict(frozen=True)
 
     @classmethod
-    def from_record(cls, record: LogRecord) -> "ButlerLogRecord":
+    def from_record(cls, record: LogRecord) -> ButlerLogRecord:
         """Create a new instance from a `~logging.LogRecord`.
 
         Parameters
         ----------
         record : `logging.LogRecord`
             The record from which to extract the relevant information.
         """
@@ -288,26 +290,26 @@
 # being Any even though we wish to constrain them to Record.
 class ButlerLogRecords(_ButlerLogRecords):
     """Class representing a collection of `ButlerLogRecord`."""
 
     _log_format: str | None = PrivateAttr(None)
 
     @classmethod
-    def from_records(cls, records: Iterable[ButlerLogRecord]) -> "ButlerLogRecords":
+    def from_records(cls, records: Iterable[ButlerLogRecord]) -> ButlerLogRecords:
         """Create collection from iterable.
 
         Parameters
         ----------
         records : iterable of `ButlerLogRecord`
             The records to seed this class with.
         """
         return cls.model_construct(root=list(records))
 
     @classmethod
-    def from_file(cls, filename: str) -> "ButlerLogRecords":
+    def from_file(cls, filename: str) -> ButlerLogRecords:
         """Read records from file.
 
         Parameters
         ----------
         filename : `str`
             Name of file containing the JSON records.
 
@@ -370,15 +372,15 @@
                 f" {first_char!r} from {error_type} content starting with {startdata!r}"
             )
 
         # Assume a record per line.
         return False
 
     @classmethod
-    def from_stream(cls, stream: IO) -> "ButlerLogRecords":
+    def from_stream(cls, stream: IO) -> ButlerLogRecords:
         """Read records from I/O stream.
 
         Parameters
         ----------
         stream : `typing.IO`
             Stream from which to read JSON records.
 
@@ -407,15 +409,15 @@
             line = line.rstrip()
             if line:  # Filter out blank lines.
                 records.append(ButlerLogRecord.model_validate_json(line))
 
         return cls.from_records(records)
 
     @classmethod
-    def from_raw(cls, serialized: str | bytes) -> "ButlerLogRecords":
+    def from_raw(cls, serialized: str | bytes) -> ButlerLogRecords:
         """Parse raw serialized form and return records.
 
         Parameters
         ----------
         serialized : `bytes` or `str`
             Either the serialized JSON of the model created using
             ``.model_dump_json()`` or a streaming format of one JSON
@@ -485,17 +487,17 @@
     def __setitem__(self, index: int, value: Record) -> None:
         self.root[index] = self._validate_record(value)
 
     @overload
     def __getitem__(self, index: int) -> ButlerLogRecord: ...
 
     @overload
-    def __getitem__(self, index: slice) -> "ButlerLogRecords": ...
+    def __getitem__(self, index: slice) -> ButlerLogRecords: ...
 
-    def __getitem__(self, index: slice | int) -> "Union[ButlerLogRecords, ButlerLogRecord]":
+    def __getitem__(self, index: slice | int) -> ButlerLogRecords | ButlerLogRecord:
         # Handles slices and returns a new collection in that
         # case.
         item = self.root[index]
         if isinstance(item, list):
             return type(self)(item)
         else:
             return item
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/mapping_factory.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/mapping_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,17 +260,16 @@
         if key in self._registry and not overwrite:
             # Compare the class strings since dynamic classes can be the
             # same thing but be different.
             if str(self._registry[key]) == str(typeName):
                 return
 
             raise KeyError(
-                "Item with key {} already registered with different value ({} != {})".format(
-                    key, self._registry[key], typeName
-                )
+                f"Item with key {key} already registered with different value "
+                f"({self._registry[key]} != {typeName})"
             )
 
         self._registry[key] = {
             "type": typeName,
             "kwargs": dict(**kwargs),
         }
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/nonempty_mapping.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/persistence_context.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/persistence_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/progress.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/progress.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/pydantic_utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/pydantic_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -23,21 +23,25 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
-__all__ = ("DeferredValidation", "get_universe_from_context")
+__all__ = ("DeferredValidation", "get_universe_from_context", "SerializableRegion", "SerializableTime")
 
-from typing import TYPE_CHECKING, Any, ClassVar, Generic, Self, TypeVar, get_args
+from typing import TYPE_CHECKING, Annotated, Any, ClassVar, Generic, Self, TypeAlias, TypeVar, get_args
 
 import pydantic
+from astropy.time import Time
+from lsst.sphgeom import Region
 from pydantic_core import core_schema
 
+from .time_utils import TimeConverter
+
 if TYPE_CHECKING:
     from .dimensions import DimensionUniverse
 
 _T = TypeVar("_T")
 
 
 def get_universe_from_context(context: dict[str, Any] | None) -> DimensionUniverse:
@@ -239,7 +243,74 @@
         cls, _core_schema: core_schema.CoreSchema, handler: pydantic.json_schema.GetJsonSchemaHandler
     ) -> pydantic.json_schema.JsonSchemaValue:
         # This is the Pydantic hook for customizing JSON schema.  We ignore
         # the schema generated for this class, and just return the JSON schema
         # of the wrapped type.
         json_schema = handler(cls._get_wrapped_type_adapter().core_schema)
         return handler.resolve_ref_schema(json_schema)
+
+
+def _deserialize_region(value: object, handler: pydantic.ValidatorFunctionWrapHandler) -> Region:
+    if isinstance(value, Region):
+        return value
+
+    string = handler(value)
+    return Region.decode(bytes.fromhex(string))
+
+
+def _serialize_region(region: Region) -> str:
+    return region.encode().hex()
+
+
+SerializableRegion: TypeAlias = Annotated[
+    Region,
+    pydantic.GetPydanticSchema(lambda _, h: h(str)),
+    pydantic.WrapValidator(_deserialize_region),
+    pydantic.PlainSerializer(_serialize_region),
+    pydantic.WithJsonSchema(
+        {
+            "type": "string",
+            "description": "A region on the sphere from the lsst.sphgeom package.",
+            "media": {"binaryEncoding": "base16", "type": "application/lsst.sphgeom"},
+        }
+    ),
+]
+"""A Pydantic-annotated version of `lsst.sphgeom.Region`.
+
+An object annotated with this type is always an `lsst.sphgeom.Region` instance
+in Python, but unlike `lsst.sphgeom.Region` itself it can be used as a type
+in Pydantic models and type adapters, resulting in the field being saved as
+a hex encoding of the sphgeom-encoded bytes.
+"""
+
+
+def _deserialize_time(value: object, handler: pydantic.ValidatorFunctionWrapHandler) -> Region:
+    if isinstance(value, Time):
+        return value
+
+    integer = handler(value)
+    return TimeConverter().nsec_to_astropy(integer)
+
+
+def _serialize_time(time: Time) -> int:
+    return TimeConverter().astropy_to_nsec(time)
+
+
+SerializableTime: TypeAlias = Annotated[
+    Time,
+    pydantic.GetPydanticSchema(lambda _, h: h(int)),
+    pydantic.WrapValidator(_deserialize_time),
+    pydantic.PlainSerializer(_serialize_time),
+    pydantic.WithJsonSchema(
+        {
+            "type": "integer",
+            "description": "A TAI time represented as integer nanoseconds since 1970-01-01 00:00:00.",
+        }
+    ),
+]
+"""A Pydantic-annotated version of `astropy.time.Time`.
+
+An object annotated with this type is always an `astropy.time.Time` instance
+in Python, but unlike `astropy.time.Time` itself it can be used as a type
+in Pydantic models and type adapters, resulting in the field being saved as
+integer nanoseconds since 1970-01-01 00:00:00.
+"""
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,25 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+# Re-export some top-level exception types for backwards compatibility -- these
+# used to be part of registry.
+from .._exceptions import (
+    CollectionTypeError,
+    DimensionNameError,
+    MissingCollectionError,
+    MissingDatasetTypeError,
+)
+from .._exceptions_legacy import CollectionError, DataIdError, DatasetTypeError, RegistryError
+
+# Registry imports.
 from . import interfaces, managers, queries, wildcards
 from ._collection_summary import *
 from ._collection_type import *
 from ._config import *
 from ._defaults import *
 from ._exceptions import *
 from ._registry import *
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_caching_context.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_caching_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_record_cache.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_record_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,32 +75,30 @@
         # In case we replace same record name with different key, find the
         # existing record and drop its key.
         if (old_record := self._by_name.get(record.name)) is not None:
             self._by_key.pop(old_record.key)
         if (old_record := self._by_key.get(record.key)) is not None:
             self._by_name.pop(old_record.name)
         self._by_name[record.name] = record
-        if not isinstance(record.key, str):
-            self._by_key[record.key] = record
+        self._by_key[record.key] = record
 
     def set(self, records: Iterable[CollectionRecord], *, full: bool = False) -> None:
         """Replace cache contents with the new set of records.
 
         Parameters
         ----------
         records : `~collections.abc.Iterable` [`CollectionRecord`]
             Collection records.
         full : `bool`
             If `True` then ``records`` contain all known collection records.
         """
         self.clear()
         for record in records:
             self._by_name[record.name] = record
-            if not isinstance(record.key, str):
-                self._by_key[record.key] = record
+            self._by_key[record.key] = record
         self._full = full
 
     def clear(self) -> None:
         """Remove all records from the cache."""
         self._by_name = {}
         self._by_key = {}
         self._full = False
@@ -110,16 +108,15 @@
 
         Parameters
         ----------
         record : `CollectionRecord`
             Collection record to remove.
         """
         self._by_name.pop(record.name, None)
-        if not isinstance(record.key, str):
-            self._by_key.pop(record.key, None)
+        self._by_key.pop(record.key, None)
 
     def get_by_name(self, name: str) -> CollectionRecord | None:
         """Return collection record given its name.
 
         Parameters
         ----------
         name : `str`
@@ -143,16 +140,14 @@
 
         Returns
         -------
         record : `CollectionRecord` or `None`
             Collection record, `None` is returned if the key is not in the
             cache.
         """
-        if isinstance(key, str):
-            return self._by_name.get(key)
         return self._by_key.get(key)
 
     def records(self) -> Iterator[CollectionRecord]:
         """Return iterator for the set of records in the cache, can only be
         used if `full` is true.
 
         Raises
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDatasets.py`

 * *Files 24% similar despite different names*

```diff
@@ -22,222 +22,204 @@
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
-__all__ = ("CollectionSummary",)
-
 import dataclasses
-from collections.abc import Generator, Iterable, Mapping, Set
-from typing import cast
+from collections import defaultdict
+from collections.abc import Iterable
+from types import EllipsisType
+from typing import TYPE_CHECKING
 
-from .._dataset_ref import DatasetRef
-from .._dataset_type import DatasetType
-from .._named import NamedValueSet
-from ..dimensions import DataCoordinate
+import numpy as np
+from astropy.table import Table as AstropyTable
 
+from .._butler import Butler
+from ..cli.utils import sortAstropyTable
 
-@dataclasses.dataclass
-class CollectionSummary:
-    """A summary of the datasets that can be found in a collection."""
+if TYPE_CHECKING:
+    from lsst.daf.butler import DatasetRef
+    from lsst.daf.butler.registry.queries import DatasetQueryResults
+    from lsst.resources import ResourcePath
 
-    def copy(self) -> CollectionSummary:
-        """Return a deep copy of this object.
 
-        Returns
-        -------
-        copy : `CollectionSummary`
-            A copy of ``self`` that can be modified without modifying ``self``
-            at all.
-        """
-        return CollectionSummary(
-            dataset_types=self.dataset_types.copy(),
-            governors={k: v.copy() for k, v in self.governors.items()},
-        )
-
-    def add_datasets_generator(self, refs: Iterable[DatasetRef]) -> Generator[DatasetRef, None, None]:
-        """Include the given datasets in the summary, yielding them back as a
-        generator.
-
-        Parameters
-        ----------
-        refs : `~collections.abc.Iterable` [ `DatasetRef` ]
-            Datasets to include.
+@dataclasses.dataclass(frozen=True)
+class _RefInfo:
+    datasetRef: DatasetRef
+    uri: str | None
 
-        Yields
-        ------
-        ref : `DatasetRef`
-            The same dataset references originally passed in.
-
-        Notes
-        -----
-        As a generator, this method does nothing if its return iterator is not
-        used.  Call `add_datasets` instead to avoid this; this method is
-        intended for the case where the given iterable may be single-pass and a
-        copy is not desired, but other processing needs to be done on its
-        elements.
-        """
-        for ref in refs:
-            self.dataset_types.add(ref.datasetType)
-            for gov in ref.dataId.dimensions.governors:
-                self.governors.setdefault(gov, set()).add(cast(str, ref.dataId[gov]))
-            yield ref
 
-    def add_datasets(self, refs: Iterable[DatasetRef]) -> None:
-        """Include the given datasets in the summary.
+class _Table:
+    """Aggregates rows for a single dataset type, and creates an astropy table
+    with the aggregated data. Eliminates duplicate rows.
+    """
 
-        Parameters
-        ----------
-        refs : `~collections.abc.Iterable` [ `DatasetRef` ]
-            Datasets to include.
-        """
-        for _ in self.add_datasets_generator(refs):
-            pass
+    datasetRefs: set[_RefInfo]
 
-    def add_data_ids_generator(
-        self, dataset_type: DatasetType, data_ids: Iterable[DataCoordinate]
-    ) -> Generator[DataCoordinate, None, None]:
-        """Include the given dataset type and data IDs in the summary, yielding
-        them back as a generator.
+    def __init__(self) -> None:
+        self.datasetRefs = set()
 
-        Parameters
-        ----------
-        dataset_type : `DatasetType`
-            Dataset type to include.
-        data_ids : `~collections.abc.Iterable` [ `DataCoordinate` ]
-            Data IDs to include.
-
-        Yields
-        ------
-        data_id : `DataCoordinate`
-            The same data IDs originally passed in.
-
-        Notes
-        -----
-        As a generator, this method does nothing if its return iterator is not
-        used.  Call `add_data_ids` instead to avoid this; this method is
-        intended for the case where the given iterable may be single-pass and a
-        copy is not desired, but other processing needs to be done on its
-        elements.
-        """
-        self.dataset_types.add(dataset_type)
-        for data_id in data_ids:
-            for gov in data_id.dimensions.governors:
-                self.governors.setdefault(gov, set()).add(cast(str, data_id[gov]))
-            yield data_id
+    def add(self, datasetRef: DatasetRef, uri: ResourcePath | None = None) -> None:
+        """Add a row of information to the table.
 
-    def add_data_ids(self, dataset_type: DatasetType, data_ids: Iterable[DataCoordinate]) -> None:
-        """Include the given dataset type and data IDs in the summary.
+        ``uri`` is optional but must be the consistent; provided or not, for
+        every call to a ``_Table`` instance.
 
         Parameters
         ----------
-        dataset_type : `DatasetType`
-            Dataset type to include.
-        data_ids : `~collections.abc.Iterable` [ `DataCoordinate` ]
-            Data IDs to include.
+        datasetRef : `DatasetRef`
+            A dataset ref that will be added as a row in the table.
+        uri : `lsst.resources.ResourcePath`, optional
+            The URI to show as a file location in the table, by default `None`.
         """
-        for _ in self.add_data_ids_generator(dataset_type, data_ids):
-            pass
+        uri_str = str(uri) if uri else None
+        self.datasetRefs.add(_RefInfo(datasetRef, uri_str))
 
-    def update(self, *args: CollectionSummary) -> None:
-        """Update this summary with dataset types and governor dimension values
-        from other summaries.
+    def getAstropyTable(self, datasetTypeName: str) -> AstropyTable:
+        """Get the table as an astropy table.
 
         Parameters
         ----------
-        *args : `CollectionSummary`
-            Summaries to include in ``self``.
-        """
-        for arg in args:
-            self.dataset_types.update(arg.dataset_types)
-            for gov, values in arg.governors.items():
-                self.governors.setdefault(gov, set()).update(values)
-
-    def union(*args: CollectionSummary) -> CollectionSummary:
-        """Construct a summary that contains all dataset types and governor
-        dimension values in any of the inputs.
-
-        Parameters
-        ----------
-        *args : `CollectionSummary`
-            Summaries to combine.
+        datasetTypeName : `str`
+            The dataset type name to show in the ``type`` column of the table.
 
         Returns
         -------
-        unioned : `CollectionSummary`
-            New summary object that represents the union of the given ones.
+        table : `astropy.table._Table`
+            The table with the provided column names and rows.
         """
-        result = CollectionSummary()
-        result.update(*args)
-        return result
+        # Should never happen; adding a dataset should be the action that
+        # causes a _Table to be created.
+        if not self.datasetRefs:
+            raise RuntimeError(f"No DatasetRefs were provided for dataset type {datasetTypeName}")
+
+        refInfo = next(iter(self.datasetRefs))
+        dimensions = [
+            refInfo.datasetRef.dataId.universe.dimensions[k]
+            for k in refInfo.datasetRef.dataId.dimensions.data_coordinate_keys
+        ]
+        columnNames = ["type", "run", "id", *[str(item) for item in dimensions]]
+
+        # Need to hint the column types for numbers since the per-row
+        # constructor of Table does not work this out on its own and sorting
+        # will not work properly without.
+        typeMap = {float: np.float64, int: np.int64}
+        columnTypes = [
+            None,
+            None,
+            str,
+            *[typeMap.get(type(value)) for value in refInfo.datasetRef.dataId.full_values],
+        ]
+        if refInfo.uri:
+            columnNames.append("URI")
+            columnTypes.append(None)
+
+        rows = []
+        for refInfo in self.datasetRefs:
+            row = [
+                datasetTypeName,
+                refInfo.datasetRef.run,
+                str(refInfo.datasetRef.id),
+                *refInfo.datasetRef.dataId.full_values,
+            ]
+            if refInfo.uri:
+                row.append(refInfo.uri)
+            rows.append(row)
+
+        dataset_table = AstropyTable(np.array(rows), names=columnNames, dtype=columnTypes)
+        return sortAstropyTable(dataset_table, dimensions, ["type", "run"])
+
+
+class QueryDatasets:
+    """Get dataset refs from a repository.
+
+    Parameters
+    ----------
+    glob : iterable [`str`]
+        A list of glob-style search string that fully or partially identify
+        the dataset type names to search for.
+    collections : iterable [`str`]
+        A list of glob-style search string that fully or partially identify
+        the collections to search for.
+    where : `str`
+        A string expression similar to a SQL WHERE clause.  May involve any
+        column of a dimension table or (as a shortcut for the primary key
+        column of a dimension table) dimension name.
+    find_first : `bool`
+        For each result data ID, only yield one DatasetRef of each DatasetType,
+        from the first collection in which a dataset of that dataset type
+        appears (according to the order of `collections` passed in).  If used,
+        `collections` must specify at least one expression and must not contain
+        wildcards.
+    show_uri : `bool`
+        If True, include the dataset URI in the output.
+    repo : `str` or `None`
+        URI to the location of the repo or URI to a config file describing the
+        repo and its location. One of `repo` and `butler` must be `None` and
+        the other must not be `None`.
+    butler : `lsst.daf.butler.Butler` or `None`
+        The butler to use to query. One of `repo` and `butler` must be `None`
+        and the other must not be `None`.
+    """
 
-    def is_compatible_with(
+    def __init__(
         self,
-        dataset_type: DatasetType,
-        dimensions: Mapping[str, Set[str]],
-        rejections: list[str] | None = None,
-        name: str | None = None,
-    ) -> bool:
-        """Test whether the collection summarized by this object should be
-        queried for a given dataset type and governor dimension values.
+        glob: Iterable[str],
+        collections: Iterable[str],
+        where: str,
+        find_first: bool,
+        show_uri: bool,
+        repo: str | None = None,
+        butler: Butler | None = None,
+    ):
+        if (repo and butler) or (not repo and not butler):
+            raise RuntimeError("One of repo and butler must be provided and the other must be None.")
+        # show_uri requires a datastore.
+        without_datastore = not show_uri
+        self.butler = butler or Butler.from_config(repo, without_datastore=without_datastore)
+        self._getDatasets(glob, collections, where, find_first)
+        self.showUri = show_uri
+
+    def _getDatasets(
+        self, glob: Iterable[str], collections: Iterable[str], where: str, find_first: bool
+    ) -> None:
+        datasetTypes = glob or ...
+        query_collections: Iterable[str] | EllipsisType = collections or ...
+
+        self.datasets = self.butler.registry.queryDatasets(
+            datasetType=datasetTypes, collections=query_collections, where=where, findFirst=find_first
+        ).expanded()
 
-        Parameters
-        ----------
-        dataset_type : `DatasetType`
-            Dataset type being queried.  If this collection has no instances of
-            this dataset type (or its parent dataset type, if it is a
-            component), `False` will always be returned.
-        dimensions : `~collections.abc.Mapping`
-            Bounds on the values governor dimensions can take in the query,
-            usually from a WHERE expression, as a mapping from dimension name
-            to a set of `str` governor dimension values.
-        rejections : `list` [ `str` ], optional
-            If provided, a list that will be populated with a log- or
-            exception-friendly message explaining why this dataset is
-            incompatible with this collection when `False` is returned.
-        name : `str`, optional
-            Name of the collection this object summarizes, for use in messages
-            appended to ``rejections``.  Ignored if ``rejections`` is `None`.
+    def getTables(self) -> list[AstropyTable]:
+        """Get the datasets as a list of astropy tables.
 
         Returns
         -------
-        compatible : `bool`
-            `True` if the dataset query described by this summary and the given
-            arguments might yield non-empty results; `False` if the result from
-            such a query is definitely empty.
+        datasetTables : `list` [``astropy.table._Table``]
+            A list of astropy tables, one for each dataset type.
         """
-        parent = dataset_type if not dataset_type.isComponent() else dataset_type.makeCompositeDatasetType()
-        if parent.name not in self.dataset_types.names:
-            if rejections is not None:
-                rejections.append(f"No datasets of type {parent.name} in collection {name!r}.")
-            return False
-        for gov_name in self.governors.keys() & dataset_type.dimensions.names & dimensions.keys():
-            values_in_collection = self.governors[gov_name]
-            values_given = dimensions[gov_name]
-            if values_in_collection.isdisjoint(values_given):
-                if rejections is not None:
-                    rejections.append(
-                        f"No datasets with {gov_name} in {values_given} in collection {name!r}."
-                    )
-                return False
-        return True
-
-    dataset_types: NamedValueSet[DatasetType] = dataclasses.field(default_factory=NamedValueSet)
-    """Dataset types that may be present in the collection
-    (`NamedValueSet` [ `DatasetType` ]).
+        tables: dict[str, _Table] = defaultdict(_Table)
+        if not self.showUri:
+            for dataset_ref in self.datasets:
+                tables[dataset_ref.datasetType.name].add(dataset_ref)
+        else:
+            d = list(self.datasets)
+            ref_uris = self.butler.get_many_uris(d, predict=True)
+            for ref, uris in ref_uris.items():
+                if uris.primaryURI:
+                    tables[ref.datasetType.name].add(ref, uris.primaryURI)
+                for name, uri in uris.componentURIs.items():
+                    tables[ref.datasetType.componentTypeName(name)].add(ref, uri)
 
-    A dataset type not in this set is definitely not in the collection, but
-    the converse is not necessarily true.
-    """
+        return [table.getAstropyTable(datasetTypeName) for datasetTypeName, table in tables.items()]
 
-    governors: dict[str, set[str]] = dataclasses.field(default_factory=dict)
-    """Governor data ID values that are present in the collection's dataset
-    data IDs (`dict` [ `str`, `set` [ `str` ] ]).
-
-    A data ID value not in this restriction is not necessarily inconsistent
-    with a query in the collection; such a search may only involve dataset
-    types that do not include one or more governor dimensions in their data
-    IDs, and hence the values of those data IDs are unconstrained by this
-    collection in the query.
-    """
+    def getDatasets(self) -> DatasetQueryResults:
+        """Get the datasets as a list of ``DatasetQueryResults``.
+
+        Returns
+        -------
+        refs : `lsst.daf.butler.registry.queries.DatasetQueryResults`
+            Dataset references matching the given query criteria.
+        """
+        return self.datasets
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_summary_cache.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_summary_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_collection_type.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_collection_type.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_config.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_dataset_type_cache.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_dataset_type_cache.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_defaults.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_defaults.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,17 +31,17 @@
 
 import contextlib
 from collections.abc import Sequence, Set
 from typing import TYPE_CHECKING, Any
 
 from lsst.utils.classes import immutable
 
+from .._exceptions import MissingCollectionError
 from ..dimensions import DataCoordinate
 from ._collection_summary import CollectionSummary
-from ._exceptions import MissingCollectionError
 from .wildcards import CollectionWildcard
 
 if TYPE_CHECKING:
     from .sql_registry import SqlRegistry
 
 
 @immutable
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_exceptions.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_exceptions.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,109 +24,53 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 
 __all__ = (
     "ArgumentError",
-    "CollectionError",
     "CollectionExpressionError",
-    "CollectionTypeError",
     "ConflictingDefinitionError",
-    "DataIdError",
     "DataIdValueError",
-    "DatasetTypeError",
     "DatasetTypeExpressionError",
-    "DimensionNameError",
     "InconsistentDataIdError",
-    "MissingCollectionError",
-    "MissingDatasetTypeError",
     "MissingSpatialOverlapError",
     "NoDefaultCollectionError",
     "OrphanedRecordError",
     "RegistryConsistencyError",
-    "RegistryError",
     "UnsupportedIdGeneratorError",
     "UserExpressionError",
     "UserExpressionSyntaxError",
 )
 
-
-class RegistryError(Exception):
-    """Base class for many exception classes produced by Registry methods.
-
-    Notes
-    -----
-    The client code that needs to handle exceptions generated by the Registry
-    methods can catch this class or one of its many subclasses as described by
-    the particular method documentation. While most of the Registry methods
-    should only raise the exceptions of this type, it is hard to guarantee
-    that they will never raise other exception types. If the client needs to
-    handle all possible exceptions, then it should also catch a standard
-    `Exception` type as well. Additionally, some Registry methods can be
-    explicitly documented to raise exceptions outside this class hierarchy.
-    """
+from .._exceptions_legacy import CollectionError, DataIdError, RegistryError
 
 
 class ArgumentError(RegistryError):
     """Exception raised when method arguments are invalid or inconsistent."""
 
 
-class DatasetTypeError(RegistryError):
-    """Exception raised for problems with dataset types."""
-
-
-class MissingDatasetTypeError(DatasetTypeError, KeyError):
-    """Exception raised when a dataset type does not exist."""
-
-
 class DatasetTypeExpressionError(RegistryError):
     """Exception raised for an incorrect dataset type expression."""
 
 
-class DataIdError(RegistryError):
-    """Exception raised for incorrect data IDs, this is a base class for other
-    specific error types.
-    """
-
-
-class DimensionNameError(DataIdError):
-    """Exception raised when a dimension specified in a data ID does not exist
-    or required dimension is not provided.
-    """
-
-
 class DataIdValueError(DataIdError):
     """Exception raised when a value specified in a data ID does not exist."""
 
 
 class InconsistentDataIdError(DataIdError):
     """Exception raised when a data ID contains contradictory key-value pairs,
     according to dimension relationships.
     """
 
 
-class CollectionError(RegistryError):
-    """Exception raised for collection-related errors."""
-
-
-class CollectionTypeError(CollectionError):
-    """Exception raised when type of a collection is incorrect."""
-
-
 class CollectionExpressionError(CollectionError):
     """Exception raised for an incorrect collection expression."""
 
 
-class MissingCollectionError(CollectionError):
-    """Exception raised when an operation attempts to use a collection that
-    does not exist.
-    """
-
-
 class NoDefaultCollectionError(CollectionError):
     """Exception raised when a collection is needed, but collection argument
     is not provided and default collection is not defined in registry.
     """
 
 
 class UserExpressionError(RegistryError):
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_registry.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/_registry_factory.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/_registry_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/attributes.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/attributes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/ephemeral.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/ephemeral.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/bridge/monolithic.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/bridge/monolithic.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/_base.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,25 +26,24 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 from ... import ddl
 
 __all__ = ()
 
-import itertools
 from abc import abstractmethod
-from collections import namedtuple
-from collections.abc import Iterable, Iterator, Set
-from typing import TYPE_CHECKING, Any, TypeVar, cast
+from collections.abc import Callable, Iterable, Iterator, Set
+from contextlib import contextmanager
+from typing import TYPE_CHECKING, Any, Generic, Literal, NamedTuple, TypeVar, cast
 
 import sqlalchemy
 
+from ..._exceptions import CollectionCycleError, CollectionTypeError, MissingCollectionError
 from ...timespan_database_representation import TimespanDatabaseRepresentation
 from .._collection_type import CollectionType
-from .._exceptions import MissingCollectionError
 from ..interfaces import ChainedCollectionRecord, CollectionManager, CollectionRecord, RunRecord, VersionTuple
 from ..wildcards import CollectionWildcard
 
 if TYPE_CHECKING:
     from .._caching_context import CachingContext
     from ..interfaces import Database
 
@@ -73,15 +72,21 @@
     This method assumes fixed name ("collection") of a collections table.
     There is also a general assumption that collection primary key consists
     of a single column.
     """
     return ddl.ForeignKeySpec("collection", source=(sourceColumnName,), target=(collectionIdName,), **kwargs)
 
 
-CollectionTablesTuple = namedtuple("CollectionTablesTuple", ["collection", "run", "collection_chain"])
+_T = TypeVar("_T")
+
+
+class CollectionTablesTuple(NamedTuple, Generic[_T]):
+    collection: _T
+    run: _T
+    collection_chain: _T
 
 
 def makeRunTableSpec(
     collectionIdName: str, collectionIdType: type, TimespanReprClass: type[TimespanDatabaseRepresentation]
 ) -> ddl.TableSpec:
     """Define specification for "run" table.
 
@@ -184,15 +189,15 @@
     in memory. Memory cache is synchronized from database when `refresh`
     method is called.
     """
 
     def __init__(
         self,
         db: Database,
-        tables: CollectionTablesTuple,
+        tables: CollectionTablesTuple[sqlalchemy.Table],
         collectionIdName: str,
         *,
         caching_context: CachingContext,
         registry_schema_version: VersionTuple | None = None,
     ):
         super().__init__(registry_schema_version=registry_schema_version)
         self._db = db
@@ -400,43 +405,267 @@
     def _fetch_by_key(self, collection_ids: Iterable[K] | None) -> list[CollectionRecord[K]]:
         """Fetch collection record from database given its key, or fetch all
         collctions if argument is None.
         """
         raise NotImplementedError()
 
     def update_chain(
-        self, chain: ChainedCollectionRecord[K], children: Iterable[str], flatten: bool = False
-    ) -> ChainedCollectionRecord[K]:
-        # Docstring inherited from CollectionManager.
-        children_as_wildcard = CollectionWildcard.from_names(children)
+        self,
+        parent_collection_name: str,
+        child_collection_names: list[str],
+        allow_use_in_caching_context: bool = False,
+    ) -> None:
+        with self._modify_collection_chain(
+            parent_collection_name,
+            child_collection_names,
+            # update_chain is currently used in setCollectionChain, which is
+            # called within caching contexts.  (At least in Butler.import_ and
+            # possibly other places.)  So, unlike the other collection chain
+            # modification methods, it has to update the collection cache.
+            skip_caching_check=allow_use_in_caching_context,
+        ) as c:
+            self._db.delete(self._tables.collection_chain, ["parent"], {"parent": c.parent_key})
+            self._block_for_concurrency_test()
+            self._insert_collection_chain_rows(c.parent_key, 0, c.child_keys)
+
+        names = [child.name for child in c.child_records]
+        record = ChainedCollectionRecord[K](c.parent_key, parent_collection_name, children=tuple(names))
+        self._addCachedRecord(record)
+
+    def prepend_collection_chain(
+        self, parent_collection_name: str, child_collection_names: list[str]
+    ) -> None:
+        self._add_to_collection_chain(
+            parent_collection_name, child_collection_names, self._find_prepend_position
+        )
+
+    def extend_collection_chain(self, parent_collection_name: str, child_collection_names: list[str]) -> None:
+        self._add_to_collection_chain(
+            parent_collection_name, child_collection_names, self._find_extend_position
+        )
+
+    def _add_to_collection_chain(
+        self,
+        parent_collection_name: str,
+        child_collection_names: list[str],
+        position_func: Callable[[_CollectionChainModificationContext], int],
+    ) -> None:
+        with self._modify_collection_chain(parent_collection_name, child_collection_names) as c:
+            # Remove any of the new children that are already in the
+            # collection, so they move to a new position instead of being
+            # duplicated.
+            self._remove_collection_chain_rows(c.parent_key, c.child_keys)
+            # Figure out where to insert the new children.
+            starting_position = position_func(c)
+            self._block_for_concurrency_test()
+            self._insert_collection_chain_rows(c.parent_key, starting_position, c.child_keys)
+
+    def remove_from_collection_chain(
+        self, parent_collection_name: str, child_collection_names: list[str]
+    ) -> None:
+        with self._modify_collection_chain(
+            parent_collection_name,
+            child_collection_names,
+            # Removing members from a chain can't create collection cycles
+            skip_cycle_check=True,
+        ) as c:
+            self._remove_collection_chain_rows(c.parent_key, c.child_keys)
+
+    @contextmanager
+    def _modify_collection_chain(
+        self,
+        parent_collection_name: str,
+        child_collection_names: list[str],
+        *,
+        skip_caching_check: bool = False,
+        skip_cycle_check: bool = False,
+    ) -> Iterator[_CollectionChainModificationContext[K]]:
+        if (not skip_caching_check) and self._caching_context.is_enabled:
+            # Avoid having cache-maintenance code around that is unlikely to
+            # ever be used.
+            raise RuntimeError("Chained collection modification not permitted with active caching context.")
+
+        if not skip_cycle_check:
+            self._sanity_check_collection_cycles(parent_collection_name, child_collection_names)
+
+        # Look up the collection primary keys corresponding to the
+        # user-provided list of child collection names.  Because there is no
+        # locking for the child collections, it's possible for a concurrent
+        # deletion of one of the children to cause a foreign key constraint
+        # violation when we attempt to insert them in the collection chain
+        # table later.
+        child_records = self.resolve_wildcard(
+            CollectionWildcard.from_names(child_collection_names), flatten_chains=False
+        )
+        child_keys = [child.key for child in child_records]
+
+        with self._db.transaction():
+            # Lock the parent collection to prevent concurrent updates to the
+            # same collection chain.
+            parent_key = self._find_and_lock_collection_chain(parent_collection_name)
+            yield _CollectionChainModificationContext[K](
+                parent_key=parent_key, child_keys=child_keys, child_records=child_records
+            )
+
+    def _sanity_check_collection_cycles(
+        self, parent_collection_name: str, child_collection_names: list[str]
+    ) -> None:
+        """Raise an exception if any of the collections in the ``child_names``
+        list have ``parent_name`` as a child, creating a collection cycle.
+
+        This is only a sanity check, and does not guarantee that no collection
+        cycles are possible.  Concurrent updates might allow collection cycles
+        to be inserted.
+        """
         for record in self.resolve_wildcard(
-            children_as_wildcard,
+            CollectionWildcard.from_names(child_collection_names),
             flatten_chains=True,
             include_chains=True,
             collection_types={CollectionType.CHAINED},
         ):
-            if record == chain:
-                raise ValueError(f"Cycle in collection chaining when defining '{chain.name}'.")
-        if flatten:
-            children = tuple(
-                record.name for record in self.resolve_wildcard(children_as_wildcard, flatten_chains=True)
-            )
+            if record.name == parent_collection_name:
+                raise CollectionCycleError(
+                    f"Cycle in collection chaining when defining '{parent_collection_name}'."
+                )
+
+    def _insert_collection_chain_rows(
+        self,
+        parent_key: K,
+        starting_position: int,
+        child_keys: list[K],
+    ) -> None:
+        rows = [
+            {
+                "parent": parent_key,
+                "child": child,
+                "position": position,
+            }
+            for position, child in enumerate(child_keys, starting_position)
+        ]
+
+        # It's possible for the DB to raise an exception for the integers being
+        # out of range here.  The position column is only a 16-bit number.
+        # Even if there aren't an unreasonably large number of children in the
+        # collection, a series of many deletes and insertions could cause the
+        # space to become fragmented.
+        #
+        # If this ever actually happens, we should consider doing a migration
+        # to increase the position column to a 32-bit number.
+        # To fix it in the short term, you can re-write the collection chain to
+        # defragment it by doing something like:
+        # registry.setCollectionChain(
+        #     parent,
+        #     registry.getCollectionChain(parent)
+        # )
+        self._db.insert(self._tables.collection_chain, *rows)
 
-        rows = []
-        position = itertools.count()
-        names = []
-        for child in self.resolve_wildcard(CollectionWildcard.from_names(children), flatten_chains=False):
-            rows.append(
-                {
-                    "parent": chain.key,
-                    "child": child.key,
-                    "position": next(position),
-                }
+    def _remove_collection_chain_rows(
+        self,
+        parent_key: K,
+        child_keys: list[K],
+    ) -> None:
+        table = self._tables.collection_chain
+        where = sqlalchemy.and_(table.c.parent == parent_key, table.c.child.in_(child_keys))
+        self._db.deleteWhere(table, where)
+
+    def _find_prepend_position(self, c: _CollectionChainModificationContext) -> int:
+        """Return the position where children can be inserted to
+        prepend them to a collection chain.
+        """
+        return self._find_position_in_collection_chain(c.parent_key, "begin") - len(c.child_keys)
+
+    def _find_extend_position(self, c: _CollectionChainModificationContext) -> int:
+        """Return the position where children can be inserted to append them to
+        a collection chain.
+        """
+        return self._find_position_in_collection_chain(c.parent_key, "end") + 1
+
+    def _find_position_in_collection_chain(self, chain_key: K, begin_or_end: Literal["begin", "end"]) -> int:
+        """Return the lowest or highest numbered position in a collection
+        chain, or 0 if the chain is empty.
+        """
+        table = self._tables.collection_chain
+
+        func: sqlalchemy.Function
+        match (begin_or_end):
+            case "begin":
+                func = sqlalchemy.func.min(table.c.position)
+            case "end":
+                func = sqlalchemy.func.max(table.c.position)
+
+        query = sqlalchemy.select(func).where(table.c.parent == chain_key)
+        with self._db.query(query) as cursor:
+            position = cursor.scalar()
+
+        if position is None:
+            return 0
+
+        return position
+
+    def _find_and_lock_collection_chain(self, collection_name: str) -> K:
+        """
+        Take a row lock on the specified collection's row in the collections
+        table, and return the collection's primary key.
+
+        This lock is used to synchronize updates to collection chains.
+
+        The locking strategy requires cooperation from everything modifying the
+        collection chain table -- all operations that modify collection chains
+        must obtain this lock first.  The database will NOT automatically
+        prevent modification of tables based on this lock.  The only guarantee
+        is that only one caller will be allowed to hold this lock for a given
+        collection at a time.  Concurrent calls will block until the caller
+        holding the lock has completed its transaction.
+
+        Parameters
+        ----------
+        collection_name : `str`
+            Name of the collection whose chain is being modified.
+
+        Returns
+        -------
+        id : ``K``
+            The primary key for the given collection.
+
+        Raises
+        ------
+        MissingCollectionError
+            If the specified collection is not in the database table.
+        CollectionTypeError
+            If the specified collection is not a chained collection.
+        """
+        assert self._db.isInTransaction(), (
+            "Row locks are only held until the end of the current transaction,"
+            " so it makes no sense to take a lock outside a transaction."
+        )
+        assert self._db.isWriteable(), "Collection row locks are only useful for write operations."
+
+        query = self._select_pkey_by_name(collection_name).with_for_update()
+        with self._db.query(query) as cursor:
+            rows = cursor.all()
+
+        if len(rows) == 0:
+            raise MissingCollectionError(
+                f"Parent collection {collection_name} not found when updating collection chain."
             )
-            names.append(child.name)
-        with self._db.transaction():
-            self._db.delete(self._tables.collection_chain, ["parent"], {"parent": chain.key})
-            self._db.insert(self._tables.collection_chain, *rows)
+        assert len(rows) == 1, "There should only be one entry for each collection in collection table."
+        r = rows[0]._mapping
+        if r["type"] != CollectionType.CHAINED:
+            raise CollectionTypeError(f"Parent collection {collection_name} is not a chained collection.")
+        return r["key"]
 
-        record = ChainedCollectionRecord[K](chain.key, chain.name, children=tuple(names))
-        self._addCachedRecord(record)
-        return record
+    @abstractmethod
+    def _select_pkey_by_name(self, collection_name: str) -> sqlalchemy.Select:
+        """Return a SQLAlchemy select statement that will return columns from
+        the one row in the ``collection` table matching the given name.  The
+        select statement includes two columns:
+
+        - ``key`` : the primary key for the collection
+        - ``type`` : the collection type
+        """
+        raise NotImplementedError()
+
+
+class _CollectionChainModificationContext(NamedTuple, Generic[K]):
+    parent_key: K
+    child_keys: list[K]
+    child_records: list[CollectionRecord[K]]
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/nameKey.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/nameKey.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 import logging
 from collections.abc import Iterable, Mapping
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy
 
 from ... import ddl
+from ...column_spec import COLLECTION_NAME_MAX_LENGTH
 from ...timespan_database_representation import TimespanDatabaseRepresentation
 from .._collection_type import CollectionType
 from ..interfaces import ChainedCollectionRecord, CollectionRecord, RunRecord, VersionTuple
 from ._base import (
     CollectionTablesTuple,
     DefaultCollectionManager,
     makeCollectionChainTableSpec,
@@ -46,25 +47,29 @@
 )
 
 if TYPE_CHECKING:
     from .._caching_context import CachingContext
     from ..interfaces import Database, StaticTablesContext
 
 
-_KEY_FIELD_SPEC = ddl.FieldSpec("name", dtype=sqlalchemy.String, length=64, primaryKey=True)
+_KEY_FIELD_SPEC = ddl.FieldSpec(
+    "name", dtype=sqlalchemy.String, length=COLLECTION_NAME_MAX_LENGTH, primaryKey=True
+)
 
 
 # This has to be updated on every schema change
 _VERSION = VersionTuple(2, 0, 0)
 
 
 _LOG = logging.getLogger(__name__)
 
 
-def _makeTableSpecs(TimespanReprClass: type[TimespanDatabaseRepresentation]) -> CollectionTablesTuple:
+def _makeTableSpecs(
+    TimespanReprClass: type[TimespanDatabaseRepresentation],
+) -> CollectionTablesTuple[ddl.TableSpec]:
     return CollectionTablesTuple(
         collection=ddl.TableSpec(
             fields=[
                 _KEY_FIELD_SPEC,
                 ddl.FieldSpec("type", dtype=sqlalchemy.SmallInteger, nullable=False),
                 ddl.FieldSpec("doc", dtype=sqlalchemy.Text, nullable=True),
             ],
@@ -175,14 +180,20 @@
             .select_from(table)
             .where(table.columns["child"] == key)
         )
         with self._db.query(sql) as sql_result:
             parent_names = set(sql_result.scalars().all())
         return parent_names
 
+    def lookup_name_sql(
+        self, sql_key: sqlalchemy.ColumnElement[str], sql_from_clause: sqlalchemy.FromClause
+    ) -> tuple[sqlalchemy.ColumnElement[str], sqlalchemy.FromClause]:
+        # Docstring inherited.
+        return sql_key, sql_from_clause
+
     def _fetch_by_name(self, names: Iterable[str]) -> list[CollectionRecord[str]]:
         # Docstring inherited from base class.
         return self._fetch_by_key(names)
 
     def _fetch_by_key(self, collection_ids: Iterable[str] | None) -> list[CollectionRecord[str]]:
         # Docstring inherited from base class.
         _LOG.debug("Fetching collection records using names %s.", collection_ids)
@@ -276,11 +287,17 @@
                 name=name,
                 children=children_names,
             )
             records.append(record)
 
         return records
 
+    def _select_pkey_by_name(self, collection_name: str) -> sqlalchemy.Select:
+        table = self._tables.collection
+        return sqlalchemy.select(table.c.name.label("key"), table.c.type).where(
+            table.c.name == collection_name
+        )
+
     @classmethod
     def currentVersions(cls) -> list[VersionTuple]:
         # Docstring inherited from VersionedExtension.
         return [_VERSION]
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/collections/synthIntKey.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/collections/synthIntKey.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 
 import logging
 from collections.abc import Iterable, Mapping
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy
 
+from ...column_spec import COLLECTION_NAME_MAX_LENGTH
 from ...timespan_database_representation import TimespanDatabaseRepresentation
 from .._collection_type import CollectionType
 from ..interfaces import ChainedCollectionRecord, CollectionRecord, RunRecord, VersionTuple
 from ._base import (
     CollectionTablesTuple,
     DefaultCollectionManager,
     makeCollectionChainTableSpec,
@@ -58,20 +59,24 @@
 
 # This has to be updated on every schema change
 _VERSION = VersionTuple(2, 0, 0)
 
 _LOG = logging.getLogger(__name__)
 
 
-def _makeTableSpecs(TimespanReprClass: type[TimespanDatabaseRepresentation]) -> CollectionTablesTuple:
+def _makeTableSpecs(
+    TimespanReprClass: type[TimespanDatabaseRepresentation],
+) -> CollectionTablesTuple[ddl.TableSpec]:
     return CollectionTablesTuple(
         collection=ddl.TableSpec(
             fields=[
                 _KEY_FIELD_SPEC,
-                ddl.FieldSpec("name", dtype=sqlalchemy.String, length=64, nullable=False),
+                ddl.FieldSpec(
+                    "name", dtype=sqlalchemy.String, length=COLLECTION_NAME_MAX_LENGTH, nullable=False
+                ),
                 ddl.FieldSpec("type", dtype=sqlalchemy.SmallInteger, nullable=False),
                 ddl.FieldSpec("doc", dtype=sqlalchemy.Text, nullable=True),
             ],
             unique=[("name",)],
         ),
         run=makeRunTableSpec("collection_id", sqlalchemy.BigInteger, TimespanReprClass),
         collection_chain=makeCollectionChainTableSpec("collection_id", sqlalchemy.BigInteger),
@@ -176,14 +181,25 @@
             .join(chain, onclause=collection.columns[self._collectionIdName] == chain.columns["parent"])
             .where(chain.columns["child"] == key)
         )
         with self._db.query(sql) as sql_result:
             parent_names = set(sql_result.scalars().all())
         return parent_names
 
+    def lookup_name_sql(
+        self, sql_key: sqlalchemy.ColumnElement[int], sql_from_clause: sqlalchemy.FromClause
+    ) -> tuple[sqlalchemy.ColumnElement[str], sqlalchemy.FromClause]:
+        # Docstring inherited.
+        return (
+            self._tables.collection.c.name,
+            sql_from_clause.join(
+                self._tables.collection, onclause=self._tables.collection.c[_KEY_FIELD_SPEC.name] == sql_key
+            ),
+        )
+
     def _fetch_by_name(self, names: Iterable[str]) -> list[CollectionRecord[int]]:
         # Docstring inherited from base class.
         _LOG.debug("Fetching collection records using names %s.", names)
         return self._fetch("name", names)
 
     def _fetch_by_key(self, collection_ids: Iterable[int] | None) -> list[CollectionRecord[int]]:
         # Docstring inherited from base class.
@@ -293,11 +309,17 @@
                 name=name,
                 children=children_names,
             )
             records.append(record)
 
         return records
 
+    def _select_pkey_by_name(self, collection_name: str) -> sqlalchemy.Select:
+        table = self._tables.collection
+        return sqlalchemy.select(table.c.collection_id.label("key"), table.c.type).where(
+            table.c.name == collection_name
+        )
+
     @classmethod
     def currentVersions(cls) -> list[VersionTuple]:
         # Docstring inherited from VersionedExtension.
         return [_VERSION]
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/connectionString.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/postgresql.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 import psycopg2
 import sqlalchemy
 import sqlalchemy.dialects.postgresql
 from sqlalchemy import sql
 
 from ..._named import NamedValueAbstractSet
 from ..._timespan import Timespan
+from ...name_shrinker import NameShrinker
 from ...timespan_database_representation import TimespanDatabaseRepresentation
 from ..interfaces import Database
-from ..nameShrinker import NameShrinker
 
 _SERVER_VERSION_REGEX = re.compile(r"(?P<major>\d+)\.(?P<minor>\d+)")
 
 
 class PostgresqlDatabase(Database):
     """An implementation of the `Database` interface for PostgreSQL.
 
@@ -370,18 +370,18 @@
             return None
         if not isinstance(value, Timespan):
             raise TypeError(f"Unsupported type: {type(value)}, expected Timespan.")
         if value.isEmpty():
             return psycopg2.extras.NumericRange(empty=True)
         else:
             converter = time_utils.TimeConverter()
-            assert value._nsec[0] >= converter.min_nsec, "Guaranteed by Timespan.__init__."
-            assert value._nsec[1] <= converter.max_nsec, "Guaranteed by Timespan.__init__."
-            lower = None if value._nsec[0] == converter.min_nsec else value._nsec[0]
-            upper = None if value._nsec[1] == converter.max_nsec else value._nsec[1]
+            assert value.nsec[0] >= converter.min_nsec, "Guaranteed by Timespan.__init__."
+            assert value.nsec[1] <= converter.max_nsec, "Guaranteed by Timespan.__init__."
+            lower = None if value.nsec[0] == converter.min_nsec else value.nsec[0]
+            upper = None if value.nsec[1] == converter.max_nsec else value.nsec[1]
             return psycopg2.extras.NumericRange(lower=lower, upper=upper)
 
     def process_result_value(
         self, value: psycopg2.extras.NumericRange | None, dialect: sqlalchemy.engine.Dialect
     ) -> Timespan | None:
         if value is None:
             return None
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/databases/sqlite.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,18 @@
 import logging
 from collections.abc import Iterable, Mapping
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy
 
 from ...._dataset_ref import DatasetId, DatasetIdGenEnum, DatasetRef, DatasetType
+from ...._exceptions_legacy import DatasetTypeError
 from ....dimensions import DimensionUniverse
 from ..._collection_summary import CollectionSummary
-from ..._exceptions import (
-    ConflictingDefinitionError,
-    DatasetTypeError,
-    DatasetTypeExpressionError,
-    OrphanedRecordError,
-)
+from ..._exceptions import ConflictingDefinitionError, DatasetTypeExpressionError, OrphanedRecordError
 from ...interfaces import DatasetRecordStorage, DatasetRecordStorageManager, VersionTuple
 from ...wildcards import DatasetTypeWildcard
 from ._storage import ByDimensionsDatasetRecordStorage, ByDimensionsDatasetRecordStorageUUID
 from .summaries import CollectionSummaryManager
 from .tables import (
     addDatasetForeignKey,
     makeCalibTableName,
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/_storage.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,21 +40,24 @@
 import sqlalchemy
 from lsst.daf.relation import Relation, sql
 
 from ...._column_tags import DatasetColumnTag, DimensionKeyColumnTag
 from ...._column_type_info import LogicalColumn
 from ...._dataset_ref import DatasetId, DatasetIdFactory, DatasetIdGenEnum, DatasetRef
 from ...._dataset_type import DatasetType
+from ...._exceptions import CollectionTypeError
 from ...._timespan import Timespan
 from ....dimensions import DataCoordinate
+from ....direct_query_driver import QueryBuilder, QueryJoiner  # new query system, server+direct only
+from ....queries import tree as qt  # new query system, both clients + server
 from ..._collection_summary import CollectionSummary
 from ..._collection_type import CollectionType
-from ..._exceptions import CollectionTypeError, ConflictingDefinitionError
+from ..._exceptions import ConflictingDefinitionError
 from ...interfaces import DatasetRecordStorage
-from ...queries import SqlQueryContext
+from ...queries import SqlQueryContext  # old registry query system
 from .tables import makeTagTableSpec
 
 if TYPE_CHECKING:
     from ...interfaces import CollectionManager, CollectionRecord, Database, RunRecord
     from .summaries import CollectionSummaryManager
     from .tables import StaticDatasetTablesTuple
 
@@ -548,14 +551,207 @@
             payload.columns_available.keys(),
             payload=payload,
             name=self.datasetType.name,
             parameters={record.name: rank for record, rank in collections},
         )
         return leaf
 
+    def make_query_joiner(self, collections: Sequence[CollectionRecord], fields: Set[str]) -> QueryJoiner:
+        # This method largely mimics `make_relation`, but it uses the new query
+        # system primitives instead of the old one.  In terms of the SQL
+        # queries it builds, there are two more main differences:
+        #
+        # - Collection and run columns are now string names rather than IDs.
+        #   This insulates the query result-processing code from collection
+        #   caching and the collection manager subclass details.
+        #
+        # - The subquery always has unique rows, which is achieved by using
+        #   SELECT DISTINCT when necessary.
+        #
+        collection_types = {collection.type for collection in collections}
+        assert CollectionType.CHAINED not in collection_types, "CHAINED collections must be flattened."
+        #
+        # There are two kinds of table in play here:
+        #
+        #  - the static dataset table (with the dataset ID, dataset type ID,
+        #    run ID/name, and ingest date);
+        #
+        #  - the dynamic tags/calibs table (with the dataset ID, dataset type
+        #    type ID, collection ID/name, data ID, and possibly validity
+        #    range).
+        #
+        # That means that we might want to return a query against either table
+        # or a JOIN of both, depending on which quantities the caller wants.
+        # But the data ID is always included, which means we'll always include
+        # the tags/calibs table and join in the static dataset table only if we
+        # need things from it that we can't get from the tags/calibs table.
+        #
+        # Note that it's important that we include a WHERE constraint on both
+        # tables for any column (e.g. dataset_type_id) that is in both when
+        # it's given explicitly; not doing can prevent the query planner from
+        # using very important indexes.  At present, we don't include those
+        # redundant columns in the JOIN ON expression, however, because the
+        # FOREIGN KEY (and its index) are defined only on dataset_id.
+        columns = qt.ColumnSet(self.datasetType.dimensions.as_group())
+        columns.drop_implied_dimension_keys()
+        columns.dataset_fields[self.datasetType.name].update(fields)
+        tags_builder: QueryBuilder | None = None
+        if collection_types != {CollectionType.CALIBRATION}:
+            # We'll need a subquery for the tags table if any of the given
+            # collections are not a CALIBRATION collection.  This intentionally
+            # also fires when the list of collections is empty as a way to
+            # create a dummy subquery that we know will fail.
+            # We give the table an alias because it might appear multiple times
+            # in the same query, for different dataset types.
+            tags_builder = self._finish_query_builder(
+                QueryJoiner(self._db, self._tags.alias(f"{self.datasetType.name}_tags")).to_builder(columns),
+                [record for record in collections if record.type is not CollectionType.CALIBRATION],
+                fields,
+            )
+            if "timespan" in fields:
+                tags_builder.joiner.timespans[self.datasetType.name] = (
+                    self._db.getTimespanRepresentation().fromLiteral(Timespan(None, None))
+                )
+        calibs_builder: QueryBuilder | None = None
+        if CollectionType.CALIBRATION in collection_types:
+            # If at least one collection is a CALIBRATION collection, we'll
+            # need a subquery for the calibs table, and could include the
+            # timespan as a result or constraint.
+            assert (
+                self._calibs is not None
+            ), "DatasetTypes with isCalibration() == False can never be found in a CALIBRATION collection."
+            calibs_builder = self._finish_query_builder(
+                QueryJoiner(self._db, self._calibs.alias(f"{self.datasetType.name}_calibs")).to_builder(
+                    columns
+                ),
+                [record for record in collections if record.type is CollectionType.CALIBRATION],
+                fields,
+            )
+            if "timespan" in fields:
+                calibs_builder.joiner.timespans[self.datasetType.name] = (
+                    self._db.getTimespanRepresentation().from_columns(self._calibs.columns)
+                )
+
+            # In calibration collections, we need timespan as well as data ID
+            # to ensure unique rows.
+            calibs_builder.distinct = calibs_builder.distinct and "timespan" not in fields
+        if tags_builder is not None:
+            if calibs_builder is not None:
+                # Need a UNION subquery.
+                return tags_builder.union_subquery([calibs_builder])
+            else:
+                return tags_builder.to_joiner()
+        elif calibs_builder is not None:
+            return calibs_builder.to_joiner()
+        else:
+            raise AssertionError("Branch should be unreachable.")
+
+    def _finish_query_builder(
+        self,
+        sql_projection: QueryBuilder,
+        collections: Sequence[CollectionRecord],
+        fields: Set[str],
+    ) -> QueryBuilder:
+        # This method plays the same role as _finish_single_relation in the new
+        # query system. It is called exactly one or two times by
+        # make_sql_builder, just as _finish_single_relation is called exactly
+        # one or two times by make_relation.  See make_sql_builder comments for
+        # what's different.
+        assert sql_projection.joiner.from_clause is not None
+        run_collections_only = all(record.type is CollectionType.RUN for record in collections)
+        sql_projection.joiner.where(
+            sql_projection.joiner.from_clause.c.dataset_type_id == self._dataset_type_id
+        )
+        dataset_id_col = sql_projection.joiner.from_clause.c.dataset_id
+        collection_col = sql_projection.joiner.from_clause.c[self._collections.getCollectionForeignKeyName()]
+        fields_provided = sql_projection.joiner.fields[self.datasetType.name]
+        # We always constrain and optionally retrieve the collection(s) via the
+        # tags/calibs table.
+        if "collection_key" in fields:
+            sql_projection.joiner.fields[self.datasetType.name]["collection_key"] = collection_col
+        if len(collections) == 1:
+            only_collection_record = collections[0]
+            sql_projection.joiner.where(collection_col == only_collection_record.key)
+            if "collection" in fields:
+                fields_provided["collection"] = sqlalchemy.literal(only_collection_record.name)
+        elif not collections:
+            sql_projection.joiner.where(sqlalchemy.literal(False))
+            if "collection" in fields:
+                fields_provided["collection"] = sqlalchemy.literal("NO COLLECTIONS")
+        else:
+            sql_projection.joiner.where(collection_col.in_([collection.key for collection in collections]))
+            if "collection" in fields:
+                # Avoid a join to the collection table to get the name by using
+                # a CASE statement.  The SQL will be a bit more verbose but
+                # more efficient.
+                fields_provided["collection"] = sqlalchemy.case(
+                    {record.key: record.name for record in collections}, value=collection_col
+                )
+        # Add more column definitions, starting with the data ID.
+        sql_projection.joiner.extract_dimensions(self.datasetType.dimensions.required.names)
+        # We can always get the dataset_id from the tags/calibs table, even if
+        # could also get it from the 'static' dataset table.
+        if "dataset_id" in fields:
+            fields_provided["dataset_id"] = dataset_id_col
+
+        # It's possible we now have everything we need, from just the
+        # tags/calibs table.  The things we might need to get from the static
+        # dataset table are the run key and the ingest date.
+        need_static_table = False
+        if "run" in fields:
+            if len(collections) == 1 and run_collections_only:
+                # If we are searching exactly one RUN collection, we
+                # know that if we find the dataset in that collection,
+                # then that's the datasets's run; we don't need to
+                # query for it.
+                fields_provided["run"] = sqlalchemy.literal(only_collection_record.name)
+            elif run_collections_only:
+                # Once again we can avoid joining to the collection table by
+                # adding a CASE statement.
+                fields_provided["run"] = sqlalchemy.case(
+                    {record.key: record.name for record in collections},
+                    value=self._static.dataset.c[self._runKeyColumn],
+                )
+                need_static_table = True
+            else:
+                # Here we can't avoid a join to the collection table, because
+                # we might find a dataset via something other than its RUN
+                # collection.
+                (
+                    fields_provided["run"],
+                    sql_projection.joiner.from_clause,
+                ) = self._collections.lookup_name_sql(
+                    self._static.dataset.c[self._runKeyColumn],
+                    sql_projection.joiner.from_clause,
+                )
+                need_static_table = True
+        # Ingest date can only come from the static table.
+        if "ingest_date" in fields:
+            fields_provided["ingest_date"] = self._static.dataset.c.ingest_date
+            need_static_table = True
+        if need_static_table:
+            # If we need the static table, join it in via dataset_id.  We don't
+            # use QueryJoiner.join because we're joining on dataset ID, not
+            # dimensions.
+            sql_projection.joiner.from_clause = sql_projection.joiner.from_clause.join(
+                self._static.dataset, onclause=(dataset_id_col == self._static.dataset.c.id)
+            )
+            # Also constrain dataset_type_id in static table in case that helps
+            # generate a better plan. We could also include this in the JOIN ON
+            # clause, but my guess is that that's a good idea IFF it's in the
+            # foreign key, and right now it isn't.
+            sql_projection.joiner.where(self._static.dataset.c.dataset_type_id == self._dataset_type_id)
+        sql_projection.distinct = (
+            # If there are multiple collections, this subquery might have
+            # non-unique rows.
+            len(collections) > 1
+            and not fields
+        )
+        return sql_projection
+
     def getDataId(self, id: DatasetId) -> DataCoordinate:
         """Return DataId for a dataset.
 
         Parameters
         ----------
         id : `DatasetId`
             Unique dataset identifier.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/summaries.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/datasets/byDimensions/tables.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/dimensions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/dimensions/static.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/dimensions/static.py`

 * *Files 11% similar despite different names*

```diff
@@ -26,42 +26,48 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 import dataclasses
 import itertools
 import logging
 from collections import defaultdict
-from collections.abc import Mapping, Sequence, Set
+from collections.abc import Iterable, Mapping, Sequence, Set
 from typing import TYPE_CHECKING, Any
 
 import sqlalchemy
 from lsst.daf.relation import Calculation, ColumnExpression, Join, Relation, sql
+from lsst.sphgeom import Region
 
 from ... import ddl
 from ..._column_tags import DimensionKeyColumnTag, DimensionRecordColumnTag
 from ..._column_type_info import LogicalColumn
 from ..._named import NamedKeyDict
 from ...dimensions import (
+    DatabaseDimensionElement,
     DatabaseTopologicalFamily,
     DataCoordinate,
     Dimension,
     DimensionElement,
     DimensionGroup,
     DimensionRecord,
     DimensionRecordSet,
     DimensionUniverse,
     SkyPixDimension,
     addDimensionForeignKey,
 )
 from ...dimensions.record_cache import DimensionRecordCache
+from ...direct_query_driver import QueryBuilder, QueryJoiner  # Future query system (direct,server).
+from ...queries import tree as qt  # Future query system (direct,client,server)
+from ...queries.overlaps import OverlapsVisitor
+from ...queries.visitors import PredicateVisitFlags
 from .._exceptions import MissingSpatialOverlapError
 from ..interfaces import Database, DimensionRecordStorageManager, StaticTablesContext, VersionTuple
 
 if TYPE_CHECKING:
-    from .. import queries
+    from .. import queries  # Current Registry.query* system.
 
 
 # This has to be updated on every schema change
 _VERSION = VersionTuple(6, 0, 2)
 
 _LOG = logging.getLogger(__name__)
 
@@ -148,14 +154,27 @@
             if not element.has_own_table:
                 continue
             spec = element.RecordClass.fields.makeTableSpec(TimespanReprClass=db.getTimespanRepresentation())
             tables[element.name] = context.addTable(element.name, spec)
             if element.spatial is not None:
                 spatial.setdefault(element.spatial, []).append(element)
                 overlap_tables[element.name] = cls._make_skypix_overlap_tables(context, element)
+            for field_name in spec.fields.names:
+                if (
+                    len(qt.ColumnSet.get_qualified_name(element.name, field_name))
+                    >= db.dialect.max_identifier_length
+                ):
+                    # Being able to assume that all dimension fields fit inside
+                    # the DB's identifier limit is really convenient and very
+                    # unlikely to cause trouble in practice.  We'll just make
+                    # sure we catch any such trouble as early as possible.
+                    raise RuntimeError(
+                        f"Dimension filed '{element.name}.{field_name}' is too long for this database. "
+                        "Please file a ticket for long-field support if this was not a mistake."
+                    )
         # Add some tables for materialized overlaps between database
         # dimensions.  We've never used these and no longer plan to, but we
         # have to keep creating them to keep schema versioning consistent.
         cls._make_legacy_overlap_tables(context, spatial)
         # Create tables that store DimensionGraph definitions.
         dimension_group_storage = _DimensionGroupStorage.initialize(db, context, universe=universe)
         return cls(
@@ -422,14 +441,48 @@
             # It's not obvious that's better than just telling the user to
             # materialize more overlaps, though.
             raise MissingSpatialOverlapError(
                 f"No materialized overlaps for spatial join between {element1!r} and {element2!r}."
             )
         return overlaps, needs_refinement
 
+    def make_query_joiner(self, element: DimensionElement, fields: Set[str]) -> QueryJoiner:
+        if element.implied_union_target is not None:
+            assert not fields, "Dimensions with implied-union storage never have fields."
+            return QueryBuilder(
+                self.make_query_joiner(element.implied_union_target, fields),
+                columns=qt.ColumnSet(element.minimal_group).drop_implied_dimension_keys(),
+                distinct=True,
+            ).to_joiner()
+        if not element.has_own_table:
+            raise NotImplementedError(f"Cannot join dimension element {element} with no table.")
+        table = self._tables[element.name]
+        result = QueryJoiner(self._db, table)
+        for dimension_name, column_name in zip(element.required.names, element.schema.required.names):
+            result.dimension_keys[dimension_name].append(table.columns[column_name])
+        result.extract_dimensions(element.implied.names)
+        for field in fields:
+            if field == "timespan":
+                result.timespans[element.name] = self._db.getTimespanRepresentation().from_columns(
+                    table.columns
+                )
+            else:
+                result.fields[element.name][field] = table.columns[field]
+        return result
+
+    def process_query_overlaps(
+        self,
+        dimensions: DimensionGroup,
+        predicate: qt.Predicate,
+        join_operands: Iterable[DimensionGroup],
+    ) -> tuple[qt.Predicate, QueryBuilder]:
+        overlaps_visitor = _CommonSkyPixMediatedOverlapsVisitor(self._db, dimensions, self._overlap_tables)
+        new_predicate = overlaps_visitor.run(predicate, join_operands)
+        return new_predicate, overlaps_visitor.builder
+
     def _make_relation(
         self,
         element: DimensionElement,
         context: queries.SqlQueryContext,
     ) -> Relation:
         table = self._tables[element.name]
         payload = sql.Payload[LogicalColumn](table)
@@ -944,7 +997,163 @@
             Retrieved graph.
         """
         graph = self._groupsByKey.get(key)
         if graph is None:
             self.refresh()
             graph = self._groupsByKey[key]
         return graph
+
+
+class _CommonSkyPixMediatedOverlapsVisitor(OverlapsVisitor):
+    def __init__(
+        self,
+        db: Database,
+        dimensions: DimensionGroup,
+        overlap_tables: Mapping[str, tuple[sqlalchemy.Table, sqlalchemy.Table]],
+    ):
+        super().__init__(dimensions)
+        self.builder: QueryBuilder = QueryJoiner(db).to_builder(qt.ColumnSet(dimensions))
+        self.common_skypix = dimensions.universe.commonSkyPix
+        self.overlap_tables: Mapping[str, tuple[sqlalchemy.Table, sqlalchemy.Table]] = overlap_tables
+        self.common_skypix_overlaps_done: set[DatabaseDimensionElement] = set()
+
+    def visit_spatial_constraint(
+        self,
+        element: DimensionElement,
+        region: Region,
+        flags: PredicateVisitFlags,
+    ) -> qt.Predicate | None:
+        # Reject spatial constraints that are nested inside OR or NOT, because
+        # the postprocessing needed for those would be a lot harder.
+        if flags & PredicateVisitFlags.INVERTED or flags & PredicateVisitFlags.HAS_OR_SIBLINGS:
+            raise NotImplementedError(
+                "Spatial overlap constraints nested inside OR or NOT are not supported."
+            )
+        # Delegate to super just because that's good practice with
+        # OverlapVisitor.
+        super().visit_spatial_constraint(element, region, flags)
+        match element:
+            case DatabaseDimensionElement():
+                # If this is a database dimension element like tract, patch, or
+                # visit, we need to:
+                # - join in the common skypix overlap table for this element;
+                # - constrain the common skypix index to be inside the
+                #   ranges that overlap the region as a SQL where clause;
+                # - add postprocessing to reject rows where the database
+                #   dimension element's region doesn't actually overlap the
+                #   region.
+                self.builder.postprocessing.spatial_where_filtering.append((element, region))
+                if self.common_skypix.name in self.dimensions:
+                    # The common skypix dimension should be part of the query
+                    # as a first-class dimension, so we can join in the overlap
+                    # table directly, and fall through to the end of this
+                    # function to construct a Predicate that will turn into the
+                    # SQL WHERE clause we want.
+                    self._join_common_skypix_overlap(element)
+                    skypix = self.common_skypix
+                else:
+                    # We need to hide the common skypix dimension from the
+                    # larger query, so we make a subquery out of the overlap
+                    # table that embeds the SQL WHERE clause we want and then
+                    # projects out that dimension (with SELECT DISTINCT, to
+                    # avoid introducing duplicate rows into the larger query).
+                    joiner = self._make_common_skypix_overlap_joiner(element)
+                    sql_where_or: list[sqlalchemy.ColumnElement[bool]] = []
+                    sql_skypix_col = joiner.dimension_keys[self.common_skypix.name][0]
+                    for begin, end in self.common_skypix.pixelization.envelope(region):
+                        sql_where_or.append(sqlalchemy.and_(sql_skypix_col >= begin, sql_skypix_col < end))
+                    joiner.where(sqlalchemy.or_(*sql_where_or))
+                    self.builder.join(
+                        joiner.to_builder(
+                            qt.ColumnSet(element.minimal_group).drop_implied_dimension_keys(), distinct=True
+                        ).to_joiner()
+                    )
+                    # Short circuit here since the SQL WHERE clause has already
+                    # been embedded in the subquery.
+                    return qt.Predicate.from_bool(True)
+            case SkyPixDimension():
+                # If this is a skypix dimension, we can do a index-in-ranges
+                # test directly on that dimension.  Note that this doesn't on
+                # its own guarantee the skypix dimension column will be in the
+                # query; that'll be the job of the DirectQueryDriver to sort
+                # out (generally this will require a dataset using that skypix
+                # dimension to be joined in, unless this is the common skypix
+                # system).
+                assert (
+                    element.name in self.dimensions
+                ), "QueryTree guarantees dimensions are expanded when constraints are added."
+                skypix = element
+            case _:
+                raise NotImplementedError(
+                    f"Spatial overlap constraint for dimension {element} not supported."
+                )
+        # Convert the region-overlap constraint into a skypix
+        # index range-membership constraint in SQL.
+        result = qt.Predicate.from_bool(False)
+        skypix_col_ref = qt.DimensionKeyReference.model_construct(dimension=skypix)
+        for begin, end in skypix.pixelization.envelope(region):
+            result = result.logical_or(qt.Predicate.in_range(skypix_col_ref, start=begin, stop=end))
+        return result
+
+    def visit_spatial_join(
+        self, a: DimensionElement, b: DimensionElement, flags: PredicateVisitFlags
+    ) -> qt.Predicate | None:
+        # Reject spatial joins that are nested inside OR or NOT, because the
+        # postprocessing needed for those would be a lot harder.
+        if flags & PredicateVisitFlags.INVERTED or flags & PredicateVisitFlags.HAS_OR_SIBLINGS:
+            raise NotImplementedError("Spatial overlap joins nested inside OR or NOT are not supported.")
+        # Delegate to super to check for invalid joins and record this
+        # "connection" for use when seeing whether to add an automatic join
+        # later.
+        super().visit_spatial_join(a, b, flags)
+        match (a, b):
+            case (self.common_skypix, DatabaseDimensionElement() as b):
+                self._join_common_skypix_overlap(b)
+            case (DatabaseDimensionElement() as a, self.common_skypix):
+                self._join_common_skypix_overlap(a)
+            case (DatabaseDimensionElement() as a, DatabaseDimensionElement() as b):
+                if self.common_skypix.name in self.dimensions:
+                    # We want the common skypix dimension to appear in the
+                    # query as a first-class dimension, so just join in the
+                    # two overlap tables directly.
+                    self._join_common_skypix_overlap(a)
+                    self._join_common_skypix_overlap(b)
+                else:
+                    # We do not want the common skypix system to appear in the
+                    # query or cause duplicate rows, so we join the two overlap
+                    # tables in a subquery that projects out the common skypix
+                    # index column with SELECT DISTINCT.
+
+                    self.builder.join(
+                        self._make_common_skypix_overlap_joiner(a)
+                        .join(self._make_common_skypix_overlap_joiner(b))
+                        .to_builder(
+                            qt.ColumnSet(a.minimal_group | b.minimal_group).drop_implied_dimension_keys(),
+                            distinct=True,
+                        )
+                        .to_joiner()
+                    )
+                # In both cases we add postprocessing to check that the regions
+                # really do overlap, since overlapping the same common skypix
+                # tile is necessary but not sufficient for that.
+                self.builder.postprocessing.spatial_join_filtering.append((a, b))
+            case _:
+                raise NotImplementedError(f"Unsupported combination for spatial join: {a, b}.")
+        return qt.Predicate.from_bool(True)
+
+    def _join_common_skypix_overlap(self, element: DatabaseDimensionElement) -> None:
+        if element not in self.common_skypix_overlaps_done:
+            self.builder.join(self._make_common_skypix_overlap_joiner(element))
+            self.common_skypix_overlaps_done.add(element)
+
+    def _make_common_skypix_overlap_joiner(self, element: DatabaseDimensionElement) -> QueryJoiner:
+        _, overlap_table = self.overlap_tables[element.name]
+        return (
+            QueryJoiner(self.builder.joiner.db, overlap_table)
+            .extract_dimensions(element.required.names, skypix_index=self.common_skypix.name)
+            .where(
+                sqlalchemy.and_(
+                    overlap_table.c.skypix_system == self.common_skypix.system.name,
+                    overlap_table.c.skypix_level == self.common_skypix.level,
+                )
+            )
+        )
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_attributes.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_attributes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_bridge.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_bridge.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_collections.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_collections.py`

 * *Files 20% similar despite different names*

```diff
@@ -35,14 +35,16 @@
     "RunRecord",
 ]
 
 from abc import abstractmethod
 from collections.abc import Iterable, Set
 from typing import TYPE_CHECKING, Any, Generic, Self, TypeVar
 
+import sqlalchemy
+
 from ..._timespan import Timespan
 from .._collection_type import CollectionType
 from ..wildcards import CollectionWildcard
 from ._versioning import VersionedExtension, VersionTuple
 
 if TYPE_CHECKING:
     from .._caching_context import CachingContext
@@ -602,22 +604,170 @@
         names : `set` [`str`]
             Parent collection names.
         """
         raise NotImplementedError()
 
     @abstractmethod
     def update_chain(
-        self, record: ChainedCollectionRecord[_Key], children: Iterable[str], flatten: bool = False
-    ) -> ChainedCollectionRecord[_Key]:
-        """Update chained collection composition.
+        self,
+        parent_collection_name: str,
+        child_collection_names: list[str],
+        allow_use_in_caching_context: bool = False,
+    ) -> None:
+        """Replace all of the children in a chained collection with a new list.
+
+        Parameters
+        ----------
+        parent_collection_name : `str`
+            The name of a CHAINED collection to be modified.
+        child_collection_names : `list` [ `str ` ]
+            A child collection name or list of child collection names to be
+            assigned to the parent.
+        allow_use_in_caching_context : `bool`, optional
+            If `True`, skip a check that would otherwise disallow this function
+            from being called inside an active caching context.
+            (Only exists for legacy use, will eventually be removed).
+
+        Raises
+        ------
+        MissingCollectionError
+            If any of the specified collections do not exist.
+        CollectionTypeError
+            If the parent collection is not a CHAINED collection.
+        CollectionCycleError
+            If this operation would create a collection cycle.
+
+        Notes
+        -----
+        If this function is called within a call to ``Butler.transaction``, it
+        will hold a lock that prevents other processes from modifying the
+        parent collection until the end of the transaction.  Keep these
+        transactions short.
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
+    def prepend_collection_chain(
+        self, parent_collection_name: str, child_collection_names: list[str]
+    ) -> None:
+        """Add children to the beginning of a CHAINED collection.
+
+        If any of the children already existed in the chain, they will be moved
+        to the new position at the beginning of the chain.
+
+        Parameters
+        ----------
+        parent_collection_name : `str`
+            The name of a CHAINED collection to which we will add new children.
+        child_collection_names : `list` [ `str ` ]
+            A child collection name or list of child collection names to be
+            added to the parent.
+
+        Raises
+        ------
+        MissingCollectionError
+            If any of the specified collections do not exist.
+        CollectionTypeError
+            If the parent collection is not a CHAINED collection.
+        CollectionCycleError
+            If this operation would create a collection cycle.
+
+        Notes
+        -----
+        If this function is called within a call to ``Butler.transaction``, it
+        will hold a lock that prevents other processes from modifying the
+        parent collection until the end of the transaction.  Keep these
+        transactions short.
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
+    def extend_collection_chain(self, parent_collection_name: str, child_collection_names: list[str]) -> None:
+        """Add children to the end of a CHAINED collection.
+
+        If any of the children already existed in the chain, they will be moved
+        to the new position at the end of the chain.
 
         Parameters
         ----------
-        record : `ChainedCollectionRecord`
-            Chained collection record.
-        children : `~collections.abc.Iterable` [`str`]
-            Ordered names of children collections.
-        flatten : `bool`, optional
-            If `True`, recursively flatten out any nested
-            `~CollectionType.CHAINED` collections in ``children`` first.
+        parent_collection_name : `str`
+            The name of a CHAINED collection to which we will add new children.
+        child_collection_names : `list` [ `str ` ]
+            A child collection name or list of child collection names to be
+            added to the parent.
+
+        Raises
+        ------
+        MissingCollectionError
+            If any of the specified collections do not exist.
+        CollectionTypeError
+            If the parent collection is not a CHAINED collection.
+        CollectionCycleError
+            If this operation would create a collection cycle.
+
+        Notes
+        -----
+        If this function is called within a call to ``Butler.transaction``, it
+        will hold a lock that prevents other processes from modifying the
+        parent collection until the end of the transaction.  Keep these
+        transactions short.
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
+    def remove_from_collection_chain(
+        self, parent_collection_name: str, child_collection_names: list[str]
+    ) -> None:
+        """Remove children from a CHAINED collection.
+
+        Parameters
+        ----------
+        parent_collection_name : `str`
+            The name of a CHAINED collection from which we will remove
+            children.
+        child_collection_names : `list` [ `str ` ]
+            A child collection name or list of child collection names to be
+            removed from the parent.
+
+        Raises
+        ------
+        MissingCollectionError
+            If any of the specified collections do not exist.
+        CollectionTypeError
+            If the parent collection is not a CHAINED collection.
+
+        Notes
+        -----
+        If this function is called within a call to ``Butler.transaction``, it
+        will hold a lock that prevents other processes from modifying the
+        parent collection until the end of the transaction.  Keep these
+        transactions short.
+        """
+        raise NotImplementedError()
+
+    def lookup_name_sql(
+        self, sql_key: sqlalchemy.ColumnElement[_Key], sql_from_clause: sqlalchemy.FromClause
+    ) -> tuple[sqlalchemy.ColumnElement[str], sqlalchemy.FromClause]:
+        """Return a SQLAlchemy column and FROM clause that enable a query
+        to look up a collection name from the key.
+
+        Parameters
+        ----------
+        sql_key : `sqlalchemy.ColumnElement`
+            SQL column expression that evaluates to the collection key.
+        sql_from_clause : `sqlalchemy.FromClause`
+            SQL FROM clause from which ``sql_key`` was obtained.
+
+        Returns
+        -------
+        sql_name : `sqlalchemy.ColumnElement` [ `str` ]
+            SQL column expression that evalutes to the collection name.
+        sql_from_clause : `sqlalchemy.FromClause`
+            SQL FROM clause that includes the given ``sql_from_clause`` and
+            any table needed to provided ``sql_name``.
         """
         raise NotImplementedError()
+
+    def _block_for_concurrency_test(self) -> None:
+        """No-op normally. Provide a place for unit tests to hook in and
+        verify locking behavior.
+        """
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_database.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_database.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,15 +460,15 @@
     ) -> Iterator[None]:
         """Return a context manager that represents a transaction.
 
         Parameters
         ----------
         interrupting : `bool`, optional
             If `True` (`False` is default), this transaction block may not be
-            nested without an outer one, and attempting to do so is a logic
+            nested within an outer one, and attempting to do so is a logic
             (i.e. assertion) error.
         savepoint : `bool`, optional
             If `True` (`False` is default), create a `SAVEPOINT`, allowing
             exceptions raised by the database (e.g. due to constraint
             violations) during this transaction's context to be caught outside
             it without also rolling back all operations in an outer transaction
             block.  If `False`, transactions may still be nested, but a
@@ -628,15 +628,15 @@
             an exception.  When entered, it returns a tuple of:
 
             - ``is_new`` (`bool`): whether this is a new (outermost)
               transaction;
             - ``connection`` (`sqlalchemy.engine.Connection`): the connection.
         """
         with self._session() as connection:
-            already_in_transaction = connection.in_transaction()
+            already_in_transaction = self.isInTransaction()
             assert not (interrupting and already_in_transaction), (
                 "Logic error in transaction nesting: an operation that would "
                 "interrupt the active transaction context has been requested."
             )
             savepoint = savepoint or connection.in_nested_transaction()
             trans: sqlalchemy.engine.Transaction | None
             if already_in_transaction:
@@ -790,14 +790,21 @@
             raise
 
     @abstractmethod
     def isWriteable(self) -> bool:
         """Return `True` if this database can be modified by this client."""
         raise NotImplementedError()
 
+    def isInTransaction(self) -> bool:
+        """Return `True` if there is currently a database connection open with
+        an active transaction; `False` otherwise.
+        """
+        session = self._session_connection
+        return session is not None and session.in_transaction()
+
     @abstractmethod
     def __str__(self) -> str:
         """Return a human-readable identifier for this `Database`, including
         any namespace or schema that identifies its names within a `Registry`.
         """
         raise NotImplementedError()
 
@@ -1116,17 +1123,15 @@
         read-only databases if and only if the table does in fact already
         exist.
 
         Subclasses may override this method, but usually should not need to.
         """
         # TODO: if _engine is used to make a table then it uses separate
         # connection and should not interfere with current transaction
-        assert (
-            self._session_connection is None or not self._session_connection.in_transaction()
-        ), "Table creation interrupts transactions."
+        assert not self.isInTransaction(), "Table creation interrupts transactions."
         assert self._metadata is not None, "Static tables must be declared before dynamic tables."
         table = self.getExistingTable(name, spec)
         if table is not None:
             return table
         if not self.isWriteable():
             raise ReadOnlyDatabaseError(
                 f"Table {name} does not exist, and cannot be created because database {self} is read-only."
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_datasets.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_datasets.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,30 +28,31 @@
 from __future__ import annotations
 
 from ... import ddl
 
 __all__ = ("DatasetRecordStorageManager", "DatasetRecordStorage")
 
 from abc import ABC, abstractmethod
-from collections.abc import Iterable, Iterator, Mapping, Set
+from collections.abc import Iterable, Iterator, Mapping, Sequence, Set
 from typing import TYPE_CHECKING, Any
 
 from lsst.daf.relation import Relation
 
 from ..._dataset_ref import DatasetId, DatasetIdGenEnum, DatasetRef
 from ..._dataset_type import DatasetType
+from ..._exceptions import MissingDatasetTypeError
 from ..._timespan import Timespan
 from ...dimensions import DataCoordinate
-from .._exceptions import MissingDatasetTypeError
 from ._versioning import VersionedExtension, VersionTuple
 
 if TYPE_CHECKING:
+    from ...direct_query_driver import QueryJoiner  # new query system, server+direct only
     from .._caching_context import CachingContext
     from .._collection_summary import CollectionSummary
-    from ..queries import SqlQueryContext
+    from ..queries import SqlQueryContext  # old registry query system
     from ._collections import CollectionManager, CollectionRecord, RunRecord
     from ._database import Database, StaticTablesContext
     from ._dimensions import DimensionRecordStorageManager
 
 
 class DatasetRecordStorage(ABC):
     """An interface that manages the records associated with a particular
@@ -307,14 +308,46 @@
         Returns
         -------
         relation : `~lsst.daf.relation.Relation`
             Representation of the query.
         """
         raise NotImplementedError()
 
+    @abstractmethod
+    def make_query_joiner(self, collections: Sequence[CollectionRecord], fields: Set[str]) -> QueryJoiner:
+        """Make a `..direct_query_driver.QueryJoiner` that represents a search
+        for datasets of this type.
+
+        Parameters
+        ----------
+        collections : `~collections.abc.Sequence` [ `CollectionRecord` ]
+            Collections to search, in order, after filtering out collections
+            with no datasets of this type via collection summaries.
+        fields : `~collections.abc.Set` [ `str` ]
+            Names of fields to make available in the joiner.  Options include:
+
+            - ``dataset_id`` (UUID)
+            - ``run` (collection name, `str`)
+            - ``collection`` (collection name, `str`)
+            - ``collection_key`` (collection primary key, manager-dependent)
+            - ``timespan`` (validity range, or unbounded for non-calibrations)
+            - ``ingest_date`` (time dataset was ingested into repository)
+
+            Dimension keys for the dataset type's required dimensions are
+            always included.
+
+        Returns
+        -------
+        joiner : `..direct_query_driver.QueryJoiner`
+            A query-construction object representing a table or subquery.  If
+            ``fields`` is empty or ``len(collections) <= 1``, this is
+            guaranteed to have rows that are unique over dimension keys.
+        """
+        raise NotImplementedError()
+
     datasetType: DatasetType
     """Dataset type whose records this object manages (`DatasetType`).
     """
 
 
 class DatasetRecordStorageManager(VersionedExtension):
     """An interface that manages the tables that describe datasets.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_dimensions.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_dimensions.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ("DimensionRecordStorageManager",)
 
 from abc import abstractmethod
-from collections.abc import Set
+from collections.abc import Iterable, Set
 from typing import TYPE_CHECKING, Any
 
 from lsst.daf.relation import Join, Relation
 
 from ...dimensions import (
     DataCoordinate,
     DimensionElement,
@@ -42,15 +42,17 @@
     DimensionRecordSet,
     DimensionUniverse,
 )
 from ...dimensions.record_cache import DimensionRecordCache
 from ._versioning import VersionedExtension, VersionTuple
 
 if TYPE_CHECKING:
-    from .. import queries
+    from ...direct_query_driver import QueryBuilder, QueryJoiner  # Future query system (direct,server).
+    from ...queries.tree import Predicate  # Future query system (direct,client,server).
+    from .. import queries  # Old Registry.query* system.
     from ._database import Database, StaticTablesContext
 
 
 class DimensionRecordStorageManager(VersionedExtension):
     """An interface for managing the dimension records in a `Registry`.
 
     `DimensionRecordStorageManager` primarily serves as a container and factory
@@ -353,11 +355,85 @@
             dimensions of both elements.
         needs_refinement : `bool`
             Whether the returned relation represents a conservative join that
             needs refinement via native-iteration predicate.
         """
         raise NotImplementedError()
 
+    @abstractmethod
+    def make_query_joiner(self, element: DimensionElement, fields: Set[str]) -> QueryJoiner:
+        """Make a `..direct_query_driver.QueryJoiner` that represents a
+        dimension element table.
+
+        Parameters
+        ----------
+        element : `DimensionElement`
+            Dimension element the table corresponds to.
+        fields : `~collections.abc.Set` [ `str` ]
+            Names of fields to make available in the joiner.  These can be any
+            metadata or alternate key field in the element's schema, including
+            the special ``region`` and ``timespan`` fields. Dimension keys in
+            the element's schema are always included.
+
+        Returns
+        -------
+        joiner : `..direct_query_driver.QueryJoiner`
+            A query-construction object representing a table or subquery.  This
+            is guaranteed to have rows that are unique over dimension keys and
+            all possible key values for this dimension, so joining in a
+            dimension element table:
+
+             - never introduces duplicates into the query's result rows;
+             - never restricts the query's rows *except* to ensure
+               required-implied relationships are followed.
+        """
+        raise NotImplementedError()
+
+    @abstractmethod
+    def process_query_overlaps(
+        self,
+        dimensions: DimensionGroup,
+        predicate: Predicate,
+        join_operands: Iterable[DimensionGroup],
+    ) -> tuple[Predicate, QueryBuilder]:
+        """Process a query's WHERE predicate and dimensions to handle spatial
+        and temporal overlaps.
+
+        Parameters
+        ----------
+        dimensions : `..dimensions.DimensionGroup`
+            Full dimensions of all tables to be joined into the query (even if
+            they are not included in the query results).
+        predicate : `..queries.tree.Predicate`
+            Boolean column expression that may contain user-provided  spatial
+            and/or temporal overlaps intermixed with other constraints.
+        join_operands : `~collections.abc.Iterable` [ \
+                `..dimensions.DimensionGroup` ]
+            Dimensions of tables or subqueries that are already going to be
+            joined into the query that may establish their own spatial or
+            temporal relationships (e.g. a dataset search with both ``visit``
+            and ``patch`` dimensions).
+
+        Returns
+        -------
+        predicate : `..queries.tree.Predicate`
+            A version of the given predicate that preserves the overall
+            behavior of the filter while possibly rewriting overlap expressions
+            that have been partially moved into ``builder`` as some combination
+            of new nested predicates, joins, and postprocessing.
+        builder : `..direct_query_driver.QueryBuilder`
+            A query-construction helper object that includes any initial joins
+            and postprocessing needed to handle overlap expression extracted
+            from the original predicate.
+
+        Notes
+        -----
+        Implementations must delegate to `.queries.overlaps.OverlapsVisitor`
+        (possibly by subclassing it) to ensure "automatic" spatial and temporal
+        joins are added consistently by all query-construction implementations.
+        """
+        raise NotImplementedError()
+
     universe: DimensionUniverse
     """Universe of all dimensions and dimension elements known to the
     `Registry` (`DimensionUniverse`).
     """
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_obscore.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_obscore.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_opaque.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_opaque.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/interfaces/_versioning.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/interfaces/_versioning.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/managers.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/managers.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/nameShrinker.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/name_shrinker.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ["NameShrinker"]
 
 import hashlib
+from collections.abc import Iterator
 
 
 class NameShrinker:
     """A utility class for `Database` implementations that need a nontrivial
     implementation of `Database.shrinkDatabaseEntityName` and
     `Database.expandDatabaseEntityName`.
 
@@ -93,7 +94,24 @@
         Returns
         -------
         expanded : `str`
             The expanded form. If the given name was not passed to `shrink`
             or was not modified by it, it is returned unmodified.
         """
         return self._by_shrunk.get(shrunk, shrunk)
+
+    def __iter__(self) -> Iterator[tuple[str, str]]:
+        return iter(self._by_original.items())
+
+    def __len__(self) -> int:
+        return len(self._by_original)
+
+    def update(self, other: NameShrinker) -> None:
+        """Add all original <-> shrunk mappings from ``other`` to ``self``.
+
+        Parameters
+        ----------
+        other : `NameShrinker`
+            Object to extract name mappings from.
+        """
+        self._by_original.update(other._by_original)
+        self._by_shrunk.update(other._by_shrunk)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_config.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_manager.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_manager.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_records.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_records.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_schema.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_schema.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/_spatial.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/default_spatial.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/default_spatial.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/obscore/pgsphere.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/obscore/pgsphere.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/opaque.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/opaque.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_builder.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_builder.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_query.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_backend.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_query_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,17 +44,18 @@
     Predicate,
     Relation,
     UnaryOperationRelation,
 )
 
 from ..._column_tags import DatasetColumnTag, DimensionKeyColumnTag
 from ..._dataset_type import DatasetType
+from ..._exceptions import MissingDatasetTypeError
+from ..._exceptions_legacy import DatasetTypeError
 from ...dimensions import DimensionGroup, DimensionRecordSet, DimensionUniverse
 from .._collection_type import CollectionType
-from .._exceptions import DatasetTypeError, MissingDatasetTypeError
 from ..wildcards import CollectionWildcard
 from ._query_context import QueryContext
 from .find_first_dataset import FindFirstDataset
 
 if TYPE_CHECKING:
     from ..interfaces import CollectionRecord
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_query_context.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_query_context.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_readers.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_readers.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_results.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_results.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,23 +41,23 @@
 from contextlib import AbstractContextManager, ExitStack, contextmanager
 from typing import Any
 
 from deprecated.sphinx import deprecated
 
 from ..._dataset_ref import DatasetRef
 from ..._dataset_type import DatasetType
+from ..._exceptions_legacy import DatasetTypeError
 from ...dimensions import (
     DataCoordinate,
     DataCoordinateIterable,
     DimensionElement,
     DimensionGraph,
     DimensionGroup,
     DimensionRecord,
 )
-from .._exceptions import DatasetTypeError
 from ._query import Query
 from ._structs import OrderByClause
 
 
 class DataCoordinateQueryResults(DataCoordinateIterable):
     """An enhanced implementation of `DataCoordinateIterable` that represents
     data IDs retrieved from a database query.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_backend.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_sql_query_backend.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_sql_query_context.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_sql_query_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,16 +51,16 @@
     UnaryOperationRelation,
     iteration,
     sql,
 )
 
 from ..._column_tags import is_timespan_column
 from ..._column_type_info import ColumnTypeInfo, LogicalColumn
+from ...name_shrinker import NameShrinker
 from ...timespan_database_representation import TimespanDatabaseRepresentation
-from ..nameShrinker import NameShrinker
 from ._query_context import QueryContext
 from .butler_sql_engine import ButlerSqlEngine
 
 if TYPE_CHECKING:
     from ..interfaces import Database
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/_structs.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/_structs.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,16 +221,16 @@
         for name in order_by:
             if not name or name == "-":
                 raise ValueError("Empty dimension name in ORDER BY")
             ascending = True
             if name[0] == "-":
                 ascending = False
                 name = name[1:]
-            column = categorizeElementOrderByName(element, name)
-            term = cls._make_term(element, column, ascending)
+            found_element, column = categorizeElementOrderByName(element, name)
+            term = cls._make_term(found_element, column, ascending)
             terms.append(term)
         return cls(terms)
 
     @classmethod
     def _make_term(cls, element: DimensionElement, column: str | None, ascending: bool) -> SortTerm:
         """Make a single sort term from parsed user expression values.
 
@@ -299,17 +299,17 @@
         for name in order_by:
             if not name or name == "-":
                 raise ValueError("Empty dimension name in ORDER BY")
             ascending = True
             if name[0] == "-":
                 ascending = False
                 name = name[1:]
-            column = categorizeElementOrderByName(element, name)
+            found_element, column = categorizeElementOrderByName(element, name)
             self.order_by_columns.append(
-                OrderByClauseColumn(element=element, column=column, ordering=ascending)
+                OrderByClauseColumn(element=found_element, column=column, ordering=ascending)
             )
 
     order_by_columns: Iterable[OrderByClauseColumn]
     """Columns that appear in the ORDER BY
     (`~collections.abc.Iterable` [ `OrderByClauseColumn` ]).
     """
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/butler_sql_engine.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/butler_sql_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 import astropy.time
 import sqlalchemy
 from lsst.daf.relation import ColumnTag, Relation, Sort, UnaryOperation, UnaryOperationRelation, sql
 
 from ..._column_tags import is_timespan_column
 from ..._column_type_info import ColumnTypeInfo, LogicalColumn
 from ..._timespan import Timespan
+from ...name_shrinker import NameShrinker
 from ...timespan_database_representation import TimespanDatabaseRepresentation
-from ..nameShrinker import NameShrinker
 from .find_first_dataset import FindFirstDataset
 
 
 @dataclasses.dataclass(repr=False, eq=False, kw_only=True)
 class ButlerSqlEngine(sql.Engine[LogicalColumn]):
     """An extension of the `lsst.daf.relation.sql.Engine` class to add timespan
     and `FindFirstDataset` operation support.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/_predicate.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/_predicate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/categorize.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/categorize.py`

 * *Files 6% similar despite different names*

```diff
@@ -108,24 +108,16 @@
         if isinstance(element, Dimension) and column == element.primaryKey.name:
             # Allow e.g. "visit.id = x" instead of just "visit = x"; this
             # can be clearer.
             return element, None
         elif column in element.dimensions.names:
             # User said something like "patch.tract = x" or
             # "tract.tract = x" instead of just "tract = x" or
-            # "tract.id = x", which is at least needlessly confusing and
-            # possibly not actually a column name, though we can guess
-            # what they were trying to do.
-            # Encourage them to clean that up and try again.
-            name = universe[column].primaryKey.name  # type: ignore
-            raise RuntimeError(
-                f"Invalid reference to '{table}.{column}' "
-                f"in expression; please use '{column}' or "
-                f"'{column}.{name}' instead."
-            )
+            # "tract.id = x". Return the column as the element instead.
+            return element.dimensions[column], None
         else:
             return element, column
     else:
         try:
             dimension = universe[table]
         except KeyError as err:
             raise LookupError(f"No dimension with name '{table}'.") from err
@@ -237,36 +229,42 @@
         element = dimensions.universe[elem_name]
         if field_name in ("timespan.begin", "timespan.end"):
             if not element.temporal:
                 raise ValueError(f"Cannot use '{field_name}' with non-temporal element '{element}'.")
         elif isinstance(element, Dimension) and field_name == element.primaryKey.name:
             # Primary key is optional
             field_name = None
+        elif field_name in element.dimensions.names:
+            # Something like visit.physical_filter, which which want to remap
+            # to just "physical_filter".
+            return dimensions.universe[field_name], None
         else:
             if not (
                 field_name in element.metadata.names
                 or (isinstance(element, Dimension) and field_name in element.alternateKeys.names)
             ):
                 raise ValueError(f"Field '{field_name}' does not exist in '{element}'.")
 
     return element, field_name
 
 
-def categorizeElementOrderByName(element: DimensionElement, name: str) -> str | None:
+def categorizeElementOrderByName(element: DimensionElement, name: str) -> tuple[DimensionElement, str | None]:
     """Categorize an identifier in an ORDER BY clause for a single element.
 
     Parameters
     ----------
     element : `DimensionElement`
         Dimension element.
     name : `str`
         Identifier to categorize.
 
     Returns
     -------
+    element : `DimensionElement`
+        The `DimensionElement` the identifier refers to.
     column : `str` or `None`
         The name of a column in the table for ``element``, or `None` if
         ``element`` is a `Dimension` and the requested column is its primary
         key.
 
     Raises
     ------
@@ -296,25 +294,29 @@
     elif "." not in name:
         # No dot, can be either a dimension name or a field name (in any of
         # the known elements)
         if name == element.name:
             # Must be a dimension element
             if not isinstance(element, Dimension):
                 raise ValueError(f"Element '{element}' is not a dimension.")
+        elif name in element.dimensions.names and name != element.name:
+            # Something like visit.physical_filter, which which want to remap
+            # to just "physical_filter".
+            return element.universe[name], None
         else:
             # Can be a metadata name or any of the keys, but primary key needs
             # to be treated the same as a reference to the dimension name
             # itself.
             if isinstance(element, Dimension):
                 if name == element.primaryKey.name:
-                    return None
+                    return element, None
                 elif name in element.uniqueKeys.names:
-                    return name
+                    return element, name
             if name in element.metadata.names:
-                return name
+                return element, name
             raise ValueError(f"Field '{name}' does not exist in '{element}'.")
     else:
         # qualified name, must be a dimension element and a field
         elem_name, _, field_name = name.partition(".")
         if elem_name != element.name:
             if field_name == "begin" or field_name == "end":
                 extra = f"; perhaps you meant 'timespan.{field_name}'?"
@@ -330,8 +332,8 @@
         else:
             if not (
                 field_name in element.metadata.names
                 or (isinstance(element, Dimension) and field_name in element.alternateKeys.names)
             ):
                 raise ValueError(f"Field '{field_name}' does not exist in '{element}'.")
 
-    return field_name
+    return element, field_name
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/check.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/check.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/normalForm.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/normalForm.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/exprTree.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/parserLex.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/parserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/ply/lex.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/ply/yacc.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/expressions/parser/treeVisitor.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/queries/find_first_dataset.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/queries/find_first_dataset.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/sql_registry.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/sql_registry.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from lsst.utils.iteration import ensure_iterable
 
 from .._column_tags import DatasetColumnTag
 from .._config import Config
 from .._dataset_association import DatasetAssociation
 from .._dataset_ref import DatasetId, DatasetIdGenEnum, DatasetRef
 from .._dataset_type import DatasetType
+from .._exceptions import CalibrationLookupError, DimensionNameError
 from .._named import NamedKeyMapping, NameLookupMapping
 from .._storage_class import StorageClassFactory
 from .._timespan import Timespan
 from ..dimensions import (
     DataCoordinate,
     DataId,
     Dimension,
@@ -69,15 +70,14 @@
     CollectionExpressionError,
     CollectionSummary,
     CollectionType,
     CollectionTypeError,
     ConflictingDefinitionError,
     DataIdValueError,
     DatasetTypeError,
-    DimensionNameError,
     InconsistentDataIdError,
     MissingDatasetTypeError,
     NoDefaultCollectionError,
     OrphanedRecordError,
     RegistryConfig,
     RegistryConsistencyError,
     RegistryDefaults,
@@ -490,15 +490,15 @@
         Raises
         ------
         lsst.daf.butler.registry.MissingCollectionError
             Raised if no collection with the given name exists.
         """
         return self._managers.collections.find(name).type
 
-    def _get_collection_record(self, name: str) -> CollectionRecord:
+    def get_collection_record(self, name: str) -> CollectionRecord:
         """Return the record for this collection.
 
         Parameters
         ----------
         name : `str`
             Name of the collection for which the record is to be retrieved.
 
@@ -617,24 +617,29 @@
         ------
         lsst.daf.butler.registry.MissingCollectionError
             Raised when any of the given collections do not exist in the
             `Registry`.
         lsst.daf.butler.registry.CollectionTypeError
             Raised if ``parent`` does not correspond to a
             `~CollectionType.CHAINED` collection.
-        ValueError
+        CollectionCycleError
             Raised if the given collections contains a cycle.
+
+        Notes
+        -----
+        If this function is called within a call to ``Butler.transaction``, it
+        will hold a lock that prevents other processes from modifying the
+        parent collection until the end of the transaction.  Keep these
+        transactions short.
         """
-        record = self._managers.collections.find(parent)
-        if record.type is not CollectionType.CHAINED:
-            raise CollectionTypeError(f"Collection '{parent}' has type {record.type.name}, not CHAINED.")
-        assert isinstance(record, ChainedCollectionRecord)
         children = CollectionWildcard.from_expression(children).require_ordered()
-        if children != record.children or flatten:
-            self._managers.collections.update_chain(record, children, flatten=flatten)
+        if flatten:
+            children = self.queryCollections(children, flattenChains=True)
+
+        self._managers.collections.update_chain(parent, list(children), allow_use_in_caching_context=True)
 
     def getCollectionParentChains(self, collection: str) -> set[str]:
         """Return the CHAINED collections that directly contain the given one.
 
         Parameters
         ----------
         collection : `str`
@@ -959,15 +964,15 @@
                         best_row = row
                         best_rank = rank
                         have_tie = False
                     elif rank == best_rank:
                         have_tie = True
                         assert timespan is not None, "Rank ties should be impossible given DB constraints."
                 if have_tie:
-                    raise LookupError(
+                    raise CalibrationLookupError(
                         f"Ambiguous calibration lookup for {resolved_dataset_type.name} in collections "
                         f"{collection_wildcard.strings} with timespan {timespan}."
                     )
             reader = queries.DatasetRefReader(
                 resolved_dataset_type,
                 translate_collection=lambda k: self._managers.collections[k].name,
             )
@@ -1527,27 +1532,22 @@
         dimension key values that are given by the caller) may be constructed
         directly rather than obtained from the registry database.
         """
         if not withDefaults:
             defaults = None
         else:
             defaults = self.defaults.dataId
-        try:
-            standardized = DataCoordinate.standardize(
-                dataId,
-                graph=graph,
-                dimensions=dimensions,
-                universe=self.dimensions,
-                defaults=defaults,
-                **kwargs,
-            )
-        except KeyError as exc:
-            # This means either kwargs have some odd name or required
-            # dimension is missing.
-            raise DimensionNameError(str(exc)) from exc
+        standardized = DataCoordinate.standardize(
+            dataId,
+            graph=graph,
+            dimensions=dimensions,
+            universe=self.dimensions,
+            defaults=defaults,
+            **kwargs,
+        )
         if standardized.hasRecords():
             return standardized
         if records is None:
             records = {}
         elif isinstance(records, NamedKeyMapping):
             records = records.byName()
         else:
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_database.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/_database.py`

 * *Files 0% similar despite different names*

```diff
@@ -1253,15 +1253,15 @@
                     ]
                     + list(db.getTimespanRepresentation().makeFieldSpecs(nullable=True)),
                 ),
             )
         pixelization = Mq3cPixelization(10)
         start = astropy.time.Time("2020-01-01T00:00:00", format="isot", scale="tai")
         offset = astropy.time.TimeDelta(60, format="sec")
-        timespans = [Timespan(begin=start + offset * n, end=start + offset * n + 1) for n in range(3)]
+        timespans = [Timespan(begin=start + offset * n, end=start + offset * (n + 1)) for n in range(3)]
         ts_cls = db.getTimespanRepresentation()
         ts_col = ts_cls.from_columns(t.columns)
         db.insert(
             t,
             ts_cls.update(timespans[0], result={"id": 1, "name": "a", "region": pixelization.quad(12058870)}),
             ts_cls.update(timespans[1], result={"id": 2, "name": "a", "region": pixelization.quad(12058871)}),
             ts_cls.update(timespans[2], result={"id": 3, "name": "b", "region": pixelization.quad(12058872)}),
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/tests/_registry.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/tests/_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,21 +30,23 @@
 
 __all__ = ["RegistryTests"]
 
 import datetime
 import itertools
 import os
 import re
+import time
 import unittest
 import uuid
 from abc import ABC, abstractmethod
 from collections import defaultdict, namedtuple
-from collections.abc import Iterator
+from collections.abc import Callable, Iterator
+from concurrent.futures import ThreadPoolExecutor
 from datetime import timedelta
-from typing import TYPE_CHECKING
+from threading import Barrier
 
 import astropy.time
 import sqlalchemy
 
 try:
     import numpy as np
 except ImportError:
@@ -52,39 +54,35 @@
 
 import lsst.sphgeom
 from lsst.daf.relation import Relation, RelationalAlgebraError, Transfer, iteration, sql
 
 from ..._dataset_association import DatasetAssociation
 from ..._dataset_ref import DatasetIdFactory, DatasetIdGenEnum, DatasetRef
 from ..._dataset_type import DatasetType
+from ..._exceptions import CollectionTypeError, MissingCollectionError, MissingDatasetTypeError
+from ..._exceptions_legacy import DatasetTypeError
 from ..._storage_class import StorageClass
 from ..._timespan import Timespan
 from ...dimensions import DataCoordinate, DataCoordinateSet, SkyPixDimension
 from .._collection_summary import CollectionSummary
 from .._collection_type import CollectionType
 from .._config import RegistryConfig
 from .._exceptions import (
     ArgumentError,
     CollectionError,
-    CollectionTypeError,
     ConflictingDefinitionError,
     DataIdValueError,
-    DatasetTypeError,
     DatasetTypeExpressionError,
     InconsistentDataIdError,
-    MissingCollectionError,
-    MissingDatasetTypeError,
     NoDefaultCollectionError,
     OrphanedRecordError,
 )
 from .._registry import Registry
 from ..interfaces import ButlerAttributeExistsError
-
-if TYPE_CHECKING:
-    from ..sql_registry import SqlRegistry
+from ..sql_registry import SqlRegistry
 
 
 class RegistryTests(ABC):
     """Generic tests for the `SqlRegistry` class that can be subclassed to
     generate tests for different configurations.
     """
 
@@ -96,14 +94,18 @@
 
     datasetsManager: str | dict[str, str] | None = None
     """Name or configuration dictionary of the datasets manager class, if
     subclass provides value for this member then it overrides name specified
     in default configuration (`str` or `dict`).
     """
 
+    supportsCollectionRegex: bool = True
+    """True if the registry class being tested supports regex searches for
+    collections."""
+
     @classmethod
     @abstractmethod
     def getDataDir(cls) -> str:
         """Return the root directory containing test data YAML files."""
         raise NotImplementedError()
 
     def makeRegistryConfig(self) -> RegistryConfig:
@@ -345,17 +347,27 @@
     @unittest.skipIf(np is None, "numpy not available.")
     def testNumpyDataId(self):
         """Test that we can use a numpy int in a dataId."""
         registry = self.makeRegistry()
         dimensionEntries = [
             ("instrument", {"instrument": "DummyCam"}),
             ("physical_filter", {"instrument": "DummyCam", "name": "d-r", "band": "R"}),
+            ("day_obs", {"instrument": "DummyCam", "id": 20250101}),
             # Using an np.int64 here fails unless Records.fromDict is also
             # patched to look for numbers.Integral
-            ("visit", {"instrument": "DummyCam", "id": 42, "name": "fortytwo", "physical_filter": "d-r"}),
+            (
+                "visit",
+                {
+                    "instrument": "DummyCam",
+                    "id": 42,
+                    "name": "fortytwo",
+                    "physical_filter": "d-r",
+                    "day_obs": 20250101,
+                },
+            ),
         ]
         for args in dimensionEntries:
             registry.insertDimensionData(*args)
 
         # Try a normal integer and something that looks like an int but
         # is not.
         for visit_id in (42, np.int64(42)):
@@ -368,28 +380,54 @@
         """Test that `SqlRegistry.expandDataId` raises an exception when the
         given keys are inconsistent.
         """
         registry = self.makeRegistry()
         self.loadData(registry, "base.yaml")
         # Insert a few more dimension records for the next test.
         registry.insertDimensionData(
+            "day_obs",
+            {"instrument": "Cam1", "id": 20250101},
+        )
+        registry.insertDimensionData(
+            "group",
+            {"instrument": "Cam1", "name": "group1"},
+        )
+        registry.insertDimensionData(
             "exposure",
-            {"instrument": "Cam1", "id": 1, "obs_id": "one", "physical_filter": "Cam1-G"},
+            {
+                "instrument": "Cam1",
+                "id": 1,
+                "obs_id": "one",
+                "physical_filter": "Cam1-G",
+                "group": "group1",
+                "day_obs": 20250101,
+            },
+        )
+        registry.insertDimensionData(
+            "group",
+            {"instrument": "Cam1", "name": "group2"},
         )
         registry.insertDimensionData(
             "exposure",
-            {"instrument": "Cam1", "id": 2, "obs_id": "two", "physical_filter": "Cam1-G"},
+            {
+                "instrument": "Cam1",
+                "id": 2,
+                "obs_id": "two",
+                "physical_filter": "Cam1-G",
+                "group": "group2",
+                "day_obs": 20250101,
+            },
         )
         registry.insertDimensionData(
             "visit_system",
             {"instrument": "Cam1", "id": 0, "name": "one-to-one"},
         )
         registry.insertDimensionData(
             "visit",
-            {"instrument": "Cam1", "id": 1, "name": "one", "physical_filter": "Cam1-G"},
+            {"instrument": "Cam1", "id": 1, "name": "one", "physical_filter": "Cam1-G", "day_obs": 20250101},
         )
         registry.insertDimensionData(
             "visit_definition",
             {"instrument": "Cam1", "visit": 1, "exposure": 1},
         )
         with self.assertRaises(InconsistentDataIdError):
             registry.expandDataId(
@@ -730,24 +768,38 @@
         self.assertEqual(ref2b, registry.findDataset(datasetType, dataId2, collections=run2))
         # Define a new chain so we can test recursive chains.
         chain2 = "chain2"
         registry.registerCollection(chain2, type=CollectionType.CHAINED)
         registry.setCollectionChain(chain2, [run2, chain1])
         self.assertEqual(registry.getCollectionParentChains(chain1), {chain2})
         self.assertEqual(registry.getCollectionParentChains(run2), {chain1, chain2})
-        # Query for collections matching a regex.
+
+        if self.supportsCollectionRegex:
+            # Query for collections matching a regex.
+            self.assertCountEqual(
+                list(registry.queryCollections(re.compile("imported_."), flattenChains=False)),
+                ["imported_r", "imported_g"],
+            )
+            # Query for collections matching a regex or an explicit str.
+            self.assertCountEqual(
+                list(registry.queryCollections([re.compile("imported_."), "chain1"], flattenChains=False)),
+                ["imported_r", "imported_g", "chain1"],
+            )
+        # Same queries as the regex ones above, but using globs instead of
+        # regex.
         self.assertCountEqual(
-            list(registry.queryCollections(re.compile("imported_."), flattenChains=False)),
+            list(registry.queryCollections("imported_*", flattenChains=False)),
             ["imported_r", "imported_g"],
         )
         # Query for collections matching a regex or an explicit str.
         self.assertCountEqual(
-            list(registry.queryCollections([re.compile("imported_."), "chain1"], flattenChains=False)),
+            list(registry.queryCollections(["imported_*", "chain1"], flattenChains=False)),
             ["imported_r", "imported_g", "chain1"],
         )
+
         # Search for bias with dataId1 should find it via tag1 in chain2,
         # recursing, because is not in run1.
         self.assertIsNone(registry.findDataset(datasetType, dataId1, collections=run2))
         self.assertEqual(registry.findDataset(datasetType, dataId1, collections=chain2), ref1)
         # Search for bias with dataId2 should find it in run2 (ref2b).
         self.assertEqual(registry.findDataset(datasetType, dataId2, collections=chain2), ref2b)
         # Search for a flat that is in run2.  That should not be found
@@ -778,28 +830,133 @@
             registry.getCollectionType(chain1)
         # Remove tag1 as well, just to test that we can remove TAGGED
         # collections.
         registry.removeCollection(tag1)
         with self.assertRaises(MissingCollectionError):
             registry.getCollectionType(tag1)
 
+    def testCollectionChainCaching(self):
+        registry = self.makeRegistry()
+        with registry.caching_context():
+            registry.registerCollection("a")
+            registry.registerCollection("chain", CollectionType.CHAINED)
+            # There used to be a caching bug (DM-43750) that would throw an
+            # exception if you modified a collection chain for a collection
+            # that was already in the cache.
+            registry.setCollectionChain("chain", ["a"])
+            self.assertEqual(list(registry.getCollectionChain("chain")), ["a"])
+
     def testCollectionChainFlatten(self):
         """Test that `SqlRegistry.setCollectionChain` obeys its 'flatten'
         option.
         """
         registry = self.makeRegistry()
         registry.registerCollection("inner", CollectionType.CHAINED)
         registry.registerCollection("innermost", CollectionType.RUN)
         registry.setCollectionChain("inner", ["innermost"])
         registry.registerCollection("outer", CollectionType.CHAINED)
         registry.setCollectionChain("outer", ["inner"], flatten=False)
         self.assertEqual(list(registry.getCollectionChain("outer")), ["inner"])
         registry.setCollectionChain("outer", ["inner"], flatten=True)
         self.assertEqual(list(registry.getCollectionChain("outer")), ["innermost"])
 
+    def testCollectionChainPrependConcurrency(self):
+        """Verify that locking via database row locks is working as
+        expected.
+        """
+
+        def blocked_thread_func(registry: SqlRegistry):
+            # This call will become blocked after it has decided on positions
+            # for the new children in the collection chain, but before
+            # inserting them.
+            registry._managers.collections.prepend_collection_chain("chain", ["a"])
+
+        def unblocked_thread_func(registry: SqlRegistry):
+            registry._managers.collections.prepend_collection_chain("chain", ["b"])
+
+        registry = self._do_collection_concurrency_test(blocked_thread_func, unblocked_thread_func)
+
+        # blocked_thread_func should have finished first, inserting "a".
+        # unblocked_thread_func should have finished second, prepending "b".
+        self.assertEqual(("b", "a"), registry.getCollectionChain("chain"))
+
+    def testCollectionChainReplaceConcurrency(self):
+        """Verify that locking via database row locks is working as
+        expected.
+        """
+
+        def blocked_thread_func(registry: SqlRegistry):
+            # This call will become blocked after deleting children, but before
+            # inserting new ones.
+            registry.setCollectionChain("chain", ["a"])
+
+        def unblocked_thread_func(registry: SqlRegistry):
+            registry.setCollectionChain("chain", ["b"])
+
+        registry = self._do_collection_concurrency_test(blocked_thread_func, unblocked_thread_func)
+
+        # blocked_thread_func should have finished first.
+        # unblocked_thread_func should have finished second, overwriting the
+        # chain with "b".
+        self.assertEqual(("b",), registry.getCollectionChain("chain"))
+
+    def _do_collection_concurrency_test(
+        self, blocked_thread_func: Callable[[SqlRegistry]], unblocked_thread_func: Callable[[SqlRegistry]]
+    ) -> SqlRegistry:
+        # This function:
+        # 1. Sets up two registries pointing at the same database.
+        # 2. Start running 'blocked_thread_func' in a background thread,
+        #    arranging for it to become blocked during a critical section in
+        #    the collections manager.
+        # 3. Wait for 'blocked_thread_func' to reach the critical section
+        # 4. Start running 'unblocked_thread_func'.
+        # 5. Allow both functions to run to completion.
+
+        # Set up two registries pointing to the same DB
+        registry1 = self.makeRegistry()
+        assert isinstance(registry1, SqlRegistry)
+        registry2 = self.makeRegistry(share_repo_with=registry1)
+        if registry2 is None:
+            # This will happen for in-memory SQL databases.
+            raise unittest.SkipTest("Testing concurrency requires two connections to the same DB.")
+
+        registry1.registerCollection("chain", CollectionType.CHAINED)
+        for collection in ["a", "b"]:
+            registry1.registerCollection(collection)
+
+        # Arrange for registry1 to block during its critical section, allowing
+        # us to detect this and control when it becomes unblocked.
+        enter_barrier = Barrier(2, timeout=60)
+        exit_barrier = Barrier(2, timeout=60)
+
+        def wait_for_barrier():
+            enter_barrier.wait()
+            exit_barrier.wait()
+
+        registry1._managers.collections._block_for_concurrency_test = wait_for_barrier
+
+        with ThreadPoolExecutor(max_workers=1) as exec1:
+            with ThreadPoolExecutor(max_workers=1) as exec2:
+                future1 = exec1.submit(blocked_thread_func, registry1)
+                enter_barrier.wait()
+
+                # At this point registry 1 has entered the critical section and
+                # is waiting for us to release it.  Start the other thread.
+                future2 = exec2.submit(unblocked_thread_func, registry2)
+                # thread2 should block inside a database call, but we have no
+                # way to detect when it is in this state.
+                time.sleep(0.200)
+
+                # Let the threads run to completion.
+                exit_barrier.wait()
+                future1.result()
+                future2.result()
+
+        return registry1
+
     def testBasicTransaction(self):
         """Test that all operations within a single transaction block are
         rolled back if an exception propagates out of the block.
         """
         registry = self.makeRegistry()
         storageClass = StorageClass("testDatasetType")
         registry.storageClasses.registerStorageClass(storageClass)
@@ -852,43 +1009,92 @@
         """
         registry = self.makeRegistry()
 
         # need a bunch of dimensions and datasets for test
         registry.insertDimensionData(
             "instrument", dict(name="DummyCam", visit_max=25, exposure_max=300, detector_max=6)
         )
+        registry.insertDimensionData("day_obs", dict(instrument="DummyCam", id=20250101))
         registry.insertDimensionData(
             "physical_filter",
             dict(instrument="DummyCam", name="dummy_r", band="r"),
             dict(instrument="DummyCam", name="dummy_i", band="i"),
         )
         registry.insertDimensionData(
             "detector", *[dict(instrument="DummyCam", id=i, full_name=str(i)) for i in range(1, 6)]
         )
         registry.insertDimensionData(
             "visit",
-            dict(instrument="DummyCam", id=10, name="ten", physical_filter="dummy_i"),
-            dict(instrument="DummyCam", id=11, name="eleven", physical_filter="dummy_r"),
-            dict(instrument="DummyCam", id=20, name="twelve", physical_filter="dummy_r"),
+            dict(instrument="DummyCam", id=10, name="ten", physical_filter="dummy_i", day_obs=20250101),
+            dict(instrument="DummyCam", id=11, name="eleven", physical_filter="dummy_r", day_obs=20250101),
+            dict(instrument="DummyCam", id=20, name="twelve", physical_filter="dummy_r", day_obs=20250101),
+        )
+        registry.insertDimensionData(
+            "group",
+            dict(instrument="DummyCam", name="ten"),
+            dict(instrument="DummyCam", name="eleven"),
+            dict(instrument="DummyCam", name="twelve"),
         )
         for i in range(1, 6):
             registry.insertDimensionData(
                 "visit_detector_region",
                 dict(instrument="DummyCam", visit=10, detector=i),
                 dict(instrument="DummyCam", visit=11, detector=i),
                 dict(instrument="DummyCam", visit=20, detector=i),
             )
         registry.insertDimensionData(
             "exposure",
-            dict(instrument="DummyCam", id=100, obs_id="100", physical_filter="dummy_i"),
-            dict(instrument="DummyCam", id=101, obs_id="101", physical_filter="dummy_i"),
-            dict(instrument="DummyCam", id=110, obs_id="110", physical_filter="dummy_r"),
-            dict(instrument="DummyCam", id=111, obs_id="111", physical_filter="dummy_r"),
-            dict(instrument="DummyCam", id=200, obs_id="200", physical_filter="dummy_r"),
-            dict(instrument="DummyCam", id=201, obs_id="201", physical_filter="dummy_r"),
+            dict(
+                instrument="DummyCam",
+                id=100,
+                obs_id="100",
+                physical_filter="dummy_i",
+                group="ten",
+                day_obs=20250101,
+            ),
+            dict(
+                instrument="DummyCam",
+                id=101,
+                obs_id="101",
+                physical_filter="dummy_i",
+                group="ten",
+                day_obs=20250101,
+            ),
+            dict(
+                instrument="DummyCam",
+                id=110,
+                obs_id="110",
+                physical_filter="dummy_r",
+                group="eleven",
+                day_obs=20250101,
+            ),
+            dict(
+                instrument="DummyCam",
+                id=111,
+                obs_id="111",
+                physical_filter="dummy_r",
+                group="eleven",
+                day_obs=20250101,
+            ),
+            dict(
+                instrument="DummyCam",
+                id=200,
+                obs_id="200",
+                physical_filter="dummy_r",
+                group="twelve",
+                day_obs=20250101,
+            ),
+            dict(
+                instrument="DummyCam",
+                id=201,
+                obs_id="201",
+                physical_filter="dummy_r",
+                group="twelve",
+                day_obs=20250101,
+            ),
         )
         registry.insertDimensionData(
             "visit_definition",
             dict(instrument="DummyCam", exposure=100, visit=10),
             dict(instrument="DummyCam", exposure=101, visit=10),
             dict(instrument="DummyCam", exposure=110, visit=11),
             dict(instrument="DummyCam", exposure=111, visit=11),
@@ -1930,41 +2136,59 @@
         t5 = astropy.time.Time("2020-01-01T05:00:00", format="isot", scale="tai")
         allTimespans = [
             Timespan(a, b) for a, b in itertools.combinations([None, t1, t2, t3, t4, t5, None], r=2)
         ]
         # Insert some exposure records with timespans between each sequential
         # pair of those.
         registry.insertDimensionData(
+            "day_obs", {"instrument": "Cam1", "id": 20200101, "timespan": Timespan(t1, t5)}
+        )
+        registry.insertDimensionData(
+            "group",
+            {"instrument": "Cam1", "name": "group0"},
+            {"instrument": "Cam1", "name": "group1"},
+            {"instrument": "Cam1", "name": "group2"},
+            {"instrument": "Cam1", "name": "group3"},
+        )
+        registry.insertDimensionData(
             "exposure",
             {
                 "instrument": "Cam1",
                 "id": 0,
+                "group": "group0",
                 "obs_id": "zero",
                 "physical_filter": "Cam1-G",
+                "day_obs": 20200101,
                 "timespan": Timespan(t1, t2),
             },
             {
                 "instrument": "Cam1",
                 "id": 1,
+                "group": "group1",
                 "obs_id": "one",
                 "physical_filter": "Cam1-G",
+                "day_obs": 20200101,
                 "timespan": Timespan(t2, t3),
             },
             {
                 "instrument": "Cam1",
                 "id": 2,
+                "group": "group2",
                 "obs_id": "two",
                 "physical_filter": "Cam1-G",
+                "day_obs": 20200101,
                 "timespan": Timespan(t3, t4),
             },
             {
                 "instrument": "Cam1",
                 "id": 3,
+                "group": "group3",
                 "obs_id": "three",
                 "physical_filter": "Cam1-G",
+                "day_obs": 20200101,
                 "timespan": Timespan(t4, t5),
             },
         )
         # Get references to some datasets.
         bias2a = registry.findDataset("bias", instrument="Cam1", detector=2, collections="imported_g")
         bias3a = registry.findDataset("bias", instrument="Cam1", detector=3, collections="imported_g")
         bias2b = registry.findDataset("bias", instrument="Cam1", detector=2, collections="imported_r")
@@ -2804,15 +3028,15 @@
             ),
             Test(
                 "-tract,-visit.exposure_time", "tract,visit", ((1, 2), (1, 2), (0, 1), (0, 1), (0, 2), (0, 2))
             ),
             Test("tract,-exposure_time", "tract,visit", ((0, 1), (0, 1), (0, 2), (0, 2), (1, 2), (1, 2))),
             Test("tract,visit.name", "tract,visit", ((0, 1), (0, 1), (0, 2), (0, 2), (1, 2), (1, 2))),
             Test(
-                "tract,-timespan.begin,timespan.end",
+                "tract,-visit.timespan.begin,visit.timespan.end",
                 "tract,visit",
                 ((0, 2), (0, 2), (0, 1), (0, 1), (1, 2), (1, 2)),
             ),
             Test("visit.day_obs,exposure.day_obs", "visit,exposure", ()),
             Test("visit.timespan.begin,-exposure.timespan.begin", "visit,exposure", ()),
             Test(
                 "tract,detector",
@@ -2868,15 +3092,15 @@
                 list(do_query().order_by(order_by))
 
         with self.assertRaisesRegex(ValueError, "Metadata 'exposure_time' exists in more than one dimension"):
             list(do_query(("exposure", "visit")).order_by("exposure_time"))
 
         with self.assertRaisesRegex(
             ValueError,
-            r"Timespan exists in more than one dimension element \(exposure, visit\); "
+            r"Timespan exists in more than one dimension element \(day_obs, exposure, visit\); "
             r"qualify timespan with specific dimension name\.",
         ):
             list(do_query(("exposure", "visit")).order_by("timespan.begin"))
 
         with self.assertRaisesRegex(
             ValueError, "Cannot find any temporal dimension element for 'timespan.begin'"
         ):
@@ -3156,15 +3380,15 @@
                 .limit(5)
             ],
             [318, 322, 326, 330, 332],
         )
         self.assertEqual(
             [
                 data_id["visit"]
-                for data_id in registry.queryDataIds(["visit"], instrument="HSC").order_by("id").limit(5)
+                for data_id in registry.queryDataIds(["visit"], instrument="HSC").order_by("visit").limit(5)
             ],
             [318, 322, 326, 330, 332],
         )
         self.assertEqual(
             [
                 record.id
                 for record in registry.queryDimensionRecords("detector", instrument="HSC")
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/versions.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/versions.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/registry/wildcards.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/registry/wildcards.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_butler/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,9 +21,8 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from ._factory import *
-from ._remote_butler import *
+from ._direct_butler import *
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_authentication.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_authentication.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 __all__ = ()
 
 import os
 from fnmatch import fnmatchcase
 from urllib.parse import urlparse
 
-_SERVER_WHITELIST = ["*.lsst.cloud"]
+_SERVER_WHITELIST = ["*.lsst.cloud", "*.slac.stanford.edu"]
 _EXPLICIT_BUTLER_ACCESS_TOKEN_ENVIRONMENT_KEY = "BUTLER_RUBIN_ACCESS_TOKEN"
 _RSP_JUPYTER_ACCESS_TOKEN_ENVIRONMENT_KEY = "ACCESS_TOKEN"
 
 
 def get_authentication_token_from_environment(server_url: str) -> str | None:
     """Search the environment for a Rubin Science Platform access token.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_collection_args.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_collection_args.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_config.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_factory.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_factory.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 import httpx
 from lsst.daf.butler.repo_relocation import replaceRoot
 
 from .._butler_config import ButlerConfig
 from .._butler_instance_options import ButlerInstanceOptions
 from ._authentication import get_authentication_token_from_environment
 from ._config import RemoteButlerConfigModel
+from ._http_connection import RemoteButlerHttpConnection
 from ._remote_butler import RemoteButler, RemoteButlerCache
 
 
 class RemoteButlerFactory:
     """Factory for instantiating RemoteButler instances bound to a user's Rubin
     Science Platform Gafaelfawr access token.  All Butler instances created by
     this factory share a common HTTP connection pool.
@@ -87,18 +88,18 @@
 
     def create_butler_for_access_token(
         self, access_token: str, *, butler_options: ButlerInstanceOptions | None = None
     ) -> RemoteButler:
         if butler_options is None:
             butler_options = ButlerInstanceOptions()
         return RemoteButler(
-            http_client=self.http_client,
-            access_token=access_token,
+            connection=RemoteButlerHttpConnection(
+                http_client=self.http_client, server_url=self.server_url, access_token=access_token
+            ),
             options=butler_options,
-            server_url=self.server_url,
             cache=self._cache,
         )
 
     def create_butler_with_credentials_from_environment(
         self, *, butler_options: ButlerInstanceOptions | None = None
     ) -> RemoteButler:
         token = get_authentication_token_from_environment(self.server_url)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_registry.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 
 from __future__ import annotations
 
 import contextlib
 from collections.abc import Iterable, Iterator, Mapping, Sequence
 from typing import Any
 
+from lsst.utils.iteration import ensure_iterable
+
 from .._dataset_association import DatasetAssociation
 from .._dataset_ref import DatasetId, DatasetIdGenEnum, DatasetRef
 from .._dataset_type import DatasetType
 from .._named import NameLookupMapping
 from .._storage_class import StorageClassFactory
 from .._timespan import Timespan
 from ..dimensions import (
@@ -47,21 +49,23 @@
     DimensionRecord,
     DimensionUniverse,
 )
 from ..registry import (
     CollectionArgType,
     CollectionSummary,
     CollectionType,
+    CollectionTypeError,
     DatasetTypeError,
     Registry,
     RegistryDefaults,
 )
 from ..registry.queries import DataCoordinateQueryResults, DatasetQueryResults, DimensionRecordQueryResults
 from ..remote_butler import RemoteButler
 from ._collection_args import convert_collection_arg_to_glob_string_list
+from .server_models import QueryCollectionsRequestModel
 
 
 class RemoteButlerRegistry(Registry):
     """Implementation of the `Registry` interface for `RemoteButler.
 
     Parameters
     ----------
@@ -102,39 +106,45 @@
 
     def registerCollection(
         self, name: str, type: CollectionType = CollectionType.TAGGED, doc: str | None = None
     ) -> bool:
         raise NotImplementedError()
 
     def getCollectionType(self, name: str) -> CollectionType:
-        raise NotImplementedError()
+        return self._butler._get_collection_info(name).type
 
     def registerRun(self, name: str, doc: str | None = None) -> bool:
         raise NotImplementedError()
 
     def removeCollection(self, name: str) -> None:
         raise NotImplementedError()
 
     def getCollectionChain(self, parent: str) -> Sequence[str]:
-        raise NotImplementedError()
+        info = self._butler._get_collection_info(parent)
+        if info.type is not CollectionType.CHAINED:
+            raise CollectionTypeError(f"Collection '{parent}' has type {info.type.name}, not CHAINED.")
+        return info.children
 
     def setCollectionChain(self, parent: str, children: Any, *, flatten: bool = False) -> None:
         raise NotImplementedError()
 
     def getCollectionParentChains(self, collection: str) -> set[str]:
-        raise NotImplementedError()
+        info = self._butler._get_collection_info(collection, include_parents=True)
+        assert info.parents is not None, "Requested list of parents from server, but it did not send them."
+        return info.parents
 
     def getCollectionDocumentation(self, collection: str) -> str | None:
-        raise NotImplementedError()
+        info = self._butler._get_collection_info(collection, include_doc=True)
+        return info.doc
 
     def setCollectionDocumentation(self, collection: str, doc: str | None) -> None:
         raise NotImplementedError()
 
     def getCollectionSummary(self, collection: str) -> CollectionSummary:
-        raise NotImplementedError()
+        return self._butler._get_collection_summary(collection)
 
     def registerDatasetType(self, datasetType: DatasetType) -> bool:
         raise NotImplementedError()
 
     def removeDatasetType(self, name: str | tuple[str, ...]) -> None:
         raise NotImplementedError()
 
@@ -267,15 +277,23 @@
         self,
         expression: Any = ...,
         datasetType: DatasetType | None = None,
         collectionTypes: Iterable[CollectionType] | CollectionType = CollectionType.all(),
         flattenChains: bool = False,
         includeChains: bool | None = None,
     ) -> Sequence[str]:
-        raise NotImplementedError()
+        if includeChains is None:
+            includeChains = not flattenChains
+        query = QueryCollectionsRequestModel(
+            search=convert_collection_arg_to_glob_string_list(expression),
+            collection_types=list(ensure_iterable(collectionTypes)),
+            flatten_chains=flattenChains,
+            include_chains=includeChains,
+        )
+        return self._butler._query_collections(query).collections
 
     def queryDatasets(
         self,
         datasetType: Any,
         *,
         collections: CollectionArgType | None = None,
         dimensions: Iterable[Dimension | str] | None = None,
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/_remote_butler.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/_remote_butler.py`

 * *Files 18% similar despite different names*

```diff
@@ -23,200 +23,157 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
-__all__ = (
-    "ButlerServerError",
-    "RemoteButler",
-)
+__all__ = ("RemoteButler",)
 
-from collections.abc import Collection, Iterable, Mapping, Sequence
+from collections.abc import Collection, Iterable, Sequence
 from contextlib import AbstractContextManager
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, TextIO, TypeVar, cast
-from uuid import uuid4
+from typing import TYPE_CHECKING, Any, TextIO, cast
 
-import httpx
-from lsst.daf.butler import __version__
 from lsst.daf.butler.datastores.file_datastore.retrieve_artifacts import (
     determine_destination_for_retrieved_artifact,
 )
 from lsst.daf.butler.datastores.fileDatastoreClient import (
     FileDatastoreGetPayload,
     get_dataset_as_python_object,
 )
 from lsst.resources import ResourcePath, ResourcePathExpression
-from pydantic import BaseModel, TypeAdapter
 
 from .._butler import Butler
+from .._butler_collections import ButlerCollections
 from .._butler_instance_options import ButlerInstanceOptions
 from .._dataset_existence import DatasetExistence
 from .._dataset_ref import DatasetId, DatasetRef, SerializedDatasetRef
 from .._dataset_type import DatasetType, SerializedDatasetType
 from .._deferredDatasetHandle import DeferredDatasetHandle
+from .._exceptions import DatasetNotFoundError
 from .._storage_class import StorageClass, StorageClassFactory
 from .._utilities.locked_object import LockedObject
 from ..datastore import DatasetRefURIs
-from ..dimensions import DataCoordinate, DataIdValue, DimensionConfig, DimensionUniverse, SerializedDataId
+from ..dimensions import DataIdValue, DimensionConfig, DimensionUniverse
 from ..registry import (
     CollectionArgType,
-    MissingDatasetTypeError,
+    CollectionSummary,
     NoDefaultCollectionError,
     Registry,
     RegistryDefaults,
 )
-from ._authentication import get_authentication_headers
 from ._collection_args import convert_collection_arg_to_glob_string_list
+from ._ref_utils import apply_storage_class_override, normalize_dataset_type_name, simplify_dataId
 from .server_models import (
-    CLIENT_REQUEST_ID_HEADER_NAME,
     CollectionList,
-    DatasetTypeName,
     FindDatasetRequestModel,
     FindDatasetResponseModel,
+    GetCollectionInfoResponseModel,
+    GetCollectionSummaryResponseModel,
     GetFileByDataIdRequestModel,
     GetFileResponseModel,
+    QueryCollectionsRequestModel,
+    QueryCollectionsResponseModel,
 )
 
 if TYPE_CHECKING:
     from .._file_dataset import FileDataset
     from .._limited_butler import LimitedButler
-    from .._query import Query
     from .._timespan import Timespan
-    from ..dimensions import DataId, DimensionGroup, DimensionRecord
+    from ..dimensions import DataId
+    from ..queries import Query
     from ..transfers import RepoExportContext
 
-
-_AnyPydanticModel = TypeVar("_AnyPydanticModel", bound=BaseModel)
-"""Generic type variable that accepts any Pydantic model class."""
-
-_SERIALIZED_DATA_ID_TYPE_ADAPTER = TypeAdapter(SerializedDataId)
+from ._http_connection import RemoteButlerHttpConnection, parse_model
 
 
 class RemoteButler(Butler):  # numpydoc ignore=PR02
     """A `Butler` that can be used to connect through a remote server.
 
     Parameters
     ----------
-    server_url : `str`
-        URL of the Butler server we will connect to.
     options : `ButlerInstanceOptions`
         Default values and other settings for the Butler instance.
-    http_client : `httpx.Client`
-        HTTP connection pool we will use to connect to the server.
-    access_token : `str`
-        Rubin Science Platform Gafaelfawr access token that will be used to
-        authenticate with the server.
-    cache : RemoteButlerCache
+    connection : `RemoteButlerHttpConnection`
+        Connection to Butler server.
+    cache : `RemoteButlerCache`
         Cache of data shared between multiple RemoteButler instances connected
         to the same server.
 
     Notes
     -----
     Instead of using this constructor, most users should use either
     `Butler.from_config` or `RemoteButlerFactory`.
     """
 
     _registry_defaults: RegistryDefaults
-    _client: httpx.Client
-    _server_url: str
-    _access_token: str
-    _headers: dict[str, str]
+    _connection: RemoteButlerHttpConnection
     _cache: RemoteButlerCache
     _registry: Registry
 
     # This is __new__ instead of __init__ because we have to support
     # instantiation via the legacy constructor Butler.__new__(), which
     # reads the configuration and selects which subclass to instantiate.  The
     # interaction between __new__ and __init__ is kind of wacky in Python.  If
     # we were using __init__ here, __init__ would be called twice (once when
     # the RemoteButler instance is constructed inside Butler.from_config(), and
     # a second time with the original arguments to Butler() when the instance
     # is returned from Butler.__new__()
     def __new__(
         cls,
         *,
-        server_url: str,
+        connection: RemoteButlerHttpConnection,
         options: ButlerInstanceOptions,
-        http_client: httpx.Client,
-        access_token: str,
         cache: RemoteButlerCache,
     ) -> RemoteButler:
         self = cast(RemoteButler, super().__new__(cls))
         self.storageClasses = StorageClassFactory()
 
-        self._client = http_client
-        self._server_url = server_url
+        self._connection = connection
         self._cache = cache
-        self._access_token = access_token
 
         # TODO: RegistryDefaults should have finish() called on it, but this
         # requires getCollectionSummary() which is not yet implemented
         self._registry_defaults = RegistryDefaults(
             options.collections, options.run, options.inferDefaults, **options.kwargs
         )
 
-        auth_headers = get_authentication_headers(access_token)
-        headers = {"user-agent": f"RemoteButler/{__version__}"}
-
-        self._headers = auth_headers | headers
-
         # Avoid a circular import by deferring this import.
         from ._registry import RemoteButlerRegistry
 
         self._registry = RemoteButlerRegistry(self)
 
         return self
 
     def isWriteable(self) -> bool:
         # Docstring inherited.
         return False
 
     @property
+    def collection_chains(self) -> ButlerCollections:
+        """Object with methods for modifying collection chains."""
+        raise NotImplementedError()
+
+    @property
     def dimensions(self) -> DimensionUniverse:
         # Docstring inherited.
         with self._cache.access() as cache:
             if cache.dimensions is not None:
                 return cache.dimensions
 
-        response = self._get("universe")
+        response = self._connection.get("universe")
 
         config = DimensionConfig.fromString(response.text, format="json")
         universe = DimensionUniverse(config)
         with self._cache.access() as cache:
             if cache.dimensions is None:
                 cache.dimensions = universe
             return cache.dimensions
 
-    def _simplify_dataId(self, dataId: DataId | None, kwargs: dict[str, DataIdValue]) -> SerializedDataId:
-        """Take a generic Data ID and convert it to a serializable form.
-
-        Parameters
-        ----------
-        dataId : `dict`, `None`, `DataCoordinate`
-            The data ID to serialize.
-        kwargs : `dict`
-            Additional entries to augment or replace the values in ``dataId``.
-
-        Returns
-        -------
-        data_id : `SerializedDataId`
-            A serializable form.
-        """
-        if dataId is None:
-            dataId = {}
-        elif isinstance(dataId, DataCoordinate):
-            dataId = dataId.to_simple(minimal=True).dataId
-        else:
-            dataId = dict(dataId)
-
-        return _SERIALIZED_DATA_ID_TYPE_ADAPTER.validate_python(dataId | kwargs)
-
     def _caching_context(self) -> AbstractContextManager[None]:
         # Docstring inherited.
         # Not implemented for now, will have to think whether this needs to
         # do something on client side and/or remote side.
         raise NotImplementedError()
 
     def transaction(self) -> AbstractContextManager[None]:
@@ -243,90 +200,92 @@
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
         parameters: dict | None = None,
         collections: Any = None,
         storageClass: str | StorageClass | None = None,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> DeferredDatasetHandle:
-        try:
-            response = self._get_file_info(datasetRefOrType, dataId, collections, kwargs)
-            # Check that artifact information is available.
-            _to_file_payload(response)
-        except FileNotFoundError as e:
-            # Inconsistent with the behavior of get(), DirectButler returns
-            # LookupError if a dataset cannot be found here.
-            raise LookupError(str(e)) from e
+        response = self._get_file_info(datasetRefOrType, dataId, collections, timespan, kwargs)
+        # Check that artifact information is available.
+        _to_file_payload(response)
         ref = DatasetRef.from_simple(response.dataset_ref, universe=self.dimensions)
         return DeferredDatasetHandle(butler=self, ref=ref, parameters=parameters, storageClass=storageClass)
 
     def get(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
         parameters: dict[str, Any] | None = None,
         collections: Any = None,
         storageClass: StorageClass | str | None = None,
+        timespan: Timespan | None = None,
         **kwargs: Any,
     ) -> Any:
         # Docstring inherited.
-        model = self._get_file_info(datasetRefOrType, dataId, collections, kwargs)
+        model = self._get_file_info(datasetRefOrType, dataId, collections, timespan, kwargs)
 
         ref = DatasetRef.from_simple(model.dataset_ref, universe=self.dimensions)
         # If the caller provided a DatasetRef, they may have overridden the
         # component on it.  We need to explicitly handle this because we did
         # not send the DatasetType to the server in this case.
         if isinstance(datasetRefOrType, DatasetRef):
             componentOverride = datasetRefOrType.datasetType.component()
             if componentOverride:
                 ref = ref.makeComponentRef(componentOverride)
-        ref = _apply_storage_class_override(ref, datasetRefOrType, storageClass)
+        ref = apply_storage_class_override(ref, datasetRefOrType, storageClass)
 
+        return self._get_dataset_as_python_object(ref, model, parameters)
+
+    def _get_dataset_as_python_object(
+        self,
+        ref: DatasetRef,
+        model: GetFileResponseModel,
+        parameters: dict[str, Any] | None,
+    ) -> Any:
+        # This thin wrapper method is here to provide a place to hook in a mock
+        # mimicking DatastoreMock functionality for use in unit tests.
         return get_dataset_as_python_object(
             ref,
             _to_file_payload(model),
             parameters=parameters,
         )
 
     def _get_file_info(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         dataId: DataId | None,
         collections: CollectionArgType,
+        timespan: Timespan | None,
         kwargs: dict[str, DataIdValue],
     ) -> GetFileResponseModel:
         """Send a request to the server for the file URLs and metadata
         associated with a dataset.
         """
         if isinstance(datasetRefOrType, DatasetRef):
             if dataId is not None:
                 raise ValueError("DatasetRef given, cannot use dataId as well")
             return self._get_file_info_for_ref(datasetRefOrType)
         else:
             request = GetFileByDataIdRequestModel(
-                dataset_type_name=self._normalize_dataset_type_name(datasetRefOrType),
+                dataset_type_name=normalize_dataset_type_name(datasetRefOrType),
                 collections=self._normalize_collections(collections),
-                data_id=self._simplify_dataId(dataId, kwargs),
+                data_id=simplify_dataId(dataId, kwargs),
+                timespan=timespan,
             )
-            response = self._post("get_file_by_data_id", request, expected_errors=(404,))
-            if response.status_code == 404:
-                raise FileNotFoundError(
-                    f"Dataset not found with DataId: {dataId} DatasetType: {datasetRefOrType}"
-                    f" collections: {collections}"
-                )
-            return self._parse_model(response, GetFileResponseModel)
+            response = self._connection.post("get_file_by_data_id", request)
+            return parse_model(response, GetFileResponseModel)
 
     def _get_file_info_for_ref(self, ref: DatasetRef) -> GetFileResponseModel:
-        response = self._get(f"get_file/{ref.id}", expected_errors=(404,))
-        if response.status_code == 404:
-            raise FileNotFoundError(f"Dataset not found: {ref.id}")
-        return self._parse_model(response, GetFileResponseModel)
+        response = self._connection.get(f"get_file/{ref.id}")
+        return parse_model(response, GetFileResponseModel)
 
     def getURIs(
         self,
         datasetRefOrType: DatasetRef | DatasetType | str,
         /,
         dataId: DataId | None = None,
         *,
@@ -335,15 +294,15 @@
         run: str | None = None,
         **kwargs: Any,
     ) -> DatasetRefURIs:
         # Docstring inherited.
         if predict or run:
             raise NotImplementedError("Predict mode is not supported by RemoteButler")
 
-        response = self._get_file_info(datasetRefOrType, dataId, collections, kwargs)
+        response = self._get_file_info(datasetRefOrType, dataId, collections, None, kwargs)
         file_info = _to_file_payload(response).file_info
         if len(file_info) == 1:
             return DatasetRefURIs(primaryURI=ResourcePath(str(file_info[0].url)))
         else:
             components = {}
             for f in file_info:
                 component = f.datastoreRecords.component
@@ -355,19 +314,15 @@
                 components[component] = ResourcePath(str(f.url))
             return DatasetRefURIs(componentURIs=components)
 
     def get_dataset_type(self, name: str) -> DatasetType:
         # In future implementation this should directly access the cache
         # and only go to the server if the dataset type is not known.
         path = f"dataset_type/{name}"
-        response = self._get(path, expected_errors=(404,))
-        if response.status_code != httpx.codes.OK:
-            content = response.json()
-            if content["exception"] == "MissingDatasetTypeError":
-                raise MissingDatasetTypeError(content["detail"])
+        response = self._connection.get(path)
         return DatasetType.from_simple(SerializedDatasetType(**response.json()), universe=self.dimensions)
 
     def get_dataset(
         self,
         id: DatasetId,
         *,
         storage_class: str | StorageClass | None = None,
@@ -377,20 +332,18 @@
         path = f"dataset/{id}"
         params: dict[str, str | bool] = {
             "dimension_records": dimension_records,
             "datastore_records": datastore_records,
         }
         if datastore_records:
             raise ValueError("Datastore records can not yet be returned in client/server butler.")
-        response = self._get(path, params=params)
+        response = self._connection.get(path, params=params)
         if response.json() is None:
             return None
-        ref = DatasetRef.from_simple(
-            self._parse_model(response, SerializedDatasetRef), universe=self.dimensions
-        )
+        ref = DatasetRef.from_simple(parse_model(response, SerializedDatasetRef), universe=self.dimensions)
         if storage_class is not None:
             ref = ref.overrideStorageClass(storage_class)
         return ref
 
     def find_dataset(
         self,
         dataset_type: DatasetType | str,
@@ -403,31 +356,31 @@
         datastore_records: bool = False,
         **kwargs: Any,
     ) -> DatasetRef | None:
         if datastore_records:
             raise ValueError("Datastore records can not yet be returned in client/server butler.")
 
         query = FindDatasetRequestModel(
-            data_id=self._simplify_dataId(data_id, kwargs),
+            data_id=simplify_dataId(data_id, kwargs),
             collections=self._normalize_collections(collections),
-            timespan=timespan.to_simple() if timespan is not None else None,
+            timespan=timespan,
             dimension_records=dimension_records,
             datastore_records=datastore_records,
         )
 
-        dataset_type_name = self._normalize_dataset_type_name(dataset_type)
+        dataset_type_name = normalize_dataset_type_name(dataset_type)
         path = f"find_dataset/{dataset_type_name}"
-        response = self._post(path, query)
+        response = self._connection.post(path, query)
 
-        model = self._parse_model(response, FindDatasetResponseModel)
+        model = parse_model(response, FindDatasetResponseModel)
         if model.dataset_ref is None:
             return None
 
         ref = DatasetRef.from_simple(model.dataset_ref, universe=self.dimensions)
-        return _apply_storage_class_override(ref, dataset_type, storage_class)
+        return apply_storage_class_override(ref, dataset_type, storage_class)
 
     def retrieveArtifacts(
         self,
         refs: Iterable[DatasetRef],
         destination: ResourcePathExpression,
         transfer: str = "auto",
         preserve_path: bool = True,
@@ -464,17 +417,17 @@
         *,
         full_check: bool = True,
         collections: Any = None,
         **kwargs: Any,
     ) -> DatasetExistence:
         try:
             response = self._get_file_info(
-                dataset_ref_or_type, dataId=data_id, collections=collections, kwargs=kwargs
+                dataset_ref_or_type, dataId=data_id, collections=collections, timespan=None, kwargs=kwargs
             )
-        except FileNotFoundError:
+        except DatasetNotFoundError:
             return DatasetExistence.UNRECOGNIZED
 
         if response.artifact is None:
             if full_check:
                 return DatasetExistence.RECORDED
             else:
                 return DatasetExistence.RECORDED | DatasetExistence._ASSUMED
@@ -574,255 +527,89 @@
     def registry(self) -> Registry:
         return self._registry
 
     def _query(self) -> AbstractContextManager[Query]:
         # Docstring inherited.
         raise NotImplementedError()
 
-    def _query_data_ids(
-        self,
-        dimensions: DimensionGroup | Iterable[str] | str,
-        *,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        expanded: bool = False,
-        order_by: Iterable[str] | str | None = None,
-        limit: int | None = None,
-        offset: int | None = None,
-        explain: bool = True,
-        **kwargs: Any,
-    ) -> list[DataCoordinate]:
-        # Docstring inherited.
-        raise NotImplementedError()
-
-    def _query_datasets(
-        self,
-        dataset_type: Any,
-        collections: CollectionArgType | None = None,
-        *,
-        find_first: bool = True,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        expanded: bool = False,
-        explain: bool = True,
-        **kwargs: Any,
-    ) -> list[DatasetRef]:
-        # Docstring inherited.
-        raise NotImplementedError()
-
-    def _query_dimension_records(
-        self,
-        element: str,
-        *,
-        data_id: DataId | None = None,
-        where: str = "",
-        bind: Mapping[str, Any] | None = None,
-        order_by: Iterable[str] | str | None = None,
-        limit: int | None = None,
-        offset: int | None = None,
-        explain: bool = True,
-        **kwargs: Any,
-    ) -> list[DimensionRecord]:
-        # Docstring inherited.
-        raise NotImplementedError()
-
     def pruneDatasets(
         self,
         refs: Iterable[DatasetRef],
         *,
         disassociate: bool = True,
         unstore: bool = False,
         tags: Iterable[str] = (),
         purge: bool = False,
     ) -> None:
         # Docstring inherited.
         raise NotImplementedError()
 
-    def _get_url(self, path: str, version: str = "v1") -> str:
-        """Form the complete path to an endpoint on the server.
-
-        Parameters
-        ----------
-        path : `str`
-            The relative path to the server endpoint.
-        version : `str`, optional
-            Version string to prepend to path. Defaults to "v1".
-
-        Returns
-        -------
-        path : `str`
-            The full path to the endpoint.
-        """
-        slash = "" if self._server_url.endswith("/") else "/"
-        return f"{self._server_url}{slash}{version}/{path}"
-
-    def _post(self, path: str, model: BaseModel, expected_errors: Iterable[int] = ()) -> httpx.Response:
-        """Send a POST request to the Butler server."""
-        json = model.model_dump_json(exclude_unset=True).encode("utf-8")
-        return self._send_request(
-            "POST",
-            path,
-            content=json,
-            headers={"content-type": "application/json"},
-            expected_errors=expected_errors,
-        )
-
-    def _get(
-        self, path: str, params: Mapping[str, str | bool] | None = None, expected_errors: Iterable[int] = ()
-    ) -> httpx.Response:
-        """Send a GET request to the Butler server."""
-        return self._send_request("GET", path, params=params, expected_errors=expected_errors)
-
-    def _send_request(
-        self,
-        method: str,
-        path: str,
-        *,
-        content: bytes | None = None,
-        params: Mapping[str, str | bool] | None = None,
-        headers: Mapping[str, str] | None = None,
-        expected_errors: Iterable[int],
-    ) -> httpx.Response:
-        url = self._get_url(path)
-
-        request_id = str(uuid4())
-        request_headers = {CLIENT_REQUEST_ID_HEADER_NAME: request_id}
-        request_headers.update(self._headers)
-        if headers is not None:
-            request_headers.update(headers)
-
-        try:
-            response = self._client.request(
-                method, url, content=content, params=params, headers=request_headers
-            )
-            if response.status_code not in expected_errors:
-                response.raise_for_status()
-            return response
-        except httpx.HTTPError as e:
-            raise ButlerServerError(request_id) from e
-
-    def _parse_model(self, response: httpx.Response, model: type[_AnyPydanticModel]) -> _AnyPydanticModel:
-        """Deserialize a Pydantic model from the body of an HTTP response."""
-        return model.model_validate_json(response.content)
-
     def _normalize_collections(self, collections: CollectionArgType | None) -> CollectionList:
         """Convert the ``collections`` parameter in the format used by Butler
         methods to a standardized format for the REST API.
         """
         if collections is None:
             if not self.collections:
                 raise NoDefaultCollectionError(
                     "No collections provided, and no defaults from butler construction."
                 )
             collections = self.collections
         return convert_collection_arg_to_glob_string_list(collections)
 
-    def _normalize_dataset_type_name(self, datasetTypeOrName: DatasetType | str) -> DatasetTypeName:
-        """Convert DatasetType parameters in the format used by Butler methods
-        to a standardized string name for the REST API.
-        """
-        if isinstance(datasetTypeOrName, DatasetType):
-            return DatasetTypeName(datasetTypeOrName.name)
-        else:
-            return DatasetTypeName(datasetTypeOrName)
-
     def _clone(
         self,
         *,
         collections: Any = None,
         run: str | None = None,
         inferDefaults: bool = True,
         **kwargs: Any,
     ) -> RemoteButler:
         return RemoteButler(
-            server_url=self._server_url,
-            http_client=self._client,
-            access_token=self._access_token,
+            connection=self._connection,
             cache=self._cache,
             options=ButlerInstanceOptions(
                 collections=collections,
                 run=run,
                 writeable=self.isWriteable(),
                 inferDefaults=inferDefaults,
                 kwargs=kwargs,
             ),
         )
 
     def __str__(self) -> str:
-        return f"RemoteButler({self._server_url})"
+        return f"RemoteButler({self._connection.server_url})"
 
+    def _get_collection_info(
+        self, collection_name: str, include_doc: bool = False, include_parents: bool = False
+    ) -> GetCollectionInfoResponseModel:
+        response = self._connection.get(
+            "collection_info",
+            {"name": collection_name, "include_doc": include_doc, "include_parents": include_parents},
+        )
+        return parse_model(response, GetCollectionInfoResponseModel)
 
-def _extract_dataset_type(datasetRefOrType: DatasetRef | DatasetType | str) -> DatasetType | None:
-    """Return the DatasetType associated with the argument, or None if the
-    argument is not an object that contains a DatasetType object.
-    """
-    if isinstance(datasetRefOrType, DatasetType):
-        return datasetRefOrType
-    elif isinstance(datasetRefOrType, DatasetRef):
-        return datasetRefOrType.datasetType
-    else:
-        return None
-
-
-def _apply_storage_class_override(
-    ref: DatasetRef,
-    original_dataset_ref_or_type: DatasetRef | DatasetType | str,
-    explicit_storage_class: StorageClass | str | None,
-) -> DatasetRef:
-    """Return a DatasetRef with its storage class overridden to match the
-    StorageClass supplied by the user as input to one of the search functions.
-
-    Parameters
-    ----------
-    ref : `DatasetRef`
-        The ref to which we will apply the StorageClass override.
-    original_dataset_ref_or_type : `DatasetRef` | `DatasetType` | `str`
-        The ref or type that was input to the search, which may contain a
-        storage class override.
-    explicit_storage_class : `StorageClass` | `str` | `None`
-        A storage class that the user explicitly requested as an override.
-    """
-    if explicit_storage_class is not None:
-        return ref.overrideStorageClass(explicit_storage_class)
-
-    # If the caller provided a DatasetRef or DatasetType, they may have
-    # overridden the storage class on it, and we need to propagate that to the
-    # output.
-    dataset_type = _extract_dataset_type(original_dataset_ref_or_type)
-    if dataset_type is not None:
-        return ref.overrideStorageClass(dataset_type.storageClass)
-
-    return ref
+    def _get_collection_summary(self, collection_name: str) -> CollectionSummary:
+        response = self._connection.get("collection_summary", {"name": collection_name})
+        parsed = parse_model(response, GetCollectionSummaryResponseModel)
+        return CollectionSummary.from_simple(parsed.summary, self.dimensions)
+
+    def _query_collections(self, query: QueryCollectionsRequestModel) -> QueryCollectionsResponseModel:
+        response = self._connection.post("query_collections", query)
+        return parse_model(response, QueryCollectionsResponseModel)
 
 
 def _to_file_payload(get_file_response: GetFileResponseModel) -> FileDatastoreGetPayload:
     if get_file_response.artifact is None:
         ref = get_file_response.dataset_ref
-        raise FileNotFoundError(f"Dataset is known, but artifact is not available. (datasetId='{ref.id}')")
+        raise DatasetNotFoundError(f"Dataset is known, but artifact is not available. (datasetId='{ref.id}')")
 
     return get_file_response.artifact
 
 
 @dataclass
 class _RemoteButlerCacheData:
     dimensions: DimensionUniverse | None = None
 
 
 class RemoteButlerCache(LockedObject[_RemoteButlerCacheData]):
     def __init__(self) -> None:
         super().__init__(_RemoteButlerCacheData())
-
-
-class ButlerServerError(RuntimeError):
-    """Exception returned when there is an error communicating with the Butler
-    server.
-
-    Parameters
-    ----------
-    client_request_id : `str`
-        Request ID to include in the exception message.
-    """
-
-    def __init__(self, client_request_id: str):
-        super().__init__(f"Error while communicating with Butler server.  Request ID: {client_request_id}")
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_dependencies.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/_dependencies.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_exceptions.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/queries/tree/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,21 +21,20 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-from fastapi import HTTPException
+from ._base import *
+from ._column_expression import *
+from ._column_literal import *
+from ._column_reference import *
+from ._column_set import *
+from ._predicate import *
+from ._predicate import LogicalNot
+from ._query_tree import *
 
+LogicalNot.model_rebuild()
+del LogicalNot
 
-class NotFoundException(HTTPException):
-    """Exception corresponding to a 404 server error.
-
-    Parameters
-    ----------
-    message : `str`, optional
-        Message to include in the exception.
-    """
-
-    def __init__(self, message: str = "Not found"):
-        super().__init__(status_code=404, detail=message)
+Predicate.model_rebuild()
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_factory.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/_server.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/_server.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,24 +25,23 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = ("create_app",)
 
-from typing import Awaitable, Callable
+from collections.abc import Awaitable, Callable
 
 import safir.dependencies.logger
 from fastapi import FastAPI, Request, Response
 from fastapi.middleware.gzip import GZipMiddleware
-from fastapi.responses import JSONResponse
-from lsst.daf.butler import MissingDatasetTypeError
 from safir.logging import configure_logging, configure_uvicorn_logging
 
-from ..server_models import CLIENT_REQUEST_ID_HEADER_NAME
+from ..._exceptions import ButlerUserError
+from ..server_models import CLIENT_REQUEST_ID_HEADER_NAME, ERROR_STATUS_CODE, ErrorResponseModel
 from .handlers._external import external_router
 from .handlers._internal import internal_router
 
 configure_logging(name="lsst.daf.butler.remote_butler.server")
 configure_uvicorn_logging()
 
 
@@ -52,15 +51,21 @@
     app.add_middleware(GZipMiddleware, minimum_size=1000)
 
     # A single instance of the server can serve data from multiple Butler
     # repositories.  This 'repository' path placeholder is consumed by
     # factory_dependency().
     repository_placeholder = "{repository}"
     default_api_path = "/api/butler"
-    app.include_router(external_router, prefix=f"{default_api_path}/repo/{repository_placeholder}")
+    app.include_router(
+        external_router,
+        prefix=f"{default_api_path}/repo/{repository_placeholder}",
+        # document that 422 responses will include a JSON-formatted error
+        # message, from `butler_exception_handler()` below.
+        responses={422: {"model": ErrorResponseModel}},
+    )
     app.include_router(internal_router)
 
     # Any time an exception is returned by a handler, add a log message that
     # includes the username and request ID from the client.  This will make it
     # easier to track down user-reported issues in the logs.
     #
     # This middleware is higher in the middleware stack than FastAPI's
@@ -79,20 +84,19 @@
                 "Exception",
                 exc_info=e,
                 clientRequestId=request.headers.get(CLIENT_REQUEST_ID_HEADER_NAME, "(unknown)"),
                 user=request.headers.get("X-Auth-Request-User", "(unknown)"),
             )
             raise
 
-    @app.exception_handler(MissingDatasetTypeError)
-    def missing_dataset_type_exception_handler(
-        request: Request, exc: MissingDatasetTypeError
-    ) -> JSONResponse:
-        # Remove the double quotes around the string form. These confuse
-        # the JSON serialization when single quotes are in the message.
-        message = str(exc).strip('"')
-        return JSONResponse(
-            status_code=404,
-            content={"detail": message, "exception": "MissingDatasetTypeError"},
+    # Configure FastAPI to forward to the client any exceptions tagged as
+    # user-facing Butler errors.
+    @app.exception_handler(ButlerUserError)
+    async def butler_exception_handler(request: Request, exc: ButlerUserError) -> Response:
+        error = ErrorResponseModel(error_type=exc.error_type, detail=str(exc))
+        return Response(
+            media_type="application/json",
+            status_code=ERROR_STATUS_CODE,
+            content=error.model_dump_json(),
         )
 
     return app
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_external.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/handlers/_external.py`

 * *Files 20% similar despite different names*

```diff
@@ -27,24 +27,29 @@
 
 __all__ = ()
 
 import uuid
 from typing import Any
 
 from fastapi import APIRouter, Depends
-from lsst.daf.butler import Butler, DatasetRef, SerializedDatasetRef, SerializedDatasetType, Timespan
+from lsst.daf.butler import Butler, CollectionType, DatasetRef, SerializedDatasetRef, SerializedDatasetType
+from lsst.daf.butler.registry.interfaces import ChainedCollectionRecord
 from lsst.daf.butler.remote_butler.server_models import (
     FindDatasetRequestModel,
     FindDatasetResponseModel,
+    GetCollectionInfoResponseModel,
+    GetCollectionSummaryResponseModel,
     GetFileByDataIdRequestModel,
     GetFileResponseModel,
+    QueryCollectionsRequestModel,
+    QueryCollectionsResponseModel,
 )
 
+from ...._exceptions import DatasetNotFoundError
 from .._dependencies import factory_dependency
-from .._exceptions import NotFoundException
 from .._factory import Factory
 
 external_router = APIRouter()
 
 
 @external_router.get(
     "/butler.yaml",
@@ -128,20 +133,19 @@
 )
 def find_dataset(
     dataset_type: str,
     query: FindDatasetRequestModel,
     factory: Factory = Depends(factory_dependency),
 ) -> FindDatasetResponseModel:
     butler = factory.create_butler()
-    timespan = Timespan.from_simple(query.timespan) if query.timespan is not None else None
     ref = butler.find_dataset(
         dataset_type,
         query.data_id,
         collections=query.collections,
-        timespan=timespan,
+        timespan=query.timespan,
         dimension_records=query.dimension_records,
         datastore_records=query.datastore_records,
     )
     serialized_ref = ref.to_simple() if ref else None
     return FindDatasetResponseModel(dataset_ref=serialized_ref)
 
 
@@ -153,37 +157,85 @@
 def get_file(
     dataset_id: uuid.UUID,
     factory: Factory = Depends(factory_dependency),
 ) -> GetFileResponseModel:
     butler = factory.create_butler()
     ref = butler.get_dataset(dataset_id, datastore_records=True)
     if ref is None:
-        raise NotFoundException(f"Dataset ID {dataset_id} not found")
+        raise DatasetNotFoundError(f"Dataset ID {dataset_id} not found")
     return _get_file_by_ref(butler, ref)
 
 
 @external_router.post(
     "/v1/get_file_by_data_id",
     summary="Lookup via DataId (metadata key/value pairs) the information needed to download"
     " and use the files associated with a dataset.",
 )
 def get_file_by_data_id(
     request: GetFileByDataIdRequestModel,
     factory: Factory = Depends(factory_dependency),
 ) -> GetFileResponseModel:
     butler = factory.create_butler()
-    try:
-        ref = butler._findDatasetRef(
-            datasetRefOrType=request.dataset_type_name,
-            dataId=request.data_id,
-            collections=request.collections,
-            datastore_records=True,
-        )
-        return _get_file_by_ref(butler, ref)
-    except LookupError as e:
-        raise NotFoundException() from e
+    ref = butler._findDatasetRef(
+        datasetRefOrType=request.dataset_type_name,
+        dataId=request.data_id,
+        collections=request.collections,
+        datastore_records=True,
+        timespan=request.timespan,
+    )
+    return _get_file_by_ref(butler, ref)
 
 
 def _get_file_by_ref(butler: Butler, ref: DatasetRef) -> GetFileResponseModel:
     """Return file information associated with ``ref``."""
     payload = butler._datastore.prepare_get_for_external_client(ref)
     return GetFileResponseModel(dataset_ref=ref.to_simple(), artifact=payload)
+
+
+@external_router.get(
+    "/v1/collection_info", summary="Get information about a collection", response_model_exclude_unset=True
+)
+def get_collection_info(
+    name: str,
+    include_doc: bool = False,
+    include_parents: bool = False,
+    factory: Factory = Depends(factory_dependency),
+) -> GetCollectionInfoResponseModel:
+    butler = factory.create_butler()
+    record = butler._registry.get_collection_record(name)
+    if record.type == CollectionType.CHAINED:
+        assert isinstance(record, ChainedCollectionRecord)
+        children = record.children
+    else:
+        children = ()
+    response = GetCollectionInfoResponseModel(name=record.name, type=record.type, children=children)
+    if include_doc:
+        response.doc = butler._registry.getCollectionDocumentation(name)
+    if include_parents:
+        response.parents = butler._registry.getCollectionParentChains(name)
+    return response
+
+
+@external_router.get(
+    "/v1/collection_summary", summary="Get summary information about the datasets in a collection"
+)
+def get_collection_summary(
+    name: str, factory: Factory = Depends(factory_dependency)
+) -> GetCollectionSummaryResponseModel:
+    butler = factory.create_butler()
+    return GetCollectionSummaryResponseModel(summary=butler.registry.getCollectionSummary(name).to_simple())
+
+
+@external_router.post(
+    "/v1/query_collections", summary="Search for collections with names that match an expression"
+)
+def query_collections(
+    request: QueryCollectionsRequestModel, factory: Factory = Depends(factory_dependency)
+) -> QueryCollectionsResponseModel:
+    butler = factory.create_butler()
+    collections = butler.registry.queryCollections(
+        expression=request.search,
+        collectionTypes=request.collection_types,
+        flattenChains=request.flatten_chains,
+        includeChains=request.include_chains,
+    )
+    return QueryCollectionsResponseModel(collections=collections)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/remote_butler/server/handlers/_internal.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/remote_butler/server_models.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/server_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -21,70 +21,54 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Models used for client/server communication."""
 
-__all__ = [
-    "CLIENT_REQUEST_ID_HEADER_NAME",
-    "CollectionList",
-    "DatasetTypeName",
-    "FindDatasetRequestModel",
-    "FindDatasetResponseModel",
-    "GetFileResponseModel",
-]
+import re
+from typing import Any
 
-from typing import NewType
+from fastapi import FastAPI, HTTPException, Request, Response
 
-import pydantic
-from lsst.daf.butler import SerializedDataId, SerializedDatasetRef, SerializedTimespan
-from lsst.daf.butler.datastores.fileDatastoreClient import FileDatastoreGetPayload
 
-CLIENT_REQUEST_ID_HEADER_NAME = "X-Butler-Client-Request-Id"
+def add_auth_header_check_middleware(app: FastAPI) -> None:
+    """Add a middleware to a FastAPI app to check that Gafaelfawr
+    authentication headers are present.
 
-CollectionList = NewType("CollectionList", list[str])
-"""A list of search patterns for collection names.  May use glob
-syntax to specify wildcards."""
-DatasetTypeName = NewType("DatasetTypeName", str)
+    This is only suitable for testing -- in a real deployment,
+    GafaelfawrIngress will handle these headers and convert them to a different
+    format.
 
+    Parameters
+    ----------
+    app : `FastAPI`
+        The app the middleware will be added to.
+    """
 
-class FindDatasetRequestModel(pydantic.BaseModel):
-    """Request model for find_dataset."""
-
-    data_id: SerializedDataId
-    collections: CollectionList
-    timespan: SerializedTimespan | None
-    dimension_records: bool = False
-    datastore_records: bool = False
-
-
-class FindDatasetResponseModel(pydantic.BaseModel):
-    """Response model for find_dataset."""
-
-    dataset_ref: SerializedDatasetRef | None
-
-
-class GetFileByDataIdRequestModel(pydantic.BaseModel):
-    """Request model for ``get_file_by_data_id``."""
-
-    dataset_type_name: DatasetTypeName
-    data_id: SerializedDataId
-    collections: CollectionList
-
-
-class GetFileResponseModel(pydantic.BaseModel):
-    """Response model for get_file and get_file_by_data_id."""
-
-    dataset_ref: SerializedDatasetRef
-    artifact: FileDatastoreGetPayload | None
-    """The data needed to retrieve and use an artifact. If this is `None`, that
-    means this dataset is known to the Butler but the associated files are no
-    longer available ("known to registry but not known to datastore".)
-
-    An example of a situation where this would be `None` is a per-visit image
-    that is an intermediate file in the processing pipelines.  It is deleted to
-    save space, but the fact that it was once available must be recorded for
-    provenance tracking.
+    @app.middleware("http")
+    async def check_auth_headers(request: Request, call_next: Any) -> Response:
+        if _is_authenticated_endpoint(request.url.path):
+            header = request.headers.get("authorization")
+            if header is None:
+                raise HTTPException(status_code=401, detail="Authorization header is missing")
+            if not re.match(r"^Bearer \S+", header):
+                raise HTTPException(
+                    status_code=401, detail=f"Authorization header not in expected format: {header}"
+                )
+
+        return await call_next(request)
+
+
+def _is_authenticated_endpoint(path: str) -> bool:
+    """Return True if the specified path requires authentication in the real
+    server deployment.
     """
+    if path == "/":
+        return False
+    if path.endswith("/butler.yaml"):
+        return False
+    if path.endswith("/butler.json"):
+        return False
+
+    return True
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/repo_relocation.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/repo_relocation.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_associate.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/_associate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/_pruneDatasets.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/_pruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/butlerImport.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/butlerImport.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/certifyCalibrations.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/certifyCalibrations.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configDump.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/configDump.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/configValidate.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/configValidate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/createRepo.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/createRepo.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/exportCalibs.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/exportCalibs.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/ingest_files.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/ingest_files.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryCollections.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDataIds.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasetTypes.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDatasetTypes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDatasets.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_datasetsHelper.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,206 +20,199 @@
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
-from __future__ import annotations
-
-import dataclasses
-from collections import defaultdict
-from collections.abc import Iterable
-from types import EllipsisType
-from typing import TYPE_CHECKING
 
-import numpy as np
-from astropy.table import Table as AstropyTable
+from __future__ import annotations
 
-from .._butler import Butler
-from ..cli.utils import sortAstropyTable
+__all__ = (
+    "DatasetTestHelper",
+    "DatastoreTestHelper",
+    "BadWriteFormatter",
+    "BadNoWriteFormatter",
+    "MultiDetectorFormatter",
+)
+
+import os
+from collections.abc import Iterable, Mapping
+from typing import TYPE_CHECKING, Any
+
+from lsst.daf.butler import DataCoordinate, DatasetRef, DatasetType, DimensionGroup, StorageClass
+from lsst.daf.butler.datastore import Datastore
+from lsst.daf.butler.formatters.yaml import YamlFormatter
 
 if TYPE_CHECKING:
-    from lsst.daf.butler import DatasetRef
-    from lsst.daf.butler.registry.queries import DatasetQueryResults
-    from lsst.resources import ResourcePath
-
+    from lsst.daf.butler import Config, DatasetId, Dimension, DimensionGraph
 
-@dataclasses.dataclass(frozen=True)
-class _RefInfo:
-    datasetRef: DatasetRef
-    uri: str | None
 
+class DatasetTestHelper:
+    """Helper methods for Datasets."""
 
-class _Table:
-    """Aggregates rows for a single dataset type, and creates an astropy table
-    with the aggregated data. Eliminates duplicate rows.
-    """
+    def makeDatasetRef(
+        self,
+        datasetTypeName: str,
+        dimensions: DimensionGroup | DimensionGraph | Iterable[str | Dimension],
+        storageClass: StorageClass | str,
+        dataId: DataCoordinate | Mapping[str, Any],
+        *,
+        id: DatasetId | None = None,
+        run: str | None = None,
+        conform: bool = True,
+    ) -> DatasetRef:
+        """Make a DatasetType and wrap it in a DatasetRef for a test.
 
-    datasetRefs: set[_RefInfo]
+        Parameters
+        ----------
+        datasetTypeName : `str`
+            The name of the dataset type.
+        dimensions : `DimensionGroup` or `~collections.abc.Iterable` of `str` \
+                or `Dimension`
+            The dimensions to use for this dataset type.
+        storageClass : `StorageClass` or `str`
+            The relevant storage class.
+        dataId : `DataCoordinate` or `~collections.abc.Mapping`
+            The data ID of this ref.
+        id : `DatasetId` or `None`, optional
+            The Id of this ref. Will be assigned automatically.
+        run : `str` or `None`, optional
+            The run for this ref. Will be assigned a default value if `None`.
+        conform : `bool`, optional
+            Whther to force the dataID to be checked for conformity with
+            the provided dimensions.
 
-    def __init__(self) -> None:
-        self.datasetRefs = set()
+        Returns
+        -------
+        ref : `DatasetRef`
+            The new ref.
+        """
+        return self._makeDatasetRef(
+            datasetTypeName,
+            dimensions,
+            storageClass,
+            dataId,
+            id=id,
+            run=run,
+            conform=conform,
+        )
 
-    def add(self, datasetRef: DatasetRef, uri: ResourcePath | None = None) -> None:
-        """Add a row of information to the table.
+    def _makeDatasetRef(
+        self,
+        datasetTypeName: str,
+        dimensions: DimensionGroup | DimensionGraph | Iterable[str | Dimension],
+        storageClass: StorageClass | str,
+        dataId: DataCoordinate | Mapping,
+        *,
+        id: DatasetId | None = None,
+        run: str | None = None,
+        conform: bool = True,
+    ) -> DatasetRef:
+        # helper for makeDatasetRef
+
+        # Pretend we have a parent if this looks like a composite
+        compositeName, componentName = DatasetType.splitDatasetTypeName(datasetTypeName)
+        parentStorageClass = StorageClass("component") if componentName else None
+
+        datasetType = DatasetType(
+            datasetTypeName, dimensions, storageClass, parentStorageClass=parentStorageClass
+        )
+
+        if run is None:
+            run = "dummy"
+        if not isinstance(dataId, DataCoordinate):
+            dataId = DataCoordinate.standardize(dataId, dimensions=datasetType.dimensions)
+        return DatasetRef(datasetType, dataId, id=id, run=run, conform=conform)
+
+
+class DatastoreTestHelper:
+    """Helper methods for Datastore tests."""
+
+    root: str | None
+    config: Config
+    datastoreType: type[Datastore]
+    configFile: str
 
-        ``uri`` is optional but must be the consistent; provided or not, for
-        every call to a ``_Table`` instance.
+    def setUpDatastoreTests(self, registryClass: type, configClass: type[Config]) -> None:
+        """Shared setUp code for all Datastore tests.
 
         Parameters
         ----------
-        datasetRef : `DatasetRef`
-            A dataset ref that will be added as a row in the table.
-        uri : `lsst.resources.ResourcePath`, optional
-            The URI to show as a file location in the table, by default `None`.
+        registryClass : `type`
+            Type of registry to use.
+        configClass : `type`
+            Type of config to use.
         """
-        uri_str = str(uri) if uri else None
-        self.datasetRefs.add(_RefInfo(datasetRef, uri_str))
+        self.registry = registryClass()
+        self.config = configClass(self.configFile)
+
+        # Some subclasses override the working root directory
+        if self.root is not None:
+            self.datastoreType.setConfigRoot(self.root, self.config, self.config.copy())
 
-    def getAstropyTable(self, datasetTypeName: str) -> AstropyTable:
-        """Get the table as an astropy table.
+    def makeDatastore(self, sub: str | None = None) -> Datastore:
+        """Make a new Datastore instance of the appropriate type.
 
         Parameters
         ----------
-        datasetTypeName : `str`
-            The dataset type name to show in the ``type`` column of the table.
+        sub : `str`, optional
+            If not None, the returned Datastore will be distinct from any
+            Datastore constructed with a different value of ``sub``.  For
+            PosixDatastore, for example, the converse is also true, and ``sub``
+            is used as a subdirectory to form the new root.
 
         Returns
         -------
-        table : `astropy.table._Table`
-            The table with the provided column names and rows.
+        datastore : `Datastore`
+            Datastore constructed by this routine using the supplied
+            optional subdirectory if supported.
         """
-        # Should never happen; adding a dataset should be the action that
-        # causes a _Table to be created.
-        if not self.datasetRefs:
-            raise RuntimeError(f"No DatasetRefs were provided for dataset type {datasetTypeName}")
-
-        refInfo = next(iter(self.datasetRefs))
-        dimensions = [
-            refInfo.datasetRef.dataId.universe.dimensions[k]
-            for k in refInfo.datasetRef.dataId.dimensions.data_coordinate_keys
-        ]
-        columnNames = ["type", "run", "id", *[str(item) for item in dimensions]]
-
-        # Need to hint the column types for numbers since the per-row
-        # constructor of Table does not work this out on its own and sorting
-        # will not work properly without.
-        typeMap = {float: np.float64, int: np.int64}
-        columnTypes = [
-            None,
-            None,
-            str,
-            *[typeMap.get(type(value)) for value in refInfo.datasetRef.dataId.full_values],
-        ]
-        if refInfo.uri:
-            columnNames.append("URI")
-            columnTypes.append(None)
-
-        rows = []
-        for refInfo in self.datasetRefs:
-            row = [
-                datasetTypeName,
-                refInfo.datasetRef.run,
-                str(refInfo.datasetRef.id),
-                *refInfo.datasetRef.dataId.full_values,
-            ]
-            if refInfo.uri:
-                row.append(refInfo.uri)
-            rows.append(row)
-
-        dataset_table = AstropyTable(np.array(rows), names=columnNames, dtype=columnTypes)
-        return sortAstropyTable(dataset_table, dimensions, ["type", "run"])
-
-
-class QueryDatasets:
-    """Get dataset refs from a repository.
-
-    Parameters
-    ----------
-    glob : iterable [`str`]
-        A list of glob-style search string that fully or partially identify
-        the dataset type names to search for.
-    collections : iterable [`str`]
-        A list of glob-style search string that fully or partially identify
-        the collections to search for.
-    where : `str`
-        A string expression similar to a SQL WHERE clause.  May involve any
-        column of a dimension table or (as a shortcut for the primary key
-        column of a dimension table) dimension name.
-    find_first : `bool`
-        For each result data ID, only yield one DatasetRef of each DatasetType,
-        from the first collection in which a dataset of that dataset type
-        appears (according to the order of `collections` passed in).  If used,
-        `collections` must specify at least one expression and must not contain
-        wildcards.
-    show_uri : `bool`
-        If True, include the dataset URI in the output.
-    repo : `str` or `None`
-        URI to the location of the repo or URI to a config file describing the
-        repo and its location. One of `repo` and `butler` must be `None` and
-        the other must not be `None`.
-    butler : `lsst.daf.butler.Butler` or `None`
-        The butler to use to query. One of `repo` and `butler` must be `None`
-        and the other must not be `None`.
-    """
+        config = self.config.copy()
+        if sub is not None and self.root is not None:
+            self.datastoreType.setConfigRoot(os.path.join(self.root, sub), config, self.config)
+        if sub is not None:
+            # Ensure that each datastore gets its own registry
+            registryClass = type(self.registry)
+            registry = registryClass()
+        else:
+            registry = self.registry
+        return Datastore.fromConfig(config=config, bridgeManager=registry.getDatastoreBridgeManager())
 
-    def __init__(
-        self,
-        glob: Iterable[str],
-        collections: Iterable[str],
-        where: str,
-        find_first: bool,
-        show_uri: bool,
-        repo: str | None = None,
-        butler: Butler | None = None,
-    ):
-        if (repo and butler) or (not repo and not butler):
-            raise RuntimeError("One of repo and butler must be provided and the other must be None.")
-        # show_uri requires a datastore.
-        without_datastore = not show_uri
-        self.butler = butler or Butler.from_config(repo, without_datastore=without_datastore)
-        self._getDatasets(glob, collections, where, find_first)
-        self.showUri = show_uri
-
-    def _getDatasets(
-        self, glob: Iterable[str], collections: Iterable[str], where: str, find_first: bool
-    ) -> None:
-        datasetTypes = glob or ...
-        query_collections: Iterable[str] | EllipsisType = collections or ...
-
-        self.datasets = self.butler.registry.queryDatasets(
-            datasetType=datasetTypes, collections=query_collections, where=where, findFirst=find_first
-        ).expanded()
 
-    def getTables(self) -> list[AstropyTable]:
-        """Get the datasets as a list of astropy tables.
+class BadWriteFormatter(YamlFormatter):
+    """A formatter that never works but does leave a file behind."""
 
-        Returns
-        -------
-        datasetTables : `list` [``astropy.table._Table``]
-            A list of astropy tables, one for each dataset type.
-        """
-        tables: dict[str, _Table] = defaultdict(_Table)
-        if not self.showUri:
-            for dataset_ref in self.datasets:
-                tables[dataset_ref.datasetType.name].add(dataset_ref)
-        else:
-            d = list(self.datasets)
-            ref_uris = self.butler.get_many_uris(d, predict=True)
-            for ref, uris in ref_uris.items():
-                if uris.primaryURI:
-                    tables[ref.datasetType.name].add(ref, uris.primaryURI)
-                for name, uri in uris.componentURIs.items():
-                    tables[ref.datasetType.componentTypeName(name)].add(ref, uri)
+    def _readFile(self, path: str, pytype: type[Any] | None = None) -> Any:
+        raise NotImplementedError("This formatter can not read anything")
 
-        return [table.getAstropyTable(datasetTypeName) for datasetTypeName, table in tables.items()]
+    def _writeFile(self, inMemoryDataset: Any) -> None:
+        """Write an empty file and then raise an exception."""
+        with open(self.fileDescriptor.location.path, "wb"):
+            pass
+        raise RuntimeError("Did not succeed in writing file")
 
-    def getDatasets(self) -> DatasetQueryResults:
-        """Get the datasets as a list of ``DatasetQueryResults``.
 
-        Returns
-        -------
-        refs : `lsst.daf.butler.registry.queries.DatasetQueryResults`
-            Dataset references matching the given query criteria.
-        """
-        return self.datasets
+class BadNoWriteFormatter(BadWriteFormatter):
+    """A formatter that always fails without writing anything."""
+
+    def _writeFile(self, inMemoryDataset: Any) -> None:
+        raise RuntimeError("Did not writing anything at all")
+
+
+class MultiDetectorFormatter(YamlFormatter):
+    """A formatter that requires a detector to be specified in the dataID."""
+
+    def _writeFile(self, inMemoryDataset: Any) -> None:
+        raise NotImplementedError("Can not write")
+
+    def _fromBytes(self, serializedDataset: bytes, pytype: type[Any] | None = None) -> Any:
+        data = super()._fromBytes(serializedDataset)
+        if self.dataId is None:
+            raise RuntimeError("This formatter requires a dataId")
+        if "detector" not in self.dataId:
+            raise RuntimeError("This formatter requires detector to be present in dataId")
+        key = f"detector{self.dataId['detector']}"
+        assert pytype is not None
+        if key in data:
+            return pytype(data[key])
+        raise RuntimeError(f"Could not find '{key}' in data file")
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/queryDimensionRecords.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/queryDimensionRecords.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/register_dataset_type.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/register_dataset_type.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeCollections.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/removeCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeDatasetType.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/removeDatasetType.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/removeRuns.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/removeRuns.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/retrieveArtifacts.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/retrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/script/transferDatasets.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/script/transferDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_dummyRegistry.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_dummyRegistry.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_examplePythonTypes.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/_examplePythonTypes.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/_testRepo.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/direct_query_driver/_query_builder.py`

 * *Files 24% similar despite different names*

```diff
@@ -23,570 +23,549 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
-__all__ = [
-    "makeTestRepo",
-    "makeTestCollection",
-    "addDatasetType",
-    "expandUniqueId",
-    "DatastoreMock",
-    "addDataIdValue",
-]
-
-import random
-from collections.abc import Iterable, Mapping
-from typing import TYPE_CHECKING, Any
-from unittest.mock import MagicMock
+__all__ = ("QueryJoiner", "QueryBuilder")
+
+import dataclasses
+import itertools
+from collections.abc import Iterable, Sequence
+from typing import TYPE_CHECKING, Any, ClassVar
 
 import sqlalchemy
-from lsst.daf.butler import (
-    Butler,
-    Config,
-    DataCoordinate,
-    DatasetRef,
-    DatasetType,
-    Dimension,
-    DimensionUniverse,
-    FileDataset,
-    StorageClass,
-)
+
+from .. import ddl
+from ..name_shrinker import NameShrinker
+from ..nonempty_mapping import NonemptyMapping
+from ..queries import tree as qt
+from ._postprocessing import Postprocessing
 
 if TYPE_CHECKING:
-    from lsst.daf.butler import DatasetId
+    from ..registry.interfaces import Database
+    from ..timespan_database_representation import TimespanDatabaseRepresentation
 
 
-def makeTestRepo(
-    root: str, dataIds: Mapping[str, Iterable] | None = None, *, config: Config | None = None, **kwargs: Any
-) -> Butler:
-    """Create an empty test repository.
-
-    Parameters
-    ----------
-    root : `str`
-        The location of the root directory for the repository.
-    dataIds : `~collections.abc.Mapping` [`str`, `iterable`], optional
-        A mapping keyed by the dimensions used in the test. Each value is an
-        iterable of names for that dimension (e.g., detector IDs for
-        `"detector"`). Related dimensions (e.g., instruments and detectors) are
-        linked arbitrarily, with values created for implied dimensions only
-        when needed. This parameter is provided for compatibility with old
-        code; newer code should make the repository, then call
-        `~lsst.daf.butler.tests.addDataIdValue`.
-    config : `lsst.daf.butler.Config`, optional
-        A configuration for the repository (for details, see
-        `lsst.daf.butler.Butler.makeRepo`). If omitted, creates a repository
-        with default dataset and storage types, but optimized for speed.  The
-        defaults set ``.datastore.cls``, ``.datastore.checksum`` and
-        ``.registry.db``.  If a supplied config does not specify these values
-        the internal defaults will be used to ensure that we have a usable
-        configuration.
-    **kwargs
-        Extra arguments to `lsst.daf.butler.Butler.makeRepo`.
-
-    Returns
-    -------
-    butler : `lsst.daf.butler.Butler`
-        A Butler referring to the new repository. This Butler is provided only
-        for additional setup; to keep test cases isolated, it is highly
-        recommended that each test create its own Butler with a unique
-        run/collection. See `makeTestCollection`.
-
-    Notes
-    -----
-    This function provides a "quick and dirty" repository for simple unit tests
-    that don't depend on complex data relationships. It is ill-suited for tests
-    where the structure of the data matters. If you need such a dataset, create
-    it directly or use a saved test dataset.
-    """
-    defaults = Config()
-    defaults["datastore", "cls"] = "lsst.daf.butler.datastores.inMemoryDatastore.InMemoryDatastore"
-    defaults["datastore", "checksum"] = False  # In case of future changes
-    defaults["registry", "db"] = "sqlite:///<butlerRoot>/gen3.sqlite3"
-
-    if config:
-        defaults.update(config)
-
-    if not dataIds:
-        dataIds = {}
-
-    # Disable config root by default so that our registry override will
-    # not be ignored.
-    # newConfig guards against location-related keywords like outfile
-    newConfig = Butler.makeRepo(root, config=defaults, forceConfigRoot=False, **kwargs)
-    butler = Butler.from_config(newConfig, writeable=True)
-    dimensionRecords = _makeRecords(dataIds, butler.dimensions)
-    for dimension, records in dimensionRecords.items():
-        if butler.dimensions[dimension].has_own_table:
-            butler.registry.insertDimensionData(dimension, *records)
-    return butler
-
-
-def makeTestCollection(repo: Butler, uniqueId: str | None = None) -> Butler:
-    """Create a read/write Butler to a fresh collection.
-
-    Parameters
-    ----------
-    repo : `lsst.daf.butler.Butler`
-        A previously existing Butler to a repository, such as that returned by
-        `~lsst.daf.butler.Butler.makeRepo` or `makeTestRepo`.
-    uniqueId : `str`, optional
-        A collection ID guaranteed by external code to be unique across all
-        calls to ``makeTestCollection`` for the same repository.
-
-    Returns
-    -------
-    butler : `lsst.daf.butler.Butler`
-        A Butler referring to a new collection in the repository at ``root``.
-        The collection is (almost) guaranteed to be new.
-
-    Notes
-    -----
-    This function creates a single run collection that does not necessarily
-    conform to any repository conventions. It is only suitable for creating an
-    isolated test area, and not for repositories intended for real data
-    processing or analysis.
-    """
-    if not uniqueId:
-        # Create a "random" collection name
-        # Speed matters more than cryptographic guarantees
-        uniqueId = str(random.randrange(1_000_000_000))
-    collection = "test_" + uniqueId
-    return Butler.from_config(butler=repo, run=collection)
-
-
-def _makeRecords(dataIds: Mapping[str, Iterable], universe: DimensionUniverse) -> Mapping[str, Iterable]:
-    """Create cross-linked dimension records from a collection of
-    data ID values.
-
-    Parameters
-    ----------
-    dataIds : `~collections.abc.Mapping` [`str`, `iterable`]
-        A mapping keyed by the dimensions of interest. Each value is an
-        iterable of names for that dimension (e.g., detector IDs for
-        `"detector"`).
-    universe : lsst.daf.butler.DimensionUniverse
-        Set of all known dimensions and their relationships.
-
-    Returns
-    -------
-    dataIds : `~collections.abc.Mapping` [`str`, `iterable`]
-        A mapping keyed by the dimensions of interest, giving one
-        `~lsst.daf.butler.DimensionRecord` for each input name. Related
-        dimensions (e.g., instruments and detectors) are linked arbitrarily.
-    """
-    # Create values for all dimensions that are (recursive) required or implied
-    # dependencies of the given ones.
-    complete_data_id_values = {}
-    for dimension_name in universe.conform(dataIds.keys()).names:
-        if dimension_name in dataIds:
-            complete_data_id_values[dimension_name] = list(dataIds[dimension_name])
-        if dimension_name not in complete_data_id_values:
-            complete_data_id_values[dimension_name] = [
-                _makeRandomDataIdValue(universe.dimensions[dimension_name])
-            ]
+@dataclasses.dataclass
+class QueryBuilder:
+    """A struct used to represent an under-construction SQL SELECT query.
+
+    This object's methods frequently "consume" ``self``, by either returning
+    it after modification or returning related copy that may share state with
+    the original.  Users should be careful never to use consumed instances, and
+    are recommended to reuse the same variable name to make that hard to do
+    accidentally.
+    """
+
+    joiner: QueryJoiner
+    """Struct representing the SQL FROM and WHERE clauses, as well as the
+    columns *available* to the query (but not necessarily in the SELECT
+    clause).
+    """
+
+    columns: qt.ColumnSet
+    """Columns to include the SELECT clause.
+
+    This does not include columns required only by `postprocessing` and columns
+    in `QueryJoiner.special`, which are also always included in the SELECT
+    clause.
+    """
+
+    postprocessing: Postprocessing = dataclasses.field(default_factory=Postprocessing)
+    """Postprocessing that will be needed in Python after the SQL query has
+    been executed.
+    """
+
+    distinct: bool | Sequence[sqlalchemy.ColumnElement[Any]] = ()
+    """A representation of a DISTINCT or DISTINCT ON clause.
 
-    # Start populating dicts that will become DimensionRecords by providing
-    # alternate keys like detector names
-    record_dicts_by_dimension_name: dict[str, list[dict[str, str | int | bytes]]] = {}
-    for name, values in complete_data_id_values.items():
-        record_dicts_by_dimension_name[name] = []
-        dimension_el = universe[name]
-        for value in values:
-            # _fillAllKeys wants Dimension and not DimensionElement.
-            # universe.__getitem__ says it returns DimensionElement but this
-            # really does also seem to be a Dimension here.
-            record_dicts_by_dimension_name[name].append(
-                _fillAllKeys(dimension_el, value)  # type: ignore[arg-type]
-            )
-
-    # Pick cross-relationships arbitrarily
-    for name, record_dicts in record_dicts_by_dimension_name.items():
-        dimension_el = universe[name]
-        for record_dict in record_dicts:
-            for other in dimension_el.dimensions:
-                if other != dimension_el:
-                    relation = record_dicts_by_dimension_name[other.name][0]
-                    record_dict[other.name] = relation[other.primaryKey.name]
-
-    return {
-        dimension: [universe[dimension].RecordClass(**record_dict) for record_dict in record_dicts]
-        for dimension, record_dicts in record_dicts_by_dimension_name.items()
-    }
-
-
-def _fillAllKeys(dimension: Dimension, value: str | int) -> dict[str, str | int | bytes]:
-    """Create an arbitrary mapping of all required keys for a given dimension
-    that do not refer to other dimensions.
-
-    Parameters
-    ----------
-    dimension : `lsst.daf.butler.Dimension`
-        The dimension for which to generate a set of keys (e.g., detector).
-    value
-        The value assigned to ``dimension`` (e.g., detector ID).
-
-    Returns
-    -------
-    expandedValue : `dict` [`str`]
-        A mapping of dimension keys to values. ``dimension's`` primary key
-        maps to ``value``, but all other mappings (e.g., detector name)
-        are arbitrary.
-    """
-    expandedValue: dict[str, str | int | bytes] = {}
-    for key in dimension.uniqueKeys:
-        if key.nbytes:
-            # For `bytes` fields, we want something that casts at least `str`
-            # and `int` values to bytes and yields b'' when called with no
-            # arguments (as in the except block below).  Unfortunately, the
-            # `bytes` type itself fails for both `str` and `int`, but this
-            # lambda does what we need.  This particularly important for the
-            # skymap dimensions' bytes 'hash' field, which has a unique
-            # constraint; without this, all skymaps would get a hash of b''
-            # and end up conflicting.
-            castType = lambda *args: str(*args).encode()  # noqa: E731
-        else:
-            castType = key.dtype().python_type
-        try:
-            castValue = castType(value)
-        except TypeError:
-            castValue = castType()
-        expandedValue[key.name] = castValue
-    for key in dimension.metadata:
-        if not key.nullable:
-            expandedValue[key.name] = key.dtype().python_type(value)
-    return expandedValue
-
-
-def _makeRandomDataIdValue(dimension: Dimension) -> int | str:
-    """Generate a random value of the appropriate type for a data ID key.
-
-    Parameters
-    ----------
-    dimension : `Dimension`
-        Dimension the value corresponds to.
-
-    Returns
-    -------
-    value : `int` or `str`
-        Random value.
-    """
-    if dimension.primaryKey.getPythonType() is str:
-        return str(random.randrange(1000))
-    else:
-        return random.randrange(1000)
-
-
-def expandUniqueId(butler: Butler, partialId: Mapping[str, Any]) -> DataCoordinate:
-    """Return a complete data ID matching some criterion.
-
-    Parameters
-    ----------
-    butler : `lsst.daf.butler.Butler`
-        The repository to query.
-    partialId : `~collections.abc.Mapping` [`str`]
-        A mapping of known dimensions and values.
-
-    Returns
-    -------
-    dataId : `lsst.daf.butler.DataCoordinate`
-        The unique data ID that matches ``partialId``.
-
-    Raises
-    ------
-    ValueError
-        Raised if ``partialId`` does not uniquely identify a data ID.
-
-    Notes
-    -----
-    This method will only work correctly if all dimensions attached to the
-    target dimension (eg., "physical_filter" for "visit") are known to the
-    repository, even if they're not needed to identify a dataset. This function
-    is only suitable for certain kinds of test repositories, and not for
-    repositories intended for real data processing or analysis.
-
-    Examples
-    --------
-    .. code-block:: py
-
-       >>> butler = makeTestRepo(
-               "testdir", {"instrument": ["notACam"], "detector": [1]})
-       >>> expandUniqueId(butler, {"detector": 1})
-       DataCoordinate({instrument, detector}, ('notACam', 1))
-    """
-    # The example is *not* a doctest because it requires dangerous I/O
-    registry = butler.registry
-    dimensions = registry.dimensions.conform(partialId.keys()).required
-
-    query = " AND ".join(f"{dimension} = {value!r}" for dimension, value in partialId.items())
-
-    # Much of the purpose of this function is to do something we explicitly
-    # reject most of the time: query for a governor dimension (e.g. instrument)
-    # given something that depends on it (e.g. visit), hence check=False.
-    dataId = list(registry.queryDataIds(dimensions, where=query, check=False))
-    if len(dataId) == 1:
-        return dataId[0]
-    else:
-        raise ValueError(f"Found {len(dataId)} matches for {partialId}, expected 1.")
-
-
-def _findOrInventDataIdValue(
-    butler: Butler, data_id: dict[str, str | int], dimension: Dimension
-) -> tuple[str | int, bool]:
-    """Look up an arbitrary value for a dimension that is consistent with a
-    partial data ID that does not specify that dimension, or invent one if no
-    such value exists.
-
-    Parameters
-    ----------
-    butler : `Butler`
-        Butler to use to look up data ID values.
-    data_id : `dict` [ `str`, `str` or `int` ]
-        Dictionary of possibly-related data ID values.
-    dimension : `Dimension`
-        Dimension to obtain a value for.
-
-    Returns
-    -------
-    value : `int` or `str`
-        Value for this dimension.
-    invented : `bool`
-        `True` if the value had to be invented, `False` if a compatible value
-        already existed.
-    """
-    # No values given by caller for this dimension.  See if any exist
-    # in the registry that are consistent with the values of dimensions
-    # we do have:
-    match_data_id = {key: data_id[key] for key in data_id.keys() & dimension.dimensions.names}
-    matches = list(butler.registry.queryDimensionRecords(dimension, dataId=match_data_id).limit(1))
-    if not matches:
-        # Nothing in the registry matches: invent a data ID value
-        # with the right type (actual value does not matter).
-        # We may or may not actually make a record with this; that's
-        # easier to check later.
-        dimension_value = _makeRandomDataIdValue(dimension)
-        return dimension_value, True
-    else:
-        # A record does exist in the registry.  Use its data ID value.
-        dim_value = matches[0].dataId[dimension.name]
-        assert dim_value is not None
-        return dim_value, False
-
-
-def _makeDimensionRecordDict(data_id: dict[str, str | int], dimension: Dimension) -> dict[str, Any]:
-    """Create a dictionary that can be used to build a `DimensionRecord` that
-    is consistent with the given data ID.
-
-    Parameters
-    ----------
-    data_id : `dict` [ `str`, `str` or `int` ]
-        Dictionary that contains values for at least all of
-        ``dimension.dimensions.names`` (the main dimension, its recursive
-        required dependencies, and its non-recursive implied dependencies).
-    dimension : `Dimension`
-        Dimension to build a record dictionary for.
-
-    Returns
-    -------
-    record_dict : `dict` [ `str`, `object` ]
-        Dictionary that can be passed as ``**kwargs`` to this dimensions
-        record class constructor.
-    """
-    # Add the primary key field for this dimension.
-    record_dict: dict[str, Any] = {dimension.primaryKey.name: data_id[dimension.name]}
-    # Define secondary keys (e.g., detector name given detector id)
-    record_dict.update(_fillAllKeys(dimension, data_id[dimension.name]))
-    # Set the foreign key values for any related dimensions that should
-    # appear in the record.
-    for related_dimension in dimension.dimensions:
-        if related_dimension.name != dimension.name:
-            record_dict[related_dimension.name] = data_id[related_dimension.name]
-    return record_dict
-
-
-def addDataIdValue(butler: Butler, dimension: str, value: str | int, **related: str | int) -> None:
-    """Add the records that back a new data ID to a repository.
-
-    Parameters
-    ----------
-    butler : `lsst.daf.butler.Butler`
-        The repository to update.
-    dimension : `str`
-        The name of the dimension to gain a new value.
-    value : `str` or `int`
-        The value to register for the dimension.
-    **related : `typing.Any`
-        Any existing dimensions to be linked to ``value``.
-
-    Notes
-    -----
-    Related dimensions (e.g., the instrument associated with a detector) may be
-    specified using ``related``, which requires a value for those dimensions to
-    have been added to the repository already (generally with a previous call
-    to `addDataIdValue`.  Any dependencies of the given dimension that are not
-    included in ``related`` will be linked to existing values arbitrarily, and
-    (for implied dependencies only) created and also inserted into the registry
-    if they do not exist.  Values for required dimensions and those given in
-    ``related`` are never created.
-
-    Because this function creates filler data, it is only suitable for test
-    repositories. It should not be used for repositories intended for real data
-    processing or analysis, which have known dimension values.
-
-    Examples
-    --------
-    See the guide on :ref:`using-butler-in-tests-make-repo` for usage examples.
-    """
-    # Example is not doctest, because it's probably unsafe to create even an
-    # in-memory butler in that environment.
-    try:
-        full_dimension = butler.dimensions[dimension]
-    except KeyError as e:
-        raise ValueError from e
-    # Bad keys ignored by registry code
-    extra_keys = related.keys() - full_dimension.minimal_group.names
-    if extra_keys:
-        raise ValueError(
-            f"Unexpected keywords {extra_keys} not found in {full_dimension.minimal_group.names}"
+    If `True`, this represents a SELECT DISTINCT.  If a non-empty sequence,
+    this represents a SELECT DISTINCT ON.  If `False` or an empty sequence,
+    there is no DISTINCT clause.
+    """
+
+    group_by: Sequence[sqlalchemy.ColumnElement[Any]] = ()
+    """A representation of a GROUP BY clause.
+
+    If not-empty, a GROUP BY clause with these columns is added.  This
+    generally requires that every `sqlalchemy.ColumnElement` held in the nested
+    `joiner` that is part of `columns` must either be part of `group_by` or
+    hold an aggregate function.
+    """
+
+    EMPTY_COLUMNS_NAME: ClassVar[str] = "IGNORED"
+    """Name of the column added to a SQL SELECT clause in order to construct
+    queries that have no real columns.
+    """
+
+    EMPTY_COLUMNS_TYPE: ClassVar[type] = sqlalchemy.Boolean
+    """Type of the column added to a SQL SELECT clause in order to construct
+    queries that have no real columns.
+    """
+
+    @classmethod
+    def handle_empty_columns(
+        cls, columns: list[sqlalchemy.sql.ColumnElement]
+    ) -> list[sqlalchemy.ColumnElement]:
+        """Handle the edge case where a SELECT statement has no columns, by
+        adding a literal column that should be ignored.
+
+        Parameters
+        ----------
+        columns : `list` [ `sqlalchemy.ColumnElement` ]
+            List of SQLAlchemy column objects.  This may have no elements when
+            this method is called, and will always have at least one element
+            when it returns.
+
+        Returns
+        -------
+        columns : `list` [ `sqlalchemy.ColumnElement` ]
+            The same list that was passed in, after any modification.
+        """
+        if not columns:
+            columns.append(sqlalchemy.sql.literal(True).label(cls.EMPTY_COLUMNS_NAME))
+        return columns
+
+    def select(self) -> sqlalchemy.Select:
+        """Transform this builder into a SQLAlchemy representation of a SELECT
+        query.
+
+        Returns
+        -------
+        select : `sqlalchemy.Select`
+            SQLAlchemy SELECT statement.
+        """
+        assert not (self.distinct and self.group_by), "At most one of distinct and group_by can be set."
+        if self.joiner.name_shrinker is None:
+            self.joiner.name_shrinker = self.joiner._make_name_shrinker()
+        sql_columns: list[sqlalchemy.ColumnElement[Any]] = []
+        for logical_table, field in self.columns:
+            name = self.columns.get_qualified_name(logical_table, field)
+            if field is None:
+                sql_columns.append(self.joiner.dimension_keys[logical_table][0].label(name))
+            else:
+                name = self.joiner.name_shrinker.shrink(name)
+                if self.columns.is_timespan(logical_table, field):
+                    sql_columns.extend(self.joiner.timespans[logical_table].flatten(name))
+                else:
+                    sql_columns.append(self.joiner.fields[logical_table][field].label(name))
+        if self.postprocessing is not None:
+            for element in self.postprocessing.iter_missing(self.columns):
+                sql_columns.append(
+                    self.joiner.fields[element.name]["region"].label(
+                        self.joiner.name_shrinker.shrink(
+                            self.columns.get_qualified_name(element.name, "region")
+                        )
+                    )
+                )
+        for label, sql_column in self.joiner.special.items():
+            sql_columns.append(sql_column.label(label))
+        self.handle_empty_columns(sql_columns)
+        result = sqlalchemy.select(*sql_columns)
+        if self.joiner.from_clause is not None:
+            result = result.select_from(self.joiner.from_clause)
+        if self.distinct is True:
+            result = result.distinct()
+        elif self.distinct:
+            result = result.distinct(*self.distinct)
+        if self.group_by:
+            result = result.group_by(*self.group_by)
+        if self.joiner.where_terms:
+            result = result.where(*self.joiner.where_terms)
+        return result
+
+    def join(self, other: QueryJoiner) -> QueryBuilder:
+        """Join tables, subqueries, and WHERE clauses from another query into
+        this one, in place.
+
+        Parameters
+        ----------
+        other : `QueryJoiner`
+            Object holding the FROM and WHERE clauses to add to this one.
+            JOIN ON clauses are generated via the dimension keys in common.
+
+        Returns
+        -------
+        self : `QueryBuilder`
+            This `QueryBuilder` instance (never a copy); returned to enable
+            method-chaining.
+        """
+        self.joiner.join(other)
+        return self
+
+    def to_joiner(self, cte: bool = False, force: bool = False) -> QueryJoiner:
+        """Convert this builder into a `QueryJoiner`, nesting it in a subquery
+        or common table expression only if needed to apply DISTINCT or GROUP BY
+        clauses.
+
+        This method consumes ``self``.
+
+        Parameters
+        ----------
+        cte : `bool`, optional
+            If `True`, nest via a common table expression instead of a
+            subquery.
+        force : `bool`, optional
+            If `True`, nest via a subquery or common table expression even if
+            there is no DISTINCT or GROUP BY.
+
+        Returns
+        -------
+        joiner : `QueryJoiner`
+            QueryJoiner` with at least all columns in `columns` available.
+            This may or may not be the `joiner` attribute of this object.
+        """
+        if force or self.distinct or self.group_by:
+            sql_from_clause = self.select().cte() if cte else self.select().subquery()
+            return QueryJoiner(
+                self.joiner.db, sql_from_clause, name_shrinker=self.joiner.name_shrinker
+            ).extract_columns(self.columns, self.postprocessing, special=self.joiner.special.keys())
+        return self.joiner
+
+    def nested(self, cte: bool = False, force: bool = False) -> QueryBuilder:
+        """Convert this builder into a `QueryBuiler` that is guaranteed to have
+        no DISTINCT or GROUP BY, nesting it in a subquery or common table
+        expression only if needed to apply any current DISTINCT or GROUP BY
+        clauses.
+
+        This method consumes ``self``.
+
+        Parameters
+        ----------
+        cte : `bool`, optional
+            If `True`, nest via a common table expression instead of a
+            subquery.
+        force : `bool`, optional
+            If `True`, nest via a subquery or common table expression even if
+            there is no DISTINCT or GROUP BY.
+
+        Returns
+        -------
+        builder : `QueryBuilder`
+            `QueryBuilder` with at least all columns in `columns` available.
+            This may or may not be the `builder` attribute of this object.
+        """
+        return QueryBuilder(
+            self.to_joiner(cte=cte, force=force), columns=self.columns, postprocessing=self.postprocessing
         )
 
-    # Assemble a dictionary data ID holding the given primary dimension value
-    # and all of the related ones.
-    data_id: dict[str, int | str] = {dimension: value}
-    data_id.update(related)
-
-    # Compute the set of all dimensions that these recursively depend on.
-    all_dimensions = butler.dimensions.conform(data_id.keys())
-
-    # Create dicts that will become DimensionRecords for all of these data IDs.
-    # This iteration is guaranteed to be in topological order, so we can count
-    # on new data ID values being invented before they are needed.
-    record_dicts_by_dimension: dict[Dimension, dict[str, Any]] = {}
-    for dimension_name in all_dimensions.names:
-        dimension_obj = butler.dimensions.dimensions[dimension_name]
-        dimension_value = data_id.get(dimension_name)
-        if dimension_value is None:
-            data_id[dimension_name], invented = _findOrInventDataIdValue(butler, data_id, dimension_obj)
-            if not invented:
-                # No need to make a new record; one already exists.
-                continue
-        if dimension_name in related:
-            # Caller passed in a value of this dimension explicitly, but it
-            # isn't the primary dimension they asked to have a record created
-            # for.  That means they expect this record to already exist.
-            continue
-        if dimension_name != dimension and dimension_name in all_dimensions.required:
-            # We also don't want to automatically create new dimension records
-            # for required dimensions (except for the main dimension the caller
-            # asked for); those are also asserted by the caller to already
-            # exist.
-            continue
-        if not dimension_obj.has_own_table:
-            # Don't need to bother generating full records for dimensions whose
-            # records are not actually stored.
-            continue
-        record_dicts_by_dimension[dimension_obj] = _makeDimensionRecordDict(data_id, dimension_obj)
-
-    # Sync those dimension record dictionaries with the database.
-    for dimension_obj, record_dict in record_dicts_by_dimension.items():
-        record = dimension_obj.RecordClass(**record_dict)
-        try:
-            butler.registry.syncDimensionData(dimension_obj, record)
-        except sqlalchemy.exc.IntegrityError as e:
-            raise RuntimeError(
-                "Could not create data ID value. Automatic relationship generation "
-                "may have failed; try adding keywords to assign a specific instrument, "
-                "physical_filter, etc. based on the nested exception message."
-            ) from e
-
-
-def addDatasetType(butler: Butler, name: str, dimensions: set[str], storageClass: str) -> DatasetType:
-    """Add a new dataset type to a repository.
-
-    Parameters
-    ----------
-    butler : `lsst.daf.butler.Butler`
-        The repository to update.
-    name : `str`
-        The name of the dataset type.
-    dimensions : `set` [`str`]
-        The dimensions of the new dataset type.
-    storageClass : `str`
-        The storage class the dataset will use.
-
-    Returns
-    -------
-    datasetType : `lsst.daf.butler.DatasetType`
-        The new type.
-
-    Raises
-    ------
-    ValueError
-        Raised if the dimensions or storage class is invalid.
-
-    Notes
-    -----
-    Dataset types are shared across all collections in a repository, so this
-    function does not need to be run for each collection.
-    """
-    try:
-        datasetType = DatasetType(name, dimensions, storageClass, universe=butler.dimensions)
-        butler.registry.registerDatasetType(datasetType)
-        return datasetType
-    except KeyError as e:
-        raise ValueError from e
-
-
-class DatastoreMock:
-    """Mocks a butler datastore.
-
-    Has functions that mock the datastore in a butler. Provides an `apply`
-    function to replace the relevent butler datastore functions with the mock
-    functions.
-    """
-
-    @staticmethod
-    def apply(butler: Butler) -> None:
-        """Apply datastore mocks to a butler.
+    def union_subquery(
+        self,
+        others: Iterable[QueryBuilder],
+    ) -> QueryJoiner:
+        """Combine this builder with others to make a SELECT UNION subquery.
 
         Parameters
         ----------
-        butler : `~lsst.daf.butler.Butler`
-            Butler to be modified.
+        others : `~collections.abc.Iterable` [ `QueryBuilder` ]
+            Other query builders to union with.  Their `columns` attributes
+            must be the same as those of ``self``.
+
+        Returns
+        -------
+        joiner : `QueryJoiner`
+            `QueryJoiner` with at least all columns in `columns` available.
+            This may or may not be the `joiner` attribute of this object.
         """
-        butler._datastore.export = DatastoreMock._mock_export  # type: ignore
-        butler._datastore.get = DatastoreMock._mock_get  # type: ignore
-        butler._datastore.ingest = MagicMock()  # type: ignore
-
-    @staticmethod
-    def _mock_export(
-        refs: Iterable[DatasetRef], *, directory: str | None = None, transfer: str | None = None
-    ) -> Iterable[FileDataset]:
-        """Mock of `Datastore.export` that satisfies the requirement that
-        the refs passed in are included in the `FileDataset` objects
-        returned.
-
-        This can be used to construct a `Datastore` mock that can be used
-        in repository export via::
-
-            datastore = unittest.mock.Mock(spec=Datastore)
-            datastore.export = DatastoreMock._mock_export
-
-        """
-        for ref in refs:
-            yield FileDataset(
-                refs=[ref], path="mock/path", formatter="lsst.daf.butler.formatters.json.JsonFormatter"
-            )
-
-    @staticmethod
-    def _mock_get(
-        ref: DatasetRef,
-        parameters: Mapping[str, Any] | None = None,
-        storageClass: StorageClass | str | None = None,
-    ) -> tuple[DatasetId, Mapping[str, Any] | None]:
-        """Mock of `Datastore.get` that just returns the integer dataset ID
-        value and parameters it was given.
+        select0 = self.select()
+        other_selects = [other.select() for other in others]
+        return QueryJoiner(
+            self.joiner.db,
+            from_clause=select0.union(*other_selects).subquery(),
+            name_shrinker=self.joiner.name_shrinker,
+        ).extract_columns(self.columns, self.postprocessing)
+
+    def make_table_spec(self) -> ddl.TableSpec:
+        """Make a specification that can be used to create a table to store
+        this query's outputs.
+
+        Returns
+        -------
+        spec : `.ddl.TableSpec`
+            Table specification for this query's result columns (including
+            those from `postprocessing` and `QueryJoiner.special`).
         """
-        return (ref.id, parameters)
+        assert not self.joiner.special, "special columns not supported in make_table_spec"
+        if self.joiner.name_shrinker is None:
+            self.joiner.name_shrinker = self.joiner._make_name_shrinker()
+        results = ddl.TableSpec(
+            [
+                self.columns.get_column_spec(logical_table, field).to_sql_spec(
+                    name_shrinker=self.joiner.name_shrinker
+                )
+                for logical_table, field in self.columns
+            ]
+        )
+        if self.postprocessing:
+            for element in self.postprocessing.iter_missing(self.columns):
+                results.fields.add(
+                    ddl.FieldSpec.for_region(
+                        self.joiner.name_shrinker.shrink(
+                            self.columns.get_qualified_name(element.name, "region")
+                        )
+                    )
+                )
+        return results
+
+
+@dataclasses.dataclass
+class QueryJoiner:
+    """A struct used to represent the FROM and WHERE clauses of an
+    under-construction SQL SELECT query.
+
+    This object's methods frequently "consume" ``self``, by either returning
+    it after modification or returning related copy that may share state with
+    the original.  Users should be careful never to use consumed instances, and
+    are recommended to reuse the same variable name to make that hard to do
+    accidentally.
+    """
+
+    db: Database
+    """Object that abstracts over the database engine."""
+
+    from_clause: sqlalchemy.FromClause | None = None
+    """SQLAlchemy representation of the FROM clause.
+
+    This is initialized to `None` but in almost all cases is immediately
+    replaced.
+    """
+
+    where_terms: list[sqlalchemy.ColumnElement[bool]] = dataclasses.field(default_factory=list)
+    """Sequence of WHERE clause terms to be combined with AND."""
+
+    dimension_keys: NonemptyMapping[str, list[sqlalchemy.ColumnElement]] = dataclasses.field(
+        default_factory=lambda: NonemptyMapping(list)
+    )
+    """Mapping of dimension keys included in the FROM clause.
+
+    Nested lists correspond to different tables that have the same dimension
+    key (which should all have equal values for all result rows).
+    """
+
+    fields: NonemptyMapping[str, dict[str, sqlalchemy.ColumnElement[Any]]] = dataclasses.field(
+        default_factory=lambda: NonemptyMapping(dict)
+    )
+    """Mapping of columns that are neither dimension keys nor timespans.
+
+    Inner and outer keys correspond to the "logical table" and "field" pairs
+    that result from iterating over `~.queries.tree.ColumnSet`, with the former
+    either a dimension element name or dataset type name.
+    """
+
+    timespans: dict[str, TimespanDatabaseRepresentation] = dataclasses.field(default_factory=dict)
+    """Mapping of timespan columns.
+
+    Keys are "logical tables" - dimension element names or dataset type names.
+    """
+
+    special: dict[str, sqlalchemy.ColumnElement[Any]] = dataclasses.field(default_factory=dict)
+    """Special columns that are available from the FROM clause and
+    automatically included in the SELECT clause when this joiner is nested
+    within a `QueryBuilder`.
+
+    These columns are not part of the dimension universe and are not associated
+    with a dataset.  They are never returned to users, even if they may be
+    included in raw SQL results.
+    """
+
+    name_shrinker: NameShrinker | None = None
+    """An object that can be used to shrink field names to fit within the
+    identifier limit of the database engine.
+
+    This is important for PostgreSQL (which has a 64-character limit) and
+    dataset fields, since dataset type names are used to qualify those and they
+    can be quite long.  `DimensionUniverse` guarantees at construction that
+    dimension names and fully-qualified dimension fields do not exceed this
+    limit.
+    """
+
+    def extract_dimensions(self, dimensions: Iterable[str], **kwargs: str) -> QueryJoiner:
+        """Add dimension key columns from `from_clause` into `dimension_keys`.
+
+        Parameters
+        ----------
+        dimensions : `~collections.abc.Iterable` [ `str` ]
+            Names of dimensions to include, assuming that their names in
+            `sql_columns` are just the dimension names.
+        **kwargs : `str`
+            Additional dimensions to include, with the names in `sql_columns`
+            as keys and the actual dimension names as values.
+
+        Returns
+        -------
+        self : `QueryJoiner`
+            This `QueryJoiner` instance (never a copy). Provided to enable
+            method chaining.
+        """
+        assert self.from_clause is not None, "Cannot extract columns with no FROM clause."
+        for dimension_name in dimensions:
+            self.dimension_keys[dimension_name].append(self.from_clause.columns[dimension_name])
+        for k, v in kwargs.items():
+            self.dimension_keys[v].append(self.from_clause.columns[k])
+        return self
+
+    def extract_columns(
+        self,
+        columns: qt.ColumnSet,
+        postprocessing: Postprocessing | None = None,
+        special: Iterable[str] = (),
+    ) -> QueryJoiner:
+        """Add columns from `from_clause` into `dimension_keys`.
+
+        Parameters
+        ----------
+        columns : `.queries.tree.ColumnSet`
+            Columns to include, assuming that
+            `.queries.tree.ColumnSet.get_qualified_name` corresponds to the
+            name used in `sql_columns` (after name shrinking).
+        postprocessing : `Postprocessing`, optional
+            Postprocessing object whose needed columns should also be included.
+        special : `~collections.abc.Iterable` [ `str` ], optional
+            Additional special columns to extract.
+
+        Returns
+        -------
+        self : `QueryJoiner`
+            This `QueryJoiner` instance (never a copy). Provided to enable
+            method chaining.
+        """
+        assert self.from_clause is not None, "Cannot extract columns with no FROM clause."
+        if self.name_shrinker is None:
+            self.name_shrinker = self._make_name_shrinker()
+        for logical_table, field in columns:
+            name = columns.get_qualified_name(logical_table, field)
+            if field is None:
+                self.dimension_keys[logical_table].append(self.from_clause.columns[name])
+            else:
+                name = self.name_shrinker.shrink(name)
+                if columns.is_timespan(logical_table, field):
+                    self.timespans[logical_table] = self.db.getTimespanRepresentation().from_columns(
+                        self.from_clause.columns, name
+                    )
+                else:
+                    self.fields[logical_table][field] = self.from_clause.columns[name]
+        if postprocessing is not None:
+            for element in postprocessing.iter_missing(columns):
+                self.fields[element.name]["region"] = self.from_clause.columns[
+                    self.name_shrinker.shrink(columns.get_qualified_name(element.name, "region"))
+                ]
+            if postprocessing.check_validity_match_count:
+                self.special[postprocessing.VALIDITY_MATCH_COUNT] = self.from_clause.columns[
+                    postprocessing.VALIDITY_MATCH_COUNT
+                ]
+        for name in special:
+            self.special[name] = self.from_clause.columns[name]
+        return self
+
+    def join(self, other: QueryJoiner) -> QueryJoiner:
+        """Combine this `QueryJoiner` with another via an INNER JOIN on
+        dimension keys.
+
+        This method consumes ``self``.
+
+        Parameters
+        ----------
+        other : `QueryJoiner`
+            Other joiner to combine with this one.
+
+        Returns
+        -------
+        joined : `QueryJoiner`
+            A `QueryJoiner` with all columns present in either operand, with
+            its `from_clause` representing a SQL INNER JOIN where the dimension
+            key columns common to both operands are constrained to be equal.
+            If either operand does not have `from_clause`, the other's is used.
+            The `where_terms` of the two operands are concatenated,
+            representing a logical AND (with no attempt at deduplication).
+        """
+        join_on: list[sqlalchemy.ColumnElement] = []
+        for dimension_name in other.dimension_keys.keys():
+            if dimension_name in self.dimension_keys:
+                for column1, column2 in itertools.product(
+                    self.dimension_keys[dimension_name], other.dimension_keys[dimension_name]
+                ):
+                    join_on.append(column1 == column2)
+            self.dimension_keys[dimension_name].extend(other.dimension_keys[dimension_name])
+        if self.from_clause is None:
+            self.from_clause = other.from_clause
+        elif other.from_clause is not None:
+            join_on_sql: sqlalchemy.ColumnElement[bool]
+            match len(join_on):
+                case 0:
+                    join_on_sql = sqlalchemy.true()
+                case 1:
+                    (join_on_sql,) = join_on
+                case _:
+                    join_on_sql = sqlalchemy.and_(*join_on)
+            self.from_clause = self.from_clause.join(other.from_clause, onclause=join_on_sql)
+        for logical_table, fields in other.fields.items():
+            self.fields[logical_table].update(fields)
+        self.timespans.update(other.timespans)
+        self.special.update(other.special)
+        self.where_terms += other.where_terms
+        if other.name_shrinker:
+            if self.name_shrinker is not None:
+                self.name_shrinker.update(other.name_shrinker)
+            else:
+                self.name_shrinker = other.name_shrinker
+        return self
+
+    def where(self, *args: sqlalchemy.ColumnElement[bool]) -> QueryJoiner:
+        """Add a WHERE clause term.
+
+        Parameters
+        ----------
+        *args : `sqlalchemy.ColumnElement`
+            SQL boolean column expressions to be combined with AND.
+
+        Returns
+        -------
+        self : `QueryJoiner`
+            This `QueryJoiner` instance (never a copy). Provided to enable
+            method chaining.
+        """
+        self.where_terms.extend(args)
+        return self
+
+    def to_builder(
+        self,
+        columns: qt.ColumnSet,
+        postprocessing: Postprocessing | None = None,
+        distinct: bool | Sequence[sqlalchemy.ColumnElement[Any]] = (),
+        group_by: Sequence[sqlalchemy.ColumnElement[Any]] = (),
+    ) -> QueryBuilder:
+        """Convert this joiner into a `QueryBuilder` by providing SELECT clause
+        columns and optional DISTINCT or GROUP BY clauses.
+
+        This method consumes ``self``.
+
+        Parameters
+        ----------
+        columns : `~.queries.tree.ColumnSet`
+            Regular columns to include in the SELECT clause.
+        postprocessing : `Postprocessing`, optional
+            Addition processing to be performed on result rows after executing
+            the SQL query.
+        distinct : `bool` or `~collections.abc.Sequence` [ \
+                `sqlalchemy.ColumnElement` ], optional
+            Specification of the DISTINCT clause (see `QueryBuilder.distinct`).
+        group_by : `~collections.abc.Sequence` [ \
+                `sqlalchemy.ColumnElement` ], optional
+            Specification of the GROUP BY clause (see `QueryBuilder.group_by`).
+
+        Returns
+        -------
+        builder : `QueryBuilder`
+            New query builder.
+        """
+        return QueryBuilder(
+            self,
+            columns,
+            postprocessing=postprocessing if postprocessing is not None else Postprocessing(),
+            distinct=distinct,
+            group_by=group_by,
+        )
+
+    def _make_name_shrinker(self) -> NameShrinker:
+        return NameShrinker(self.db.dialect.max_identifier_length, 6)
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliCmdTestBase.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/cliCmdTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/cliLogTestBase.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/cliLogTestBase.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/deferredFormatter.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/deferredFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/dict_convertible_model.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/dict_convertible_model.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/hybrid_butler.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,27 +30,35 @@
 from collections.abc import Collection, Iterable, Mapping, Sequence
 from contextlib import AbstractContextManager
 from typing import Any, TextIO, cast
 
 from lsst.resources import ResourcePath, ResourcePathExpression
 
 from .._butler import Butler
+from .._butler_collections import ButlerCollections
 from .._dataset_existence import DatasetExistence
 from .._dataset_ref import DatasetId, DatasetRef
 from .._dataset_type import DatasetType
 from .._deferredDatasetHandle import DeferredDatasetHandle
 from .._file_dataset import FileDataset
 from .._limited_butler import LimitedButler
-from .._query import Query
 from .._storage_class import StorageClass
 from .._timespan import Timespan
 from ..datastore import DatasetRefURIs
-from ..dimensions import DataCoordinate, DataId, DimensionGroup, DimensionRecord, DimensionUniverse
+from ..dimensions import (
+    DataCoordinate,
+    DataId,
+    DimensionElement,
+    DimensionGroup,
+    DimensionRecord,
+    DimensionUniverse,
+)
 from ..direct_butler import DirectButler
-from ..registry import CollectionArgType, Registry
+from ..queries import Query
+from ..registry import Registry
 from ..remote_butler import RemoteButler
 from ..transfers import RepoExportContext
 from .hybrid_butler_registry import HybridButlerRegistry
 
 
 class HybridButler(Butler):
     """A `Butler` that delegates methods to internal RemoteButler and
@@ -352,15 +360,15 @@
             explain=explain,
             **kwargs,
         )
 
     def _query_datasets(
         self,
         dataset_type: Any,
-        collections: CollectionArgType | None = None,
+        collections: str | Iterable[str] | None = None,
         *,
         find_first: bool = True,
         data_id: DataId | None = None,
         where: str = "",
         bind: Mapping[str, Any] | None = None,
         expanded: bool = False,
         explain: bool = True,
@@ -431,7 +439,21 @@
         return self._direct_butler.pruneDatasets(
             refs, disassociate=disassociate, unstore=unstore, tags=tags, purge=purge
         )
 
     @property
     def dimensions(self) -> DimensionUniverse:
         return self._remote_butler.dimensions
+
+    def _extract_all_dimension_records_from_data_ids(
+        self,
+        source_butler: LimitedButler | Butler,
+        data_ids: set[DataCoordinate],
+        allowed_elements: frozenset[DimensionElement],
+    ) -> dict[DimensionElement, dict[DataCoordinate, DimensionRecord]]:
+        return self._direct_butler._extract_all_dimension_records_from_data_ids(
+            source_butler, data_ids, allowed_elements
+        )
+
+    @property
+    def collection_chains(self) -> ButlerCollections:
+        return self._direct_butler.collection_chains
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/hybrid_butler_registry.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/hybrid_butler_registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,39 +101,39 @@
 
     def registerCollection(
         self, name: str, type: CollectionType = CollectionType.TAGGED, doc: str | None = None
     ) -> bool:
         return self._direct.registerCollection(name, type, doc)
 
     def getCollectionType(self, name: str) -> CollectionType:
-        return self._direct.getCollectionType(name)
+        return self._remote.getCollectionType(name)
 
     def registerRun(self, name: str, doc: str | None = None) -> bool:
         return self._direct.registerRun(name, doc)
 
     def removeCollection(self, name: str) -> None:
         return self._direct.removeCollection(name)
 
     def getCollectionChain(self, parent: str) -> Sequence[str]:
-        return self._direct.getCollectionChain(parent)
+        return self._remote.getCollectionChain(parent)
 
     def setCollectionChain(self, parent: str, children: Any, *, flatten: bool = False) -> None:
         return self._direct.setCollectionChain(parent, children, flatten=flatten)
 
     def getCollectionParentChains(self, collection: str) -> set[str]:
-        return self._direct.getCollectionParentChains(collection)
+        return self._remote.getCollectionParentChains(collection)
 
     def getCollectionDocumentation(self, collection: str) -> str | None:
-        return self._direct.getCollectionDocumentation(collection)
+        return self._remote.getCollectionDocumentation(collection)
 
     def setCollectionDocumentation(self, collection: str, doc: str | None) -> None:
         return self._direct.setCollectionDocumentation(collection, doc)
 
     def getCollectionSummary(self, collection: str) -> CollectionSummary:
-        return self._direct.getCollectionSummary(collection)
+        return self._remote.getCollectionSummary(collection)
 
     def registerDatasetType(self, datasetType: DatasetType) -> bool:
         return self._direct.registerDatasetType(datasetType)
 
     def removeDatasetType(self, name: str | tuple[str, ...]) -> None:
         return self._direct.removeDatasetType(name)
 
@@ -255,15 +255,15 @@
         self,
         expression: Any = ...,
         datasetType: DatasetType | None = None,
         collectionTypes: Iterable[CollectionType] | CollectionType = CollectionType.all(),
         flattenChains: bool = False,
         includeChains: bool | None = None,
     ) -> Sequence[str]:
-        return self._direct.queryCollections(
+        return self._remote.queryCollections(
             expression, datasetType, collectionTypes, flattenChains, includeChains
         )
 
     def queryDatasets(
         self,
         datasetType: Any,
         *,
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/server.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from collections.abc import Iterator
 from contextlib import contextmanager
 from dataclasses import dataclass
 from tempfile import TemporaryDirectory
 
+from fastapi import FastAPI, Request
 from fastapi.testclient import TestClient
 from lsst.daf.butler import Butler, Config, LabeledButlerFactory
 from lsst.daf.butler.remote_butler import RemoteButler, RemoteButlerFactory
 from lsst.daf.butler.remote_butler.server import create_app
 from lsst.daf.butler.remote_butler.server._dependencies import butler_factory_dependency
 from lsst.resources.s3utils import clean_test_environment_for_s3, getS3Client
 
@@ -86,14 +87,15 @@
 
             with TemporaryDirectory() as root:
                 Butler.makeRepo(root, config=Config(base_config_path), forceConfigRoot=False)
                 config_file_path = os.path.join(root, "butler.yaml")
 
                 app = create_app()
                 add_auth_header_check_middleware(app)
+                _add_root_exception_handler(app)
                 # Override the server's Butler initialization to point at our
                 # test repo
                 server_butler_factory = LabeledButlerFactory({TEST_REPOSITORY_NAME: config_file_path})
                 app.dependency_overrides[butler_factory_dependency] = lambda: server_butler_factory
 
                 client = TestClient(app)
                 client_without_error_propagation = TestClient(app, raise_server_exceptions=False)
@@ -118,7 +120,29 @@
 
 
 def _make_remote_butler(client: TestClient) -> RemoteButler:
     remote_butler_factory = RemoteButlerFactory(
         f"https://test.example/api/butler/repo/{TEST_REPOSITORY_NAME}", client
     )
     return remote_butler_factory.create_butler_for_access_token("fake-access-token")
+
+
+class UnhandledServerError(Exception):
+    """Raised for unhandled exceptions within the server that would result in a
+    500 Internal Server Error in a real deployment.  This allows us to tell the
+    difference between exceptions being propagated intentionally, and those
+    just bubbling up implicitly from the server to the client.
+
+    The FastAPI TestClient by default passes unhandled exceptions up from the
+    server to the client.  This is useful behavior for unit testing because it
+    gives you traceability from the test to the problem in the server code.
+    However, because RemoteButler is in some ways just a proxy for the
+    server-side Butler, we raise similar exceptions on the client and server
+    side. Thus the default TestClient behavior can mask missing error-handling
+    logic.
+    """
+
+
+def _add_root_exception_handler(app: FastAPI) -> None:
+    @app.exception_handler(Exception)
+    async def convert_exception_types(request: Request, exc: Exception) -> None:
+        raise UnhandledServerError("Unhandled server exception") from exc
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/server_utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/_exceptions_legacy.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,54 +21,41 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
+__all__ = ("DataIdError", "DatasetTypeError", "RegistryError")
 
-import re
-from typing import Any
+# The classes in this file exist only for backwards compatibility.  New
+# exception types should not inherit from these.
 
-from fastapi import FastAPI, HTTPException, Request, Response
 
+class RegistryError(Exception):
+    """Base class for many exception classes produced by Registry methods.
 
-def add_auth_header_check_middleware(app: FastAPI) -> None:
-    """Add a middleware to a FastAPI app to check that Gafaelfawr
-    authentication headers are present.
+    Notes
+    -----
+    The client code that needs to handle exceptions generated by the Registry
+    methods can catch this class or one of its many subclasses as described by
+    the particular method documentation. While most of the Registry methods
+    should only raise the exceptions of this type, it is hard to guarantee
+    that they will never raise other exception types. If the client needs to
+    handle all possible exceptions, then it should also catch a standard
+    `Exception` type as well. Additionally, some Registry methods can be
+    explicitly documented to raise exceptions outside this class hierarchy.
+    """
 
-    This is only suitable for testing -- in a real deployment,
-    GafaelfawrIngress will handle these headers and convert them to a different
-    format.
 
-    Parameters
-    ----------
-    app : `FastAPI`
-        The app the middleware will be added to.
+class DataIdError(RegistryError):
+    """Exception raised for incorrect data IDs, this is a base class for other
+    specific error types.
     """
 
-    @app.middleware("http")
-    async def check_auth_headers(request: Request, call_next: Any) -> Response:
-        if _is_authenticated_endpoint(request.url.path):
-            header = request.headers.get("authorization")
-            if header is None:
-                raise HTTPException(status_code=401, detail="Authorization header is missing")
-            if not re.match(r"^Bearer \S+", header):
-                raise HTTPException(
-                    status_code=401, detail=f"Authorization header not in expected format: {header}"
-                )
-
-        return await call_next(request)
-
-
-def _is_authenticated_endpoint(path: str) -> bool:
-    """Return True if the specified path requires authentication in the real
-    server deployment.
-    """
-    if path == "/":
-        return False
-    if path.endswith("/butler.yaml"):
-        return False
-    if path.endswith("/butler.json"):
-        return False
 
-    return True
+class DatasetTypeError(RegistryError):
+    """Exception raised for problems with dataset types."""
+
+
+class CollectionError(RegistryError):
+    """Exception raised for collection-related errors."""
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/testFormatters.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/testFormatters.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/tests/utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/tests/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -289,36 +289,39 @@
         )
 
         # Add needed Dimensions
         self.butler.registry.insertDimensionData("instrument", {"name": "DummyCamComp"})
         self.butler.registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCamComp", "name": "d-r", "band": "R"}
         )
+        self.butler.registry.insertDimensionData("day_obs", {"instrument": "DummyCamComp", "id": 20200101})
         self.butler.registry.insertDimensionData(
             "visit_system", {"instrument": "DummyCamComp", "id": 1, "name": "default"}
         )
         visitStart = astropy.time.Time("2020-01-01 08:00:00.123456789", scale="tai")
         visitEnd = astropy.time.Time("2020-01-01 08:00:36.66", scale="tai")
         self.butler.registry.insertDimensionData(
             "visit",
             dict(
                 instrument="DummyCamComp",
                 id=423,
                 name="fourtwentythree",
                 physical_filter="d-r",
                 timespan=Timespan(visitStart, visitEnd),
+                day_obs=20200101,
             ),
         )
         self.butler.registry.insertDimensionData(
             "visit",
             dict(
                 instrument="DummyCamComp",
                 id=424,
                 name="fourtwentyfour",
                 physical_filter="d-r",
+                day_obs=20200101,
             ),
         )
 
         self.addDataset({"instrument": "DummyCamComp", "visit": 423})
         self.addDataset({"instrument": "DummyCamComp", "visit": 424})
 
     def addDataset(
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/time_utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/timespan_database_representation.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/timespan_database_representation.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,21 +24,18 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 from __future__ import annotations
 
 __all__ = ("TimespanDatabaseRepresentation",)
 
-import enum
 from abc import ABC, abstractmethod
 from collections.abc import Callable, Mapping
-from typing import TYPE_CHECKING, Any, ClassVar, TypeVar, Union
+from typing import TYPE_CHECKING, Any, ClassVar, TypeVar
 
-import astropy.time
-import astropy.utils.exceptions
 import sqlalchemy
 
 # As of astropy 4.2, the erfa interface is shipped independently and
 # ErfaWarning is no longer an AstropyWarning
 try:
     import erfa
 except ImportError:
@@ -49,30 +46,14 @@
 from ._timespan import Timespan
 from .time_utils import TimeConverter
 
 if TYPE_CHECKING:  # Imports needed only for type annotations; may be circular.
     pass
 
 
-class _SpecialTimespanBound(enum.Enum):
-    """Enumeration to provide a singleton value for empty timespan bounds.
-
-    This enum's only member should generally be accessed via the
-    `Timespan.EMPTY` alias.
-    """
-
-    EMPTY = enum.auto()
-    """The value used for both `Timespan.begin` and `Timespan.end` for empty
-    Timespans that contain no points.
-    """
-
-
-TimespanBound = Union[astropy.time.Time, _SpecialTimespanBound, None]
-
-
 _S = TypeVar("_S", bound="TimespanDatabaseRepresentation")
 
 
 class TimespanDatabaseRepresentation(ABC):
     """An interface for representing a timespan in a database.
 
     Notes
@@ -543,16 +524,16 @@
             name = cls.NAME
         if result is None:
             result = {}
         if extent is None:
             begin_nsec = None
             end_nsec = None
         else:
-            begin_nsec = extent._nsec[0]
-            end_nsec = extent._nsec[1]
+            begin_nsec = extent.nsec[0]
+            end_nsec = extent.nsec[1]
         result[f"{name}_begin"] = begin_nsec
         result[f"{name}_end"] = end_nsec
         return result
 
     @classmethod
     def extract(cls, mapping: Mapping[str, Any], name: str | None = None) -> Timespan | None:
         # Docstring inherited.
@@ -585,15 +566,15 @@
 
     @classmethod
     def fromLiteral(cls, timespan: Timespan | None) -> _CompoundTimespanDatabaseRepresentation:
         # Docstring inherited.
         if timespan is None:
             return cls(nsec=(sqlalchemy.sql.null(), sqlalchemy.sql.null()), name=cls.NAME)
         return cls(
-            nsec=(sqlalchemy.sql.literal(timespan._nsec[0]), sqlalchemy.sql.literal(timespan._nsec[1])),
+            nsec=(sqlalchemy.sql.literal(timespan.nsec[0]), sqlalchemy.sql.literal(timespan.nsec[1])),
             name=cls.NAME,
         )
 
     @property
     def name(self) -> str:
         # Docstring inherited.
         return self._name
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/__init__.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/__init__.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_context.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         collection will cause its associations with exported datasets to also
         be exported, but it does not export those datasets automatically.
 
         Exporting a `~CollectionType.CHAINED` collection does not automatically
         export its child collections; these must be explicitly exported or
         already be present in the repository they are being imported into.
         """
-        self._collections[name] = self._registry._get_collection_record(name)
+        self._collections[name] = self._registry.get_collection_record(name)
 
     def saveDimensionData(
         self, element: str | DimensionElement, records: Iterable[dict | DimensionRecord]
     ) -> None:
         """Export the given dimension records associated with one or more data
         IDs.
 
@@ -269,15 +269,15 @@
         """
         for element in self._registry.dimensions.sorted(self._records.keys()):
             # To make export deterministic sort the DataCoordinate instances.
             r = self._records[element]
             self._backend.saveDimensionData(element, *[r[dataId] for dataId in sorted(r.keys())])
         for datasetsByRun in self._datasets.values():
             for run in datasetsByRun:
-                self._collections[run] = self._registry._get_collection_record(run)
+                self._collections[run] = self._registry.get_collection_record(run)
         for collectionName in self._computeSortedCollections():
             doc = self._registry.getCollectionDocumentation(collectionName)
             self._backend.saveCollection(self._collections[collectionName], doc)
         # Sort the dataset types and runs before exporting to ensure
         # reproducible order in export file.
         for datasetType in sorted(self._datasets.keys()):
             for run in sorted(self._datasets[datasetType].keys()):
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_interfaces.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/_interfaces.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/transfers/_yaml.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/transfers/_yaml.py`

 * *Files 20% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 from __future__ import annotations
 
 __all__ = ["YamlRepoExportBackend", "YamlRepoImportBackend"]
 
+import logging
 import uuid
 import warnings
 from collections import UserDict, defaultdict
 from collections.abc import Iterable, Mapping
 from datetime import datetime
 from typing import IO, TYPE_CHECKING, Any
 
@@ -56,14 +57,16 @@
 from ..registry.sql_registry import SqlRegistry
 from ..registry.versions import IncompatibleVersionError
 from ._interfaces import RepoExportBackend, RepoImportBackend
 
 if TYPE_CHECKING:
     from lsst.resources import ResourcePathExpression
 
+_LOG = logging.getLogger(__name__)
+
 EXPORT_FORMAT_VERSION = VersionTuple(1, 0, 2)
 """Export format version.
 
 Files with a different major version or a newer minor version cannot be read by
 this version of the code.
 """
 
@@ -220,14 +223,80 @@
                 "data": self.data,
             },
             stream=self.stream,
             sort_keys=False,
         )
 
 
+class _DayObsOffsetCalculator:
+    """Interface to allow the day_obs offset to be calculated from an
+    instrument class name and cached.
+    """
+
+    name_to_class_name: dict[str, str]
+    name_to_offset: dict[str, int | None]
+
+    def __init__(self) -> None:
+        self.name_to_class_name = {}
+        self.name_to_offset = {}
+
+    def __setitem__(self, name: str, class_name: str) -> None:
+        """Store the instrument class name.
+
+        Parameters
+        ----------
+        name : `str`
+            Name of the instrument.
+        class_name : `str`
+            Full name of the instrument class.
+        """
+        self.name_to_class_name[name] = class_name
+
+    def get_offset(self, name: str, date: astropy.time.Time) -> int | None:
+        """Return the offset to use when calculating day_obs.
+
+        Parameters
+        ----------
+        name : `str`
+            The instrument name.
+        date : `astropy.time.Time`
+            Time for which the offset is required.
+
+        Returns
+        -------
+        offset : `int`
+            The offset in seconds.
+        """
+        if name in self.name_to_offset:
+            return self.name_to_offset[name]
+
+        try:
+            instrument_class = doImportType(self.name_to_class_name[name])
+        except Exception:
+            # Any error at all, store None and do not try again.
+            self.name_to_offset[name] = None
+            return None
+
+        # Assume this is a `lsst.pipe.base.Instrument` and that it has
+        # a translatorClass property pointing to an
+        # astro_metadata_translator.MetadataTranslator class. If this is not
+        # true give up and store None.
+        try:
+            offset_delta = instrument_class.translatorClass.observing_date_to_offset(date)  # type: ignore
+        except Exception:
+            offset_delta = None
+
+        if offset_delta is None:
+            self.name_to_offset[name] = None
+            return None
+
+        self.name_to_offset[name] = round(offset_delta.to_value("s"))
+        return self.name_to_offset[name]
+
+
 class YamlRepoImportBackend(RepoImportBackend):
     """A repository import implementation that reads from a YAML file.
 
     Parameters
     ----------
     stream : `io.IO`
         A readable file-like object.
@@ -292,28 +361,84 @@
             universe_version < 1
             and universe_namespace == "daf_butler"
             and "visit" in self.registry.dimensions
             and "seeing" not in self.registry.dimensions["visit"].metadata
         ):
             migrate_visit_seeing = True
 
+        # If this data exported before group was a first-class dimension,
+        # we'll need to modify some exposure columns and add group records.
+        migrate_group = False
+        if (
+            universe_version < 6
+            and universe_namespace == "daf_butler"
+            and "exposure" in self.registry.dimensions
+            and "group" in self.registry.dimensions["exposure"].implied
+        ):
+            migrate_group = True
+
+        # If this data exported before day_obs was a first-class dimension,
+        # we'll need to modify some exposure and visit columns and add day_obs
+        # records.  This is especially tricky because some files even predate
+        # the existence of data ID values.
+        migrate_exposure_day_obs = False
+        migrate_visit_day_obs = False
+        day_obs_ids: set[tuple[str, int]] = set()
+        if universe_version < 6 and universe_namespace == "daf_butler":
+            if (
+                "exposure" in self.registry.dimensions
+                and "day_obs" in self.registry.dimensions["exposure"].implied
+            ):
+                migrate_exposure_day_obs = True
+            if "visit" in self.registry.dimensions and "day_obs" in self.registry.dimensions["visit"].implied:
+                migrate_visit_day_obs = True
+
+        # If this is pre-v1 universe we may need to fill in a missing
+        # visit.day_obs field.
+        migrate_add_visit_day_obs = False
+        if (
+            universe_version < 1
+            and universe_namespace == "daf_butler"
+            and (
+                "day_obs" in self.registry.dimensions["visit"].implied
+                or "day_obs" in self.registry.dimensions["visit"].metadata
+            )
+        ):
+            migrate_add_visit_day_obs = True
+
+        # Some conversions may need to work out a day_obs timespan.
+        # The only way this offset can be found is by querying the instrument
+        # class. Read all the existing instrument classes indexed by name.
+        instrument_classes: dict[str, int] = {}
+        if migrate_exposure_day_obs or migrate_visit_day_obs or migrate_add_visit_day_obs:
+            day_obs_offset_calculator = _DayObsOffsetCalculator()
+            for rec in self.registry.queryDimensionRecords("instrument"):
+                day_obs_offset_calculator[rec.name] = rec.class_name
+
         datasetData = []
         RecordClass: type[DimensionRecord]
         for data in wrapper["data"]:
             if data["type"] == "dimension":
                 # convert all datetime values to astropy
                 for record in data["records"]:
                     for key in record:
                         # Some older YAML files were produced with native
                         # YAML support for datetime, we support reading that
                         # data back. Newer conversion uses _AstropyTimeToYAML
                         # class with special YAML tag.
                         if isinstance(record[key], datetime):
                             record[key] = astropy.time.Time(record[key], scale="utc")
 
+                if data["element"] == "instrument":
+                    if migrate_exposure_day_obs or migrate_visit_day_obs:
+                        # Might want the instrument class name for later.
+                        for record in data["records"]:
+                            if record["name"] not in instrument_classes:
+                                instrument_classes[record["name"]] = record["class_name"]
+
                 if data["element"] == "visit":
                     if migrate_visit_system:
                         # Must create the visit_system_membership records.
                         # But first create empty list for visits since other
                         # logic in this file depends on self.dimensions being
                         # populated in an order consisteny with primary keys.
                         self.dimensions[self.registry.dimensions["visit"]] = []
@@ -324,14 +449,52 @@
                                 instrument=r["instrument"], visit_system=r.pop("visit_system"), visit=r["id"]
                             )
                             for r in data["records"]
                         )
                     if migrate_visit_seeing:
                         for record in data["records"]:
                             record.pop("seeing", None)
+                    if migrate_add_visit_day_obs:
+                        # The day_obs field is missing. It can be derived from
+                        # the datetime_begin field.
+                        for record in data["records"]:
+                            date = record["datetime_begin"].tai
+                            offset = day_obs_offset_calculator.get_offset(record["instrument"], date)
+                            # This field is required so we have to calculate
+                            # it even if the offset is not defined.
+                            if offset:
+                                date = date - astropy.time.TimeDelta(offset, format="sec", scale="tai")
+                            record["day_obs"] = int(date.strftime("%Y%m%d"))
+                    if migrate_visit_day_obs:
+                        # Poke the entry for this dimension to make sure it
+                        # appears in the right order, even though we'll
+                        # populate it later.
+                        self.dimensions[self.registry.dimensions["day_obs"]]
+                        for record in data["records"]:
+                            day_obs_ids.add((record["instrument"], record["day_obs"]))
+
+                if data["element"] == "exposure":
+                    if migrate_group:
+                        element = self.registry.dimensions["group"]
+                        RecordClass = element.RecordClass
+                        group_records = self.dimensions[element]
+                        for exposure_record in data["records"]:
+                            exposure_record["group"] = exposure_record.pop("group_name")
+                            del exposure_record["group_id"]
+                            group_records.append(
+                                RecordClass(
+                                    instrument=exposure_record["instrument"], name=exposure_record["group"]
+                                )
+                            )
+                    if migrate_exposure_day_obs:
+                        # Poke the entry for this dimension to make sure it
+                        # appears in the right order, even though we'll
+                        # populate it later.
+                        for record in data["records"]:
+                            day_obs_ids.add((record["instrument"], record["day_obs"]))
 
                 element = self.registry.dimensions[data["element"]]
                 RecordClass = element.RecordClass
                 self.dimensions[element].extend(RecordClass(**r) for r in data["records"])
 
             elif data["type"] == "collection":
                 collectionType = CollectionType.from_name(data["collection_type"])
@@ -398,14 +561,49 @@
                             assocsByTimespan[Timespan(begin=d["begin"], end=d["end"])] = [
                                 x if not isinstance(x, int) else _refIntId2UUID[x] for x in d["dataset_ids"]
                             ]
                 else:
                     raise ValueError(f"Unexpected calibration type for association: {collectionType.name}.")
             else:
                 raise ValueError(f"Unexpected dictionary type: {data['type']}.")
+
+        if day_obs_ids:
+            element = self.registry.dimensions["day_obs"]
+            RecordClass = element.RecordClass
+            missing_offsets = set()
+            for instrument, day_obs in day_obs_ids:
+                # To get the offset we need the astropy time. Since we are
+                # going from a day_obs to a time, it's possible that in some
+                # scenario the offset will be wrong.
+                ymd = str(day_obs)
+                t = astropy.time.Time(
+                    f"{ymd[0:4]}-{ymd[4:6]}-{ymd[6:8]}T00:00:00", format="isot", scale="tai"
+                )
+                offset = day_obs_offset_calculator.get_offset(instrument, t)
+
+                # This should always return an offset but as a fallback
+                # allow None here in case something has gone wrong above.
+                # In particular, not being able to load an instrument class.
+                if offset is not None:
+                    timespan = Timespan.from_day_obs(day_obs, offset=offset)
+                else:
+                    timespan = None
+                    missing_offsets.add(instrument)
+                self.dimensions[element].append(
+                    RecordClass(instrument=instrument, id=day_obs, timespan=timespan)
+                )
+
+            if missing_offsets:
+                plural = "" if len(missing_offsets) == 1 else "s"
+                warnings.warn(
+                    "Constructing day_obs records with no timespans for "
+                    "visit/exposure records that were exported before day_obs was a dimension. "
+                    f"(instrument{plural}: {missing_offsets})"
+                )
+
         # key is (dataset type name, run)
         self.datasets: Mapping[tuple[str, str], list[FileDataset]] = defaultdict(list)
         for data in datasetData:
             datasetType = self.datasetTypes.get(data["dataset_type"])
             if datasetType is None:
                 datasetType = self.registry.getDatasetType(data["dataset_type"])
             self.datasets[data["dataset_type"], data["run"]].extend(
@@ -449,15 +647,17 @@
         datastore: Datastore | None,
         *,
         directory: ResourcePathExpression | None = None,
         transfer: str | None = None,
         skip_dimensions: set | None = None,
     ) -> None:
         # Docstring inherited from RepoImportBackend.load.
-        for element, dimensionRecords in self.dimensions.items():
+        # Must ensure we insert in order supported by the universe.
+        for element in self.registry.dimensions.sorted(self.dimensions.keys()):
+            dimensionRecords = self.dimensions[element]
             if skip_dimensions and element in skip_dimensions:
                 continue
             # Using skip_existing=True here assumes that the records in the
             # database are either equivalent or at least preferable to the ones
             # being imported.  It'd be ideal to check that, but that would mean
             # using syncDimensionData, which is not vectorized and is hence
             # unacceptably slo.
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst/daf/butler/utils.py` & `lsst_daf_butler-27.0.0rc1/python/lsst/daf/butler/utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/PKG-INFO` & `lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lsst-daf-butler
-Version: 26.2024.900
+Version: 27.0.0rc1
 Summary: An abstraction layer for reading and writing astronomical data to datastores.
 Author-email: Rubin Observatory Data Management <dm-admin@lists.lsst.org>
 License: BSD 3-Clause License
 Project-URL: Homepage, https://github.com/lsst/daf_butler
 Keywords: lsst
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `lsst-daf-butler-26.2024.900/python/lsst_daf_butler.egg-info/SOURCES.txt` & `lsst_daf_butler-27.0.0rc1/python/lsst_daf_butler.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -17,53 +17,51 @@
 doc/lsst.daf.butler/queries.rst
 doc/lsst.daf.butler/use-in-tests.rst
 doc/lsst.daf.butler/writing-subcommands.rst
 python/lsst/__init__.py
 python/lsst/daf/__init__.py
 python/lsst/daf/butler/__init__.py
 python/lsst/daf/butler/_butler.py
+python/lsst/daf/butler/_butler_collections.py
 python/lsst/daf/butler/_butler_config.py
 python/lsst/daf/butler/_butler_instance_options.py
 python/lsst/daf/butler/_butler_repo_index.py
 python/lsst/daf/butler/_column_categorization.py
 python/lsst/daf/butler/_column_tags.py
 python/lsst/daf/butler/_column_type_info.py
 python/lsst/daf/butler/_config.py
 python/lsst/daf/butler/_config_support.py
 python/lsst/daf/butler/_dataset_association.py
 python/lsst/daf/butler/_dataset_existence.py
 python/lsst/daf/butler/_dataset_ref.py
 python/lsst/daf/butler/_dataset_type.py
 python/lsst/daf/butler/_deferredDatasetHandle.py
 python/lsst/daf/butler/_exceptions.py
+python/lsst/daf/butler/_exceptions_legacy.py
 python/lsst/daf/butler/_file_dataset.py
 python/lsst/daf/butler/_file_descriptor.py
 python/lsst/daf/butler/_formatter.py
 python/lsst/daf/butler/_labeled_butler_factory.py
 python/lsst/daf/butler/_limited_butler.py
 python/lsst/daf/butler/_location.py
 python/lsst/daf/butler/_named.py
 python/lsst/daf/butler/_quantum.py
 python/lsst/daf/butler/_quantum_backed.py
-python/lsst/daf/butler/_query.py
-python/lsst/daf/butler/_query_results.py
 python/lsst/daf/butler/_registry_shim.py
 python/lsst/daf/butler/_storage_class.py
 python/lsst/daf/butler/_storage_class_delegate.py
 python/lsst/daf/butler/_timespan.py
 python/lsst/daf/butler/_topology.py
 python/lsst/daf/butler/arrow_utils.py
 python/lsst/daf/butler/column_spec.py
 python/lsst/daf/butler/ddl.py
-python/lsst/daf/butler/direct_butler.py
-python/lsst/daf/butler/direct_query.py
-python/lsst/daf/butler/direct_query_results.py
 python/lsst/daf/butler/json.py
 python/lsst/daf/butler/logging.py
 python/lsst/daf/butler/mapping_factory.py
+python/lsst/daf/butler/name_shrinker.py
 python/lsst/daf/butler/nonempty_mapping.py
 python/lsst/daf/butler/persistence_context.py
 python/lsst/daf/butler/progress.py
 python/lsst/daf/butler/py.typed
 python/lsst/daf/butler/pydantic_utils.py
 python/lsst/daf/butler/repo_relocation.py
 python/lsst/daf/butler/time_utils.py
@@ -92,14 +90,17 @@
 python/lsst/daf/butler/configs/registry.yaml
 python/lsst/daf/butler/configs/repo_transfer_formats.yaml
 python/lsst/daf/butler/configs/storageClasses.yaml
 python/lsst/daf/butler/configs/datastores/composites.yaml
 python/lsst/daf/butler/configs/datastores/fileDatastore.yaml
 python/lsst/daf/butler/configs/datastores/formatters.yaml
 python/lsst/daf/butler/configs/datastores/writeRecipes.yaml
+python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe5.yaml
+python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe6.yaml
+python/lsst/daf/butler/configs/old_dimensions/daf_butler_universe7.yaml
 python/lsst/daf/butler/datastore/__init__.py
 python/lsst/daf/butler/datastore/_datastore.py
 python/lsst/daf/butler/datastore/cache_manager.py
 python/lsst/daf/butler/datastore/composites.py
 python/lsst/daf/butler/datastore/constraints.py
 python/lsst/daf/butler/datastore/file_templates.py
 python/lsst/daf/butler/datastore/generic_base.py
@@ -133,24 +134,53 @@
 python/lsst/daf/butler/dimensions/_record_table.py
 python/lsst/daf/butler/dimensions/_records.py
 python/lsst/daf/butler/dimensions/_schema.py
 python/lsst/daf/butler/dimensions/_skypix.py
 python/lsst/daf/butler/dimensions/_universe.py
 python/lsst/daf/butler/dimensions/construction.py
 python/lsst/daf/butler/dimensions/record_cache.py
+python/lsst/daf/butler/direct_butler/__init__.py
+python/lsst/daf/butler/direct_butler/_direct_butler.py
+python/lsst/daf/butler/direct_butler/_direct_butler_collections.py
+python/lsst/daf/butler/direct_query_driver/__init__.py
+python/lsst/daf/butler/direct_query_driver/_driver.py
+python/lsst/daf/butler/direct_query_driver/_postprocessing.py
+python/lsst/daf/butler/direct_query_driver/_query_builder.py
+python/lsst/daf/butler/direct_query_driver/_query_plan.py
+python/lsst/daf/butler/direct_query_driver/_sql_column_visitor.py
 python/lsst/daf/butler/formatters/__init__.py
 python/lsst/daf/butler/formatters/astropyTable.py
 python/lsst/daf/butler/formatters/file.py
 python/lsst/daf/butler/formatters/json.py
 python/lsst/daf/butler/formatters/logs.py
 python/lsst/daf/butler/formatters/matplotlib.py
 python/lsst/daf/butler/formatters/packages.py
 python/lsst/daf/butler/formatters/parquet.py
 python/lsst/daf/butler/formatters/pickle.py
 python/lsst/daf/butler/formatters/yaml.py
+python/lsst/daf/butler/queries/__init__.py
+python/lsst/daf/butler/queries/_base.py
+python/lsst/daf/butler/queries/_data_coordinate_query_results.py
+python/lsst/daf/butler/queries/_dataset_query_results.py
+python/lsst/daf/butler/queries/_dimension_record_query_results.py
+python/lsst/daf/butler/queries/_query.py
+python/lsst/daf/butler/queries/convert_args.py
+python/lsst/daf/butler/queries/driver.py
+python/lsst/daf/butler/queries/expression_factory.py
+python/lsst/daf/butler/queries/overlaps.py
+python/lsst/daf/butler/queries/result_specs.py
+python/lsst/daf/butler/queries/visitors.py
+python/lsst/daf/butler/queries/tree/__init__.py
+python/lsst/daf/butler/queries/tree/_base.py
+python/lsst/daf/butler/queries/tree/_column_expression.py
+python/lsst/daf/butler/queries/tree/_column_literal.py
+python/lsst/daf/butler/queries/tree/_column_reference.py
+python/lsst/daf/butler/queries/tree/_column_set.py
+python/lsst/daf/butler/queries/tree/_predicate.py
+python/lsst/daf/butler/queries/tree/_query_tree.py
 python/lsst/daf/butler/registry/__init__.py
 python/lsst/daf/butler/registry/_caching_context.py
 python/lsst/daf/butler/registry/_collection_record_cache.py
 python/lsst/daf/butler/registry/_collection_summary.py
 python/lsst/daf/butler/registry/_collection_summary_cache.py
 python/lsst/daf/butler/registry/_collection_type.py
 python/lsst/daf/butler/registry/_config.py
@@ -232,20 +262,21 @@
 python/lsst/daf/butler/registry/tests/_database.py
 python/lsst/daf/butler/registry/tests/_registry.py
 python/lsst/daf/butler/remote_butler/__init__.py
 python/lsst/daf/butler/remote_butler/_authentication.py
 python/lsst/daf/butler/remote_butler/_collection_args.py
 python/lsst/daf/butler/remote_butler/_config.py
 python/lsst/daf/butler/remote_butler/_factory.py
+python/lsst/daf/butler/remote_butler/_http_connection.py
+python/lsst/daf/butler/remote_butler/_ref_utils.py
 python/lsst/daf/butler/remote_butler/_registry.py
 python/lsst/daf/butler/remote_butler/_remote_butler.py
 python/lsst/daf/butler/remote_butler/server_models.py
 python/lsst/daf/butler/remote_butler/server/__init__.py
 python/lsst/daf/butler/remote_butler/server/_dependencies.py
-python/lsst/daf/butler/remote_butler/server/_exceptions.py
 python/lsst/daf/butler/remote_butler/server/_factory.py
 python/lsst/daf/butler/remote_butler/server/_server.py
 python/lsst/daf/butler/remote_butler/server/handlers/_external.py
 python/lsst/daf/butler/remote_butler/server/handlers/_internal.py
 python/lsst/daf/butler/script/__init__.py
 python/lsst/daf/butler/script/_associate.py
 python/lsst/daf/butler/script/_pruneDatasets.py
@@ -269,15 +300,15 @@
 python/lsst/daf/butler/script/retrieveArtifacts.py
 python/lsst/daf/butler/script/transferDatasets.py
 python/lsst/daf/butler/tests/__init__.py
 python/lsst/daf/butler/tests/_datasetsHelper.py
 python/lsst/daf/butler/tests/_dummyRegistry.py
 python/lsst/daf/butler/tests/_examplePythonTypes.py
 python/lsst/daf/butler/tests/_testRepo.py
-python/lsst/daf/butler/tests/butler_query.py
+python/lsst/daf/butler/tests/butler_queries.py
 python/lsst/daf/butler/tests/cliCmdTestBase.py
 python/lsst/daf/butler/tests/cliLogTestBase.py
 python/lsst/daf/butler/tests/deferredFormatter.py
 python/lsst/daf/butler/tests/dict_convertible_model.py
 python/lsst/daf/butler/tests/hybrid_butler.py
 python/lsst/daf/butler/tests/hybrid_butler_registry.py
 python/lsst/daf/butler/tests/server.py
@@ -295,15 +326,14 @@
 python/lsst_daf_butler.egg-info/requires.txt
 python/lsst_daf_butler.egg-info/top_level.txt
 python/lsst_daf_butler.egg-info/zip-safe
 tests/test_astropyTableFormatter.py
 tests/test_authentication.py
 tests/test_butler.py
 tests/test_butler_factory.py
-tests/test_butler_query.py
 tests/test_cliCmdAssociate.py
 tests/test_cliCmdConfigDump.py
 tests/test_cliCmdConfigValidate.py
 tests/test_cliCmdCreate.py
 tests/test_cliCmdImport.py
 tests/test_cliCmdIngestFiles.py
 tests/test_cliCmdPruneDatasets.py
@@ -344,15 +374,19 @@
 tests/test_packages.py
 tests/test_parquet.py
 tests/test_postgresql.py
 tests/test_progress.py
 tests/test_pydantic_utils.py
 tests/test_quantum.py
 tests/test_quantumBackedButler.py
+tests/test_query_direct_postgresql.py
+tests/test_query_direct_sqlite.py
+tests/test_query_interface.py
 tests/test_query_relations.py
+tests/test_query_utilities.py
 tests/test_remote_butler.py
 tests/test_server.py
 tests/test_simpleButler.py
 tests/test_sqlite.py
 tests/test_storageClass.py
 tests/test_templates.py
 tests/test_testRepo.py
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_astropyTableFormatter.py` & `lsst_daf_butler-27.0.0rc1/tests/test_astropyTableFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_authentication.py` & `lsst_daf_butler-27.0.0rc1/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_butler.py` & `lsst_daf_butler-27.0.0rc1/tests/test_butler.py`

 * *Files 11% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 import posixpath
 import random
 import shutil
 import string
 import tempfile
 import unittest
 import uuid
-from collections.abc import Mapping
+from collections.abc import Callable, Mapping
 from typing import TYPE_CHECKING, Any, cast
 
 try:
     import boto3
     import botocore
     from lsst.resources.s3utils import clean_test_environment_for_s3
 
@@ -78,18 +78,20 @@
 
 import astropy.time
 import sqlalchemy
 from lsst.daf.butler import (
     Butler,
     ButlerConfig,
     ButlerRepoIndex,
+    CollectionCycleError,
     CollectionType,
     Config,
     DataCoordinate,
     DatasetExistence,
+    DatasetNotFoundError,
     DatasetRef,
     DatasetType,
     FileDataset,
     NoDefaultCollectionError,
     StorageClassFactory,
     ValidationError,
     script,
@@ -242,37 +244,40 @@
         butler.registry.insertDimensionData("instrument", {"name": "DummyCamComp"})
         butler.registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCamComp", "name": "d-r", "band": "R"}
         )
         butler.registry.insertDimensionData(
             "visit_system", {"instrument": "DummyCamComp", "id": 1, "name": "default"}
         )
+        butler.registry.insertDimensionData("day_obs", {"instrument": "DummyCamComp", "id": 20200101})
         visit_start = astropy.time.Time("2020-01-01 08:00:00.123456789", scale="tai")
         visit_end = astropy.time.Time("2020-01-01 08:00:36.66", scale="tai")
         butler.registry.insertDimensionData(
             "visit",
             {
                 "instrument": "DummyCamComp",
                 "id": 423,
                 "name": "fourtwentythree",
                 "physical_filter": "d-r",
                 "datetime_begin": visit_start,
                 "datetime_end": visit_end,
+                "day_obs": 20200101,
             },
         )
 
         # Add more visits for some later tests
         for visit_id in (424, 425):
             butler.registry.insertDimensionData(
                 "visit",
                 {
                     "instrument": "DummyCamComp",
                     "id": visit_id,
                     "name": f"fourtwentyfour_{visit_id}",
                     "physical_filter": "d-r",
+                    "day_obs": 20200101,
                 },
             )
         return butler, datasetType
 
     def runPutGetTest(self, storageClass: StorageClass, datasetTypeName: str) -> Butler:
         # New datasets will be added to run and tag, but we will only look in
         # tag when looking up datasets.
@@ -280,14 +285,18 @@
         butler, datasetType = self.create_butler(run, storageClass, datasetTypeName)
         assert butler.run is not None
 
         # Create and store a dataset
         metric = makeExampleMetrics()
         dataId = butler.registry.expandDataId({"instrument": "DummyCamComp", "visit": 423})
 
+        # Dataset should not exist if we haven't added it
+        with self.assertRaises(DatasetNotFoundError):
+            butler.get(datasetTypeName, dataId)
+
         # Put and remove the dataset once as a DatasetRef, once as a dataId,
         # and once with a DatasetType
 
         # Keep track of any collections we add and do not clean up
         expected_collections = {run}
 
         counter = 0
@@ -406,15 +415,15 @@
                 butler.pruneDatasets([ref], purge=True, unstore=True)
                 # Lookup with original args should still fail.
                 kwargs = {"collections": this_run}
                 if isinstance(args[0], DatasetRef):
                     kwargs = {}  # Prevent warning from being issued.
                 self.assertFalse(butler.exists(*args, **kwargs))
                 # get() should still fail.
-                with self.assertRaises(FileNotFoundError):
+                with self.assertRaises((FileNotFoundError, DatasetNotFoundError)):
                     butler.get(ref)
                 # Registry shouldn't be able to find it by dataset_id anymore.
                 self.assertIsNone(butler.get_dataset(ref.id))
 
                 # Do explicit registry removal since we know they are
                 # empty
                 butler.registry.removeCollection(this_run)
@@ -489,15 +498,15 @@
         ):
             butler.get(inconsistentDatasetType, dataId)
 
         # Combining a DatasetRef with a dataId should fail
         with self.assertRaisesRegex(ValueError, "DatasetRef given, cannot use dataId as well"):
             butler.get(ref, dataId)
         # Getting with an explicit ref should fail if the id doesn't match.
-        with self.assertRaises(FileNotFoundError):
+        with self.assertRaises((FileNotFoundError, DatasetNotFoundError)):
             butler.get(DatasetRef(ref.datasetType, ref.dataId, id=uuid.UUID(int=101), run=butler.run))
 
         # Getting a dataset with unknown parameters should fail
         with self.assertRaisesRegex(KeyError, "Parameter 'unsupported' not understood"):
             butler.get(ref, parameters={"unsupported": True})
 
         # Check we have a collection
@@ -554,17 +563,24 @@
             "example", dimensions, self.storageClassFactory.getStorageClass("StructuredData"), butler.registry
         )
         # Add needed Dimensions
         butler.registry.insertDimensionData("instrument", {"name": "DummyCamComp"})
         butler.registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCamComp", "name": "d-r", "band": "R"}
         )
+        butler.registry.insertDimensionData("day_obs", {"instrument": "DummyCamComp", "id": 20250101})
         butler.registry.insertDimensionData(
             "visit",
-            {"instrument": "DummyCamComp", "id": 423, "name": "fourtwentythree", "physical_filter": "d-r"},
+            {
+                "instrument": "DummyCamComp",
+                "id": 423,
+                "name": "fourtwentythree",
+                "physical_filter": "d-r",
+                "day_obs": 20250101,
+            },
         )
         dataId = {"instrument": "DummyCamComp", "visit": 423}
         # Create dataset.
         metric = makeExampleMetrics()
         # Register a new run and put dataset.
         run = "deferred"
         self.assertTrue(butler.registry.registerRun(run))
@@ -925,23 +941,36 @@
         datasetType = self.addDatasetType(datasetTypeName, dimensions, storageClass, butler.registry)
 
         # Add needed Dimensions
         butler.registry.insertDimensionData("instrument", {"name": "DummyCamComp"})
         butler.registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCamComp", "name": "d-r", "band": "R"}
         )
+        butler.registry.insertDimensionData("day_obs", {"instrument": "DummyCamComp", "id": 20250101})
         for detector in (1, 2):
             butler.registry.insertDimensionData(
                 "detector", {"instrument": "DummyCamComp", "id": detector, "full_name": f"detector{detector}"}
             )
 
         butler.registry.insertDimensionData(
             "visit",
-            {"instrument": "DummyCamComp", "id": 423, "name": "fourtwentythree", "physical_filter": "d-r"},
-            {"instrument": "DummyCamComp", "id": 424, "name": "fourtwentyfour", "physical_filter": "d-r"},
+            {
+                "instrument": "DummyCamComp",
+                "id": 423,
+                "name": "fourtwentythree",
+                "physical_filter": "d-r",
+                "day_obs": 20250101,
+            },
+            {
+                "instrument": "DummyCamComp",
+                "id": 424,
+                "name": "fourtwentyfour",
+                "physical_filter": "d-r",
+                "day_obs": 20250101,
+            },
         )
 
         formatter = doImportType("lsst.daf.butler.formatters.yaml.YamlFormatter")
         dataRoot = os.path.join(TESTDIR, "data", "basic")
         datasets = []
         for detector in (1, 2):
             detector_name = f"detector_{detector}"
@@ -1083,15 +1112,27 @@
                 [
                     {"instrument": "DummyCam"},
                     {"instrument": "DummyHSC"},
                     {"instrument": "DummyCamComp"},
                 ],
             ),
             ("physical_filter", [{"instrument": "DummyCam", "name": "d-r", "band": "R"}]),
-            ("visit", [{"instrument": "DummyCam", "id": 42, "name": "fortytwo", "physical_filter": "d-r"}]),
+            ("day_obs", [{"instrument": "DummyCam", "id": 20250101}]),
+            (
+                "visit",
+                [
+                    {
+                        "instrument": "DummyCam",
+                        "id": 42,
+                        "name": "fortytwo",
+                        "physical_filter": "d-r",
+                        "day_obs": 20250101,
+                    }
+                ],
+            ),
         ]
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         # Add needed Dimensions
         for element, data in dimensionEntries:
             butler.registry.insertDimensionData(element, *data)
 
         # When a DatasetType is added to the registry entries are not created
@@ -1151,15 +1192,25 @@
     def testTransaction(self) -> None:
         butler = self.create_empty_butler(run=self.default_run)
         datasetTypeName = "test_metric"
         dimensions = butler.dimensions.conform(["instrument", "visit"])
         dimensionEntries: tuple[tuple[str, Mapping[str, Any]], ...] = (
             ("instrument", {"instrument": "DummyCam"}),
             ("physical_filter", {"instrument": "DummyCam", "name": "d-r", "band": "R"}),
-            ("visit", {"instrument": "DummyCam", "id": 42, "name": "fortytwo", "physical_filter": "d-r"}),
+            ("day_obs", {"instrument": "DummyCam", "id": 20250101}),
+            (
+                "visit",
+                {
+                    "instrument": "DummyCam",
+                    "id": 42,
+                    "name": "fortytwo",
+                    "physical_filter": "d-r",
+                    "day_obs": 20250101,
+                },
+            ),
         )
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         metric = makeExampleMetrics()
         dataId = {"instrument": "DummyCam", "visit": 42}
         # Create and register a DatasetType
         datasetType = self.addDatasetType(datasetTypeName, dimensions, storageClass, butler.registry)
         with self.assertRaises(TransactionTestError):
@@ -1270,24 +1321,28 @@
         dimensions = butler.dimensions.conform(["instrument", "exposure"])
         datasetType = DatasetType(datasetTypeName, dimensions, storageClass)
         butler.registry.registerDatasetType(datasetType)
 
         n_exposures = 5
         dayobs = 20210530
 
+        butler.registry.insertDimensionData("day_obs", {"instrument": "DummyCamComp", "id": dayobs})
+
         for i in range(n_exposures):
+            butler.registry.insertDimensionData("group", {"instrument": "DummyCamComp", "name": f"group{i}"})
             butler.registry.insertDimensionData(
                 "exposure",
                 {
                     "instrument": "DummyCamComp",
                     "id": i,
                     "obs_id": f"exp{i}",
                     "seq_num": i,
                     "day_obs": dayobs,
                     "physical_filter": "d-r",
+                    "group": f"group{i}",
                 },
             )
 
         # Write some data.
         for i in range(n_exposures):
             metric = {"something": i, "other": "metric", "list": [2 * x for x in range(i)]}
 
@@ -1298,25 +1353,175 @@
             # Check that the exposure is correct in the dataId
             self.assertEqual(ref.dataId["exposure"], i)
 
             # and check that we can get the dataset back with the same dataId
             new_metric = butler.get(datasetTypeName, dataId=dataId)
             self.assertEqual(new_metric, metric)
 
+        # Check that we can find the datasets using the day_obs or the
+        # exposure.day_obs.
+        datasets_1 = list(
+            butler.registry.queryDatasets(
+                datasetType,
+                collections=self.default_run,
+                where="day_obs = dayObs AND instrument = instr",
+                bind={"dayObs": dayobs, "instr": "DummyCamComp"},
+            )
+        )
+        datasets_2 = list(
+            butler.registry.queryDatasets(
+                datasetType,
+                collections=self.default_run,
+                where="exposure.day_obs = dayObs AND instrument = instr",
+                bind={"dayObs": dayobs, "instr": "DummyCamComp"},
+            )
+        )
+        self.assertEqual(datasets_1, datasets_2)
+
     def testGetDatasetCollectionCaching(self):
         # Prior to DM-41117, there was a bug where get_dataset would throw
         # MissingCollectionError if you tried to fetch a dataset that was added
         # after the collection cache was last updated.
         reader_butler, datasetType = self.create_butler(self.default_run, "int", "datasettypename")
         writer_butler = self.create_empty_butler(writeable=True, run="new_run")
         dataId = {"instrument": "DummyCamComp", "visit": 423}
         put_ref = writer_butler.put(123, datasetType, dataId)
         get_ref = reader_butler.get_dataset(put_ref.id)
         self.assertEqual(get_ref.id, put_ref.id)
 
+    def testCollectionChainRedefine(self):
+        butler = self._setup_to_test_collection_chain()
+
+        butler.collection_chains.redefine_chain("chain", "a")
+        self._check_chain(butler, ["a"])
+
+        # Duplicates are removed from the list of children
+        butler.collection_chains.redefine_chain("chain", ["c", "b", "c"])
+        self._check_chain(butler, ["c", "b"])
+
+        # Empty list clears the chain
+        butler.collection_chains.redefine_chain("chain", [])
+        self._check_chain(butler, [])
+
+        self._test_common_chain_functionality(butler, butler.collection_chains.redefine_chain)
+
+    def testCollectionChainPrepend(self):
+        butler = self._setup_to_test_collection_chain()
+
+        # Duplicates are removed from the list of children
+        butler.collection_chains.prepend_chain("chain", ["c", "b", "c"])
+        self._check_chain(butler, ["c", "b"])
+
+        # Prepend goes on the front of existing chain
+        butler.collection_chains.prepend_chain("chain", ["a"])
+        self._check_chain(butler, ["a", "c", "b"])
+
+        # Empty prepend does nothing
+        butler.collection_chains.prepend_chain("chain", [])
+        self._check_chain(butler, ["a", "c", "b"])
+
+        # Prepending children that already exist in the chain removes them from
+        # their current position.
+        butler.collection_chains.prepend_chain("chain", ["d", "b", "c"])
+        self._check_chain(butler, ["d", "b", "c", "a"])
+
+        self._test_common_chain_functionality(butler, butler.collection_chains.prepend_chain)
+
+    def testCollectionChainExtend(self):
+        butler = self._setup_to_test_collection_chain()
+
+        # Duplicates are removed from the list of children
+        butler.collection_chains.extend_chain("chain", ["c", "b", "c"])
+        self._check_chain(butler, ["c", "b"])
+
+        # Extend goes on the end of existing chain
+        butler.collection_chains.extend_chain("chain", ["a"])
+        self._check_chain(butler, ["c", "b", "a"])
+
+        # Empty extend does nothing
+        butler.collection_chains.extend_chain("chain", [])
+        self._check_chain(butler, ["c", "b", "a"])
+
+        # Extending children that already exist in the chain removes them from
+        # their current position.
+        butler.collection_chains.extend_chain("chain", ["d", "b", "c"])
+        self._check_chain(butler, ["a", "d", "b", "c"])
+
+        self._test_common_chain_functionality(butler, butler.collection_chains.extend_chain)
+
+    def testCollectionChainRemove(self) -> None:
+        butler = self._setup_to_test_collection_chain()
+
+        butler.registry.setCollectionChain("chain", ["a", "b", "c", "d"])
+
+        butler.collection_chains.remove_from_chain("chain", "c")
+        self._check_chain(butler, ["a", "b", "d"])
+
+        # Duplicates are allowed in the list of children
+        butler.collection_chains.remove_from_chain("chain", ["b", "b", "a"])
+        self._check_chain(butler, ["d"])
+
+        # Empty remove does nothing
+        butler.collection_chains.remove_from_chain("chain", [])
+        self._check_chain(butler, ["d"])
+
+        # Removing children that aren't in the chain does nothing
+        butler.collection_chains.remove_from_chain("chain", ["a", "chain"])
+        self._check_chain(butler, ["d"])
+
+        self._test_common_chain_functionality(
+            butler, butler.collection_chains.remove_from_chain, skip_cycle_check=True
+        )
+
+    def _setup_to_test_collection_chain(self) -> Butler:
+        butler = self.create_empty_butler(writeable=True)
+
+        butler.registry.registerCollection("chain", CollectionType.CHAINED)
+
+        runs = ["a", "b", "c", "d"]
+        for run in runs:
+            butler.registry.registerCollection(run)
+
+        butler.registry.registerCollection("staticchain", CollectionType.CHAINED)
+        butler.registry.setCollectionChain("staticchain", ["a", "b"])
+
+        return butler
+
+    def _check_chain(self, butler: Butler, expected: list[str]) -> None:
+        children = butler.registry.getCollectionChain("chain")
+        self.assertEqual(expected, list(children))
+
+    def _test_common_chain_functionality(
+        self, butler, func: Callable[[str, str | list[str]], Any], *, skip_cycle_check=False
+    ) -> None:
+        # Missing parent collection
+        with self.assertRaises(MissingCollectionError):
+            func("doesnotexist", [])
+        # Missing child collection
+        with self.assertRaises(MissingCollectionError):
+            func("chain", ["doesnotexist"])
+        # Forbid operations on non-chained collections
+        with self.assertRaises(CollectionTypeError):
+            func("d", ["a"])
+
+        # Prevent collection cycles
+        if not skip_cycle_check:
+            butler.registry.registerCollection("chain2", CollectionType.CHAINED)
+            func("chain2", "chain")
+            with self.assertRaises(CollectionCycleError):
+                func("chain", "chain2")
+
+        # Make sure none of the earlier operations interfered with unrelated
+        # chains.
+        self.assertEqual(["a", "b"], list(butler.registry.getCollectionChain("staticchain")))
+
+        with butler._caching_context():
+            with self.assertRaisesRegex(RuntimeError, "Chained collection modification not permitted"):
+                func("chain", "a")
+
 
 class FileDatastoreButlerTests(ButlerTests):
     """Common tests and specialization of ButlerTests for butlers backed
     by datastores that inherit from FileDatastore.
     """
 
     trustModeSupported = True
@@ -1335,19 +1540,34 @@
         butler = self.create_empty_butler(run=self.default_run)
 
         # Add needed Dimensions
         butler.registry.insertDimensionData("instrument", {"name": "DummyCamComp"})
         butler.registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCamComp", "name": "d-r", "band": "R"}
         )
+        butler.registry.insertDimensionData("day_obs", {"instrument": "DummyCamComp", "id": 20250101})
         butler.registry.insertDimensionData(
-            "visit", {"instrument": "DummyCamComp", "id": 423, "name": "v423", "physical_filter": "d-r"}
+            "visit",
+            {
+                "instrument": "DummyCamComp",
+                "id": 423,
+                "name": "v423",
+                "physical_filter": "d-r",
+                "day_obs": 20250101,
+            },
         )
         butler.registry.insertDimensionData(
-            "visit", {"instrument": "DummyCamComp", "id": 425, "name": "v425", "physical_filter": "d-r"}
+            "visit",
+            {
+                "instrument": "DummyCamComp",
+                "id": 425,
+                "name": "v425",
+                "physical_filter": "d-r",
+                "day_obs": 20250101,
+            },
         )
 
         # Create and store a dataset
         metric = makeExampleMetrics()
 
         # Create two almost-identical DatasetTypes (both will use default
         # template)
@@ -2291,19 +2511,36 @@
         self.source_butler.registry.insertDimensionData("instrument", {"name": "DummyCamComp"})
         self.source_butler.registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCamComp", "name": "d-r", "band": "R"}
         )
         self.source_butler.registry.insertDimensionData(
             "detector", {"instrument": "DummyCamComp", "id": 1, "full_name": "det1"}
         )
+        self.source_butler.registry.insertDimensionData(
+            "day_obs",
+            {
+                "instrument": "DummyCamComp",
+                "id": 20250101,
+            },
+        )
 
         for i in range(n_exposures):
             self.source_butler.registry.insertDimensionData(
+                "group", {"instrument": "DummyCamComp", "name": f"group{i}"}
+            )
+            self.source_butler.registry.insertDimensionData(
                 "exposure",
-                {"instrument": "DummyCamComp", "id": i, "obs_id": f"exp{i}", "physical_filter": "d-r"},
+                {
+                    "instrument": "DummyCamComp",
+                    "id": i,
+                    "obs_id": f"exp{i}",
+                    "physical_filter": "d-r",
+                    "group": f"group{i}",
+                    "day_obs": 20250101,
+                },
             )
 
         # Create dataset types in the source butler.
         dimensions = self.source_butler.dimensions.conform(["instrument", "exposure"])
         for datasetTypeName in datasetTypeNames:
             datasetType = DatasetType(datasetTypeName, dimensions, storageClass)
             self.source_butler.registry.registerDatasetType(datasetType)
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_butler_factory.py` & `lsst_daf_butler-27.0.0rc1/tests/test_butler_factory.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdAssociate.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdAssociate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigDump.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdConfigDump.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdConfigValidate.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdConfigValidate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdCreate.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdCreate.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdImport.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliLog.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,50 +21,49 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for daf_butler CLI config-dump command.
+"""Unit tests for the daf_butler dataset-type CLI option.
 """
 
+import logging
 import unittest
-import unittest.mock
 
-from lsst.daf.butler.cli.cmd import butler_import
-from lsst.daf.butler.tests import CliCmdTestBase
+from lsst.daf.butler.cli.cliLog import CliLog
+from lsst.daf.butler.tests import CliLogTestBase
 
-
-class ImportTestCase(CliCmdTestBase, unittest.TestCase):
-    """Test the butler import command-line."""
-
-    mockFuncName = "lsst.daf.butler.cli.cmd.commands.script.butlerImport"
-
-    @staticmethod
-    def defaultExpected():
-        return dict(repo=None, transfer="auto", directory=None, skip_dimensions=(), export_file=None)
-
-    @staticmethod
-    def command():
-        return butler_import
-
-    def test_minimal(self):
-        """Test only required parameters, and omit optional parameters."""
-        self.run_test(["import", "here", "foo"], self.makeExpected(repo="here", directory="foo"))
-
-    def test_all(self):
-        """Test all the parameters."""
-        self.run_test(
-            ["import", "here", "foo", "--transfer", "symlink", "--export-file", "file"],
-            self.makeExpected(repo="here", directory="foo", transfer="symlink", export_file="file"),
-        )
-
-    def test_missingArgument(self):
-        """Verify the command fails if either of the positional arguments,
-        REPO or DIRECTORY, is missing.
-        """
-        self.run_missing(["import", "foo"], r"Error: Missing argument ['\"]DIRECTORY['\"].")
+try:
+    import lsst.log as lsstLog
+except ModuleNotFoundError:
+    lsstLog = None
+
+
+class CliLogTestCase(CliLogTestBase, unittest.TestCase):
+    """Test log initialization, reset, and setting log levels on python
+    `logging` and also `lsst.log` if it is setup.
+
+    This will not test use of `lsst.log` in CI because daf_butler does not
+    directly depend on that package. When running in an environment where
+    `lsst.log` is setup then this will test use of `lsst.log`. This test also
+    runs in obs_base which does provide coverage of python `logging` and
+    `lsst.log` in CI.
+    """
+
+    pass
+
+
+class ConvertPyLogLevelTestCase(unittest.TestCase):
+    """Test python command-line log levels."""
+
+    def test_convertToPyLogLevel(self):
+        self.assertEqual(logging.CRITICAL, CliLog._getPyLogLevel("CRITICAL"))
+        self.assertEqual(logging.ERROR, CliLog._getPyLogLevel("ERROR"))
+        self.assertEqual(logging.WARN, CliLog._getPyLogLevel("WARNING"))
+        self.assertEqual(logging.INFO, CliLog._getPyLogLevel("INFO"))
+        self.assertEqual(logging.DEBUG, CliLog._getPyLogLevel("DEBUG"))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdIngestFiles.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdIngestFiles.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdPruneDatasets.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdPruneDatasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryCollections.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryCollections.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,10 +295,14 @@
             self.assertChain(
                 ["--mode", "redefine", "chain1", "chain2", "run2", "run3,run4", "--flatten"],
                 "[calibration1, run1, run2, run3, run4]",
             )
 
             self.assertChain(["--mode", "pop", "chain1", "--", "-1", "-3"], "[calibration1, run1, run3]")
 
+            # Out-of-bounds index
+            result = self.runner.invoke(cli, ["collection-chain", "here", "--mode", "pop", "chain1", "10"])
+            self.assertEqual(result.exit_code, 1)
+
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDataIds.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDataIds.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasetTypes.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDatasetTypes.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,15 +133,15 @@
             # check verbose output:
             result = runner.invoke(cli, ["query-dataset-types", "here", "--verbose"])
             self.assertEqual(result.exit_code, 0, clickResultMsg(result))
             expected = AstropyTable(
                 array(
                     (
                         "test",
-                        "['band', 'instrument', 'physical_filter', 'visit']",
+                        "['band', 'instrument', 'day_obs', 'physical_filter', 'visit']",
                         storageClassName,
                     )
                 ),
                 names=("name", "dimensions", "storage class"),
             )
             self.assertAstropyTablesEqual(readTable(result.output), expected)
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDatasets.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDatasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,21 @@
     def testGlobDatasetType(self):
         """Test specifying dataset type."""
         # Create and register an additional DatasetType
         testRepo = MetricTestRepo(self.repoDir, configFile=self.configFile)
 
         testRepo.butler.registry.insertDimensionData(
             "visit",
-            {"instrument": "DummyCamComp", "id": 425, "name": "fourtwentyfive", "physical_filter": "d-r"},
+            {
+                "instrument": "DummyCamComp",
+                "id": 425,
+                "name": "fourtwentyfive",
+                "physical_filter": "d-r",
+                "day_obs": 20200101,
+            },
         )
 
         datasetType = addDatasetType(
             testRepo.butler, "alt_test_metric_comp", ("instrument", "visit"), "StructuredCompositeReadComp"
         )
 
         testRepo.addDataset(dataId={"instrument": "DummyCamComp", "visit": 425}, datasetType=datasetType)
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdQueryDimensionRecords.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdQueryDimensionRecords.py`

 * *Files 4% similar despite different names*

```diff
@@ -54,17 +54,17 @@
 
     configFile = os.path.join(TESTDIR, "config/basic/butler.yaml")
     storageClassFactory = StorageClassFactory()
 
     expectedColumnNames = (
         "instrument",
         "id",
+        "day_obs",
         "physical_filter",
         "name",
-        "day_obs",
         "seq_num",
         "exposure_time",
         "target_name",
         "observation_reason",
         "science_program",
         "azimuth",
         "zenith_angle",
@@ -86,42 +86,42 @@
         result = self.runner.invoke(butlerCli, ["query-dimension-records", self.root, "visit"])
         self.assertEqual(result.exit_code, 0, clickResultMsg(result))
         rows = array(
             (
                 (
                     "DummyCamComp",
                     "423",
+                    "20200101",
                     "d-r",
                     "fourtwentythree",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
-                    "None",
                     "[2020-01-01T08:00:00, 2020-01-01T08:00:36)",
                 ),
                 (
                     "DummyCamComp",
                     "424",
+                    "20200101",
                     "d-r",
                     "fourtwentyfour",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
-                    "None",
                 ),
             )
         )
         expected = AstropyTable(rows, names=self.expectedColumnNames)
         got = readTable(result.output)
         self.assertAstropyTablesEqual(got, expected)
 
@@ -138,25 +138,25 @@
         )
         self.assertEqual(result.exit_code, 0, clickResultMsg(result))
         rows = array(
             (
                 (
                     "DummyCamComp",
                     "423",
+                    "20200101",
                     "d-r",
                     "fourtwentythree",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
-                    "None",
                     "[2020-01-01T08:00:00, 2020-01-01T08:00:36)",
                 ),
             )
         )
         expected = AstropyTable(rows, names=self.expectedColumnNames)
         self.assertAstropyTablesEqual(readTable(result.output), expected)
 
@@ -169,14 +169,15 @@
         self.testRepo.butler.registry.insertDimensionData(
             "visit",
             {
                 "instrument": "DummyCamComp",
                 "id": 425,
                 "name": "fourtwentyfive",
                 "physical_filter": "d-r",
+                "day_obs": 20200101,
             },
         )
         self.testRepo.addDataset(dataId={"instrument": "DummyCamComp", "visit": 425}, run="foo")
 
         # verify getting records from the "ingest/run" collection
         result = self.runner.invoke(
             butlerCli,
@@ -192,42 +193,42 @@
         )
         self.assertEqual(result.exit_code, 0, clickResultMsg(result))
         rows = array(
             (
                 (
                     "DummyCamComp",
                     "423",
+                    "20200101",
                     "d-r",
                     "fourtwentythree",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
-                    "None",
                     "[2020-01-01T08:00:00, 2020-01-01T08:00:36)",
                 ),
                 (
                     "DummyCamComp",
                     "424",
+                    "20200101",
                     "d-r",
                     "fourtwentyfour",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
-                    "None",
                 ),
             )
         )
         expected = AstropyTable(rows, names=self.expectedColumnNames)
         self.assertAstropyTablesEqual(readTable(result.output), expected)
 
         # verify getting records from the "foo" collection
@@ -245,24 +246,24 @@
         )
         self.assertEqual(result.exit_code, 0, clickResultMsg(result))
         rows = array(
             (
                 (
                     "DummyCamComp",
                     "425",
+                    "20200101",
                     "d-r",
                     "fourtwentyfive",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
                     "None",
-                    "None",
                     "None",
                     "None",
                 ),
             )
         )
         expected = AstropyTable(rows, names=self.expectedColumnNames)
         self.assertAstropyTablesEqual(readTable(result.output), expected)
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveCollections.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdRemoveCollections.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdRemoveRuns.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdRemoveRuns.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliCmdRetrieveArtifacts.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliCmdRetrieveArtifacts.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliLog.py` & `lsst_daf_butler-27.0.0rc1/tests/test_matplotlibFormatter.py`

 * *Files 21% similar despite different names*

```diff
@@ -21,49 +21,74 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
-"""Unit tests for the daf_butler dataset-type CLI option.
+"""Tests for MatplotlibFormatter.
 """
 
-import logging
+import os
+import tempfile
 import unittest
-
-from lsst.daf.butler.cli.cliLog import CliLog
-from lsst.daf.butler.tests import CliLogTestBase
+from random import Random
 
 try:
-    import lsst.log as lsstLog
-except ModuleNotFoundError:
-    lsstLog = None
-
-
-class CliLogTestCase(CliLogTestBase, unittest.TestCase):
-    """Test log initialization, reset, and setting log levels on python
-    `logging` and also `lsst.log` if it is setup.
-
-    This will not test use of `lsst.log` in CI because daf_butler does not
-    directly depend on that package. When running in an environment where
-    `lsst.log` is setup then this will test use of `lsst.log`. This test also
-    runs in obs_base which does provide coverage of python `logging` and
-    `lsst.log` in CI.
-    """
-
-    pass
-
-
-class ConvertPyLogLevelTestCase(unittest.TestCase):
-    """Test python command-line log levels."""
-
-    def test_convertToPyLogLevel(self):
-        self.assertEqual(logging.CRITICAL, CliLog._getPyLogLevel("CRITICAL"))
-        self.assertEqual(logging.ERROR, CliLog._getPyLogLevel("ERROR"))
-        self.assertEqual(logging.WARN, CliLog._getPyLogLevel("WARNING"))
-        self.assertEqual(logging.INFO, CliLog._getPyLogLevel("INFO"))
-        self.assertEqual(logging.DEBUG, CliLog._getPyLogLevel("DEBUG"))
+    import matplotlib
+
+    matplotlib.use("Agg")
+    from matplotlib import pyplot
+except ImportError:
+    pyplot = None
+
+import filecmp
+
+from lsst.daf.butler import Butler, DatasetType
+from lsst.daf.butler.tests.utils import makeTestTempDir, removeTestTempDir
+
+TESTDIR = os.path.abspath(os.path.dirname(__file__))
+
+
+@unittest.skipIf(pyplot is None, "skipping test because matplotlib import failed")
+class MatplotlibFormatterTestCase(unittest.TestCase):
+    """Test for MatplotlibFormatter."""
+
+    RANDOM_SEED = 10
+
+    def setUp(self):
+        self.root = makeTestTempDir(TESTDIR)
+        Butler.makeRepo(self.root)
+        # Create a random image for testing
+        self.rng = Random(self.RANDOM_SEED)
+
+    def tearDown(self):
+        removeTestTempDir(self.root)
+
+    def testMatplotlibFormatter(self):
+        butler = Butler.from_config(self.root, run="testrun")
+        datasetType = DatasetType("test_plot", [], "Plot", universe=butler.dimensions)
+        butler.registry.registerDatasetType(datasetType)
+        # Does not have to be a random image
+        pyplot.imshow(
+            [
+                self.rng.sample(range(50), 10),
+                self.rng.sample(range(50), 10),
+                self.rng.sample(range(50), 10),
+            ]
+        )
+        ref = butler.put(pyplot.gcf(), datasetType)
+        uri = butler.getURI(ref)
+
+        # Following test needs a local file
+        with uri.as_local() as local, tempfile.NamedTemporaryFile(suffix=".png") as file:
+            pyplot.gcf().savefig(file.name)
+            self.assertTrue(filecmp.cmp(local.ospath, file.name, shallow=True))
+        self.assertTrue(butler.exists(ref))
+        with self.assertRaises(ValueError):
+            butler.get(ref)
+        butler.pruneDatasets([ref], unstore=True, purge=True)
+        self.assertFalse(butler.exists(ref))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliPluginLoader.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliPluginLoader.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitCommas.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliUtilSplitCommas.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliUtilSplitKv.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliUtilSplitKv.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliUtilToUpper.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliUtilToUpper.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_cliUtils.py` & `lsst_daf_butler-27.0.0rc1/tests/test_cliUtils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_composites.py` & `lsst_daf_butler-27.0.0rc1/tests/test_composites.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_config.py` & `lsst_daf_butler-27.0.0rc1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_connectionString.py` & `lsst_daf_butler-27.0.0rc1/tests/test_connectionString.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_constraints.py` & `lsst_daf_butler-27.0.0rc1/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_datasets.py` & `lsst_daf_butler-27.0.0rc1/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_datastore.py` & `lsst_daf_butler-27.0.0rc1/tests/test_datastore.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 import pickle
 import shutil
 import tempfile
 import time
 import unittest
 import unittest.mock
 import uuid
-from collections.abc import Callable
-from typing import Any, Iterator, cast
+from collections.abc import Callable, Iterator
+from typing import Any, cast
 
 import lsst.utils.tests
 import yaml
 from lsst.daf.butler import (
     Config,
     DataCoordinate,
     DatasetIdGenEnum,
@@ -159,23 +159,35 @@
 
         sc2 = self.storageClassFactory.getStorageClass("ThingTwo")
         if self.validationCanFail:
             with self.assertRaises(DatastoreValidationError):
                 datastore.validateConfiguration([sc2], logFailures=True)
 
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
         ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
         datastore.validateConfiguration([ref])
 
     def testParameterValidation(self) -> None:
         """Check that parameters are validated"""
         sc = self.storageClassFactory.getStorageClass("ThingOne")
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
         ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
         datastore = self.makeDatastore()
         data = {1: 2, 3: 4}
         datastore.put(data, ref)
         newdata = datastore.get(ref)
         self.assertEqual(data, newdata)
         with self.assertRaises(KeyError):
@@ -188,16 +200,28 @@
         # Create multiple storage classes for testing different formulations
         storageClasses = [
             self.storageClassFactory.getStorageClass(sc)
             for sc in ("StructuredData", "StructuredDataJson", "StructuredDataPickle")
         ]
 
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
-        dataId2 = {"instrument": "dummy", "visit": 53, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
+        dataId2 = {
+            "instrument": "dummy",
+            "visit": 53,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
 
         for sc in storageClasses:
             ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
             ref2 = self.makeDatasetRef("metric", dimensions, sc, dataId2)
 
             # Make sure that using getManyURIs without predicting before the
             # dataset has been put raises.
@@ -250,15 +274,21 @@
                 self.assertEqual(len(uris), 1)
 
         storageClass = sc
 
         # Check that we can put a metric with None in a component and
         # get it back as None
         metricsNone = makeExampleMetrics(use_none=True)
-        dataIdNone = {"instrument": "dummy", "visit": 54, "physical_filter": "V", "band": "v"}
+        dataIdNone = {
+            "instrument": "dummy",
+            "visit": 54,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
         refNone = self.makeDatasetRef("metric", dimensions, sc, dataIdNone)
         datastore.put(metricsNone, refNone)
 
         comp = "data"
         for comp in ("data", "output"):
             compRef = refNone.makeComponentRef(comp)
             output = datastore.get(compRef)
@@ -308,15 +338,21 @@
             datastore.trustGetRequest = False
 
             # Create multiple storage classes for testing with or without
             # disassembly
             sc = self.storageClassFactory.getStorageClass(sc_name)
             dimensions = self.universe.conform(("visit", "physical_filter"))
 
-            dataId = {"instrument": "dummy", "visit": 52 + i, "physical_filter": "V", "band": "v"}
+            dataId = {
+                "instrument": "dummy",
+                "visit": 52 + i,
+                "physical_filter": "V",
+                "band": "v",
+                "day_obs": 20250101,
+            }
 
             ref = self.makeDatasetRef(datasetTypeName, dimensions, sc, dataId)
             datastore.put(metrics, ref)
 
             # Does it exist?
             self.assertTrue(datastore.exists(ref))
             self.assertTrue(datastore.knows(ref))
@@ -510,15 +546,21 @@
         metrics = makeExampleMetrics()
         datastore = self.makeDatastore()
         # Put
         dimensions = self.universe.conform(("visit", "physical_filter"))
         sc = self.storageClassFactory.getStorageClass("StructuredData")
         refs = []
         for i in range(n_refs):
-            dataId = {"instrument": "dummy", "visit": 638 + i, "physical_filter": "U", "band": "u"}
+            dataId = {
+                "instrument": "dummy",
+                "visit": 638 + i,
+                "physical_filter": "U",
+                "band": "u",
+                "day_obs": 20250101,
+            }
             ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
             datastore.put(metrics, ref)
 
             # Does it exist?
             self.assertTrue(datastore.exists(ref))
 
             # Get
@@ -571,15 +613,21 @@
         # Predicted URI should still point to the file.
         self.assertTrue(uri.exists())
 
     def testTransfer(self) -> None:
         metrics = makeExampleMetrics()
 
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 2048, "physical_filter": "Uprime", "band": "u"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 2048,
+            "physical_filter": "Uprime",
+            "band": "u",
+            "day_obs": 20250101,
+        }
 
         sc = self.storageClassFactory.getStorageClass("StructuredData")
         ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
 
         inputDatastore = self.makeDatastore("test_input_datastore")
         outputDatastore = self.makeDatastore("test_output_datastore")
 
@@ -591,15 +639,16 @@
 
     def testBasicTransaction(self) -> None:
         datastore = self.makeDatastore()
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         dimensions = self.universe.conform(("visit", "physical_filter"))
         nDatasets = 6
         dataIds = [
-            {"instrument": "dummy", "visit": i, "physical_filter": "V", "band": "v"} for i in range(nDatasets)
+            {"instrument": "dummy", "visit": i, "physical_filter": "V", "band": "v", "day_obs": 20250101}
+            for i in range(nDatasets)
         ]
         data = [
             (
                 self.makeDatasetRef("metric", dimensions, storageClass, dataId),
                 makeExampleMetrics(),
             )
             for dataId in dataIds
@@ -637,24 +686,36 @@
 
     def testNestedTransaction(self) -> None:
         datastore = self.makeDatastore()
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         dimensions = self.universe.conform(("visit", "physical_filter"))
         metrics = makeExampleMetrics()
 
-        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v"}
+        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v", "day_obs": 20250101}
         refBefore = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
         datastore.put(metrics, refBefore)
         with self.assertRaises(TransactionTestError):
             with datastore.transaction():
-                dataId = {"instrument": "dummy", "visit": 1, "physical_filter": "V", "band": "v"}
+                dataId = {
+                    "instrument": "dummy",
+                    "visit": 1,
+                    "physical_filter": "V",
+                    "band": "v",
+                    "day_obs": 20250101,
+                }
                 refOuter = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
                 datastore.put(metrics, refOuter)
                 with datastore.transaction():
-                    dataId = {"instrument": "dummy", "visit": 2, "physical_filter": "V", "band": "v"}
+                    dataId = {
+                        "instrument": "dummy",
+                        "visit": 2,
+                        "physical_filter": "V",
+                        "band": "v",
+                        "day_obs": 20250101,
+                    }
                     refInner = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
                     datastore.put(metrics, refInner)
                 # All datasets should exist
                 for ref in (refBefore, refOuter, refInner):
                     metricsOut = datastore.get(ref, parameters=None)
                     self.assertEqual(metrics, metricsOut)
                 raise TransactionTestError("This should roll back the transaction")
@@ -668,15 +729,15 @@
         with self.assertRaises(FileNotFoundError):
             datastore.get(refInner)
 
     def _prepareIngestTest(self) -> tuple[MetricsExample, DatasetRef]:
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         dimensions = self.universe.conform(("visit", "physical_filter"))
         metrics = makeExampleMetrics()
-        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v"}
+        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v", "day_obs": 20250101}
         ref = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
         return metrics, ref
 
     def runIngestTest(self, func: Callable[[MetricsExample, str, DatasetRef], None]) -> None:
         metrics, ref = self._prepareIngestTest()
         # The file will be deleted after the test.
         # For symlink tests this leads to a situation where the datastore
@@ -867,15 +928,21 @@
 
         metrics = makeExampleMetrics()
         dimensions = self.universe.conform(("visit", "physical_filter"))
         sc = self.storageClassFactory.getStorageClass("StructuredData")
 
         refs = []
         for visit in (2048, 2049, 2050):
-            dataId = {"instrument": "dummy", "visit": visit, "physical_filter": "Uprime", "band": "u"}
+            dataId = {
+                "instrument": "dummy",
+                "visit": visit,
+                "physical_filter": "Uprime",
+                "band": "u",
+                "day_obs": 20250101,
+            }
             ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
             datastore.put(metrics, ref)
             refs.append(ref)
         return datastore, refs
 
     def testExportImportRecords(self) -> None:
         """Test for export_records and import_records methods."""
@@ -928,15 +995,21 @@
         with self.assertRaises(TypeError):
             list(datastore.export(refs, directory="exportDir", transfer="move"))
 
         # Create a new ref that is not known to the datastore and try to
         # export it.
         sc = self.storageClassFactory.getStorageClass("ThingOne")
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
         ref = self.makeDatasetRef("metric", dimensions, sc, dataId)
         with self.assertRaises(FileNotFoundError):
             list(datastore.export(refs + [ref], transfer=None))
 
     def test_pydantic_dict_storage_class_conversions(self) -> None:
         """Test converting a dataset stored as a pydantic model into a dict on
         read.
@@ -1026,15 +1099,15 @@
     def testAtomicWrite(self) -> None:
         """Test that we write to a temporary and then rename"""
         datastore = self.makeDatastore()
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         dimensions = self.universe.conform(("visit", "physical_filter"))
         metrics = makeExampleMetrics()
 
-        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v"}
+        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v", "day_obs": 20250101}
         ref = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
 
         with self.assertLogs("lsst.resources", "DEBUG") as cm:
             datastore.put(metrics, ref)
         move_logs = [ll for ll in cm.output if "transfer=" in ll]
         self.assertIn("transfer=move", move_logs[0])
 
@@ -1053,15 +1126,21 @@
 
         sccomp = StorageClass("Dummy")
         compositeStorageClass = StorageClass(
             "StructuredComposite", components={"dummy": sccomp, "dummy2": sccomp}
         )
 
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
 
         ref = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
         compRef = self.makeDatasetRef("metric", dimensions, compositeStorageClass, dataId)
 
         def raiser(ref: DatasetRef) -> None:
             raise DatasetTypeNotSupportedError()
 
@@ -1105,15 +1184,15 @@
     def testChecksum(self) -> None:
         """Ensure that checksums have not been calculated."""
         datastore = self.makeDatastore()
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
         dimensions = self.universe.conform(("visit", "physical_filter"))
         metrics = makeExampleMetrics()
 
-        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v"}
+        dataId = {"instrument": "dummy", "visit": 0, "physical_filter": "V", "band": "v", "day_obs": 20250101}
         ref = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
 
         # Configuration should have disabled checksum calculation
         datastore.put(metrics, ref)
         infos = datastore.getStoredItemsInfo(ref)
         self.assertIsNone(infos[0].checksum)
 
@@ -1212,15 +1291,21 @@
         """Test that a failed formatter write does cleanup a partial file."""
         metrics = makeExampleMetrics()
         datastore = self.makeDatastore()
 
         storageClass = self.storageClassFactory.getStorageClass("StructuredData")
 
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
 
         ref = self.makeDatasetRef("metric", dimensions, storageClass, dataId)
 
         # Determine where the file will end up (we assume Formatters use
         # the same file extension)
         expectedUri = datastore.getURI(ref, predict=True)
         self.assertEqual(expectedUri.fragment, "predicted")
@@ -1293,15 +1378,21 @@
         """
         metrics = makeExampleMetrics()
         datastore = self.makeDatastore()
 
         sc1 = self.storageClassFactory.getStorageClass("StructuredData")
         sc2 = self.storageClassFactory.getStorageClass("StructuredDataJson")
         dimensions = self.universe.conform(("visit", "physical_filter", "instrument"))
-        dataId = {"visit": 52, "physical_filter": "V", "band": "v", "instrument": "DummyCamComp"}
+        dataId = {
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "instrument": "DummyCamComp",
+            "day_obs": 20250101,
+        }
 
         # Write empty file suitable for ingest check (JSON and YAML variants)
         testfile_y = tempfile.NamedTemporaryFile(suffix=".yaml")
         testfile_j = tempfile.NamedTemporaryFile(suffix=".json")
         for datasetTypeName, sc, accepted in (
             ("metric", sc1, True),
             ("metric5", sc1, False),
@@ -1391,16 +1482,22 @@
         """Test chained datastore constraints model."""
         metrics = makeExampleMetrics()
         datastore = self.makeDatastore()
 
         sc1 = self.storageClassFactory.getStorageClass("StructuredData")
         sc2 = self.storageClassFactory.getStorageClass("StructuredDataJson")
         dimensions = self.universe.conform(("visit", "physical_filter", "instrument"))
-        dataId1 = {"visit": 52, "physical_filter": "V", "band": "v", "instrument": "DummyCamComp"}
-        dataId2 = {"visit": 52, "physical_filter": "V", "band": "v", "instrument": "HSC"}
+        dataId1 = {
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "instrument": "DummyCamComp",
+            "day_obs": 20250101,
+        }
+        dataId2 = {"visit": 52, "physical_filter": "V", "band": "v", "instrument": "HSC", "day_obs": 20250101}
 
         # Write empty file suitable for ingest check (JSON and YAML variants)
         testfile_y = tempfile.NamedTemporaryFile(suffix=".yaml")
         testfile_j = tempfile.NamedTemporaryFile(suffix=".json")
 
         for typeName, dataId, sc, accept, ingest in (
             ("metric", dataId1, sc1, (False, True, False), True),
@@ -1478,15 +1575,21 @@
 
         # Create a root that we can use for caching tests.
         self.root = tempfile.mkdtemp()
 
         # Create some test dataset refs and associated test files
         sc = self.storageClassFactory.getStorageClass("StructuredDataDict")
         dimensions = self.universe.conform(("visit", "physical_filter"))
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "V", "band": "v"}
+        dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "V",
+            "band": "v",
+            "day_obs": 20250101,
+        }
 
         # Create list of refs and list of temporary files
         n_datasets = 10
         self.refs = [self.makeDatasetRef(f"metric{n}", dimensions, sc, dataId) for n in range(n_datasets)]
 
         root_uri = ResourcePath(self.root, forceDirectory=True)
         self.files = [root_uri.join(f"file{n}.txt") for n in range(n_datasets)]
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_ddl.py` & `lsst_daf_butler-27.0.0rc1/tests/test_ddl.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_dimension_record_containers.py` & `lsst_daf_butler-27.0.0rc1/tests/test_dimension_record_containers.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_dimensions.py` & `lsst_daf_butler-27.0.0rc1/tests/test_dimensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -239,14 +239,16 @@
             set(self.universe.getStaticDimensions().names),
             {
                 "instrument",
                 "visit",
                 "visit_system",
                 "exposure",
                 "detector",
+                "group",
+                "day_obs",
                 "physical_filter",
                 "band",
                 "subfilter",
                 "skymap",
                 "tract",
                 "patch",
             }
@@ -259,18 +261,18 @@
         for element in self.universe.getStaticElements():
             self.checkGroupInvariants(element.minimal_group)
 
     def testInstrumentDimensions(self):
         group = self.universe.conform(["exposure", "detector", "visit"])
         self.assertCountEqual(
             group.names,
-            ("instrument", "exposure", "detector", "visit", "physical_filter", "band"),
+            ("instrument", "exposure", "detector", "visit", "physical_filter", "band", "group", "day_obs"),
         )
         self.assertCountEqual(group.required, ("instrument", "exposure", "detector", "visit"))
-        self.assertCountEqual(group.implied, ("physical_filter", "band"))
+        self.assertCountEqual(group.implied, ("physical_filter", "band", "group", "day_obs"))
         self.assertCountEqual(group.elements - group.names, ("visit_detector_region", "visit_definition"))
         self.assertCountEqual(group.governors, {"instrument"})
         for element in group.elements:
             self.assertEqual(self.universe[element].has_own_table, element != "band", element)
             self.assertEqual(
                 self.universe[element].implied_union_target,
                 "physical_filter" if element == "band" else None,
@@ -291,18 +293,18 @@
         self.assertCountEqual(group.elements, group.names)
         self.assertCountEqual(group.governors, {"instrument"})
 
     def testObservationDimensions(self):
         group = self.universe.conform(["exposure", "detector", "visit"])
         self.assertCountEqual(
             group.names,
-            ("instrument", "detector", "visit", "exposure", "physical_filter", "band"),
+            ("instrument", "detector", "visit", "exposure", "physical_filter", "band", "group", "day_obs"),
         )
         self.assertCountEqual(group.required, ("instrument", "detector", "exposure", "visit"))
-        self.assertCountEqual(group.implied, ("physical_filter", "band"))
+        self.assertCountEqual(group.implied, ("physical_filter", "band", "group", "day_obs"))
         self.assertCountEqual(group.elements - group.names, ("visit_detector_region", "visit_definition"))
         self.assertCountEqual(group.spatial.names, ("observation_regions",))
         self.assertCountEqual(group.temporal.names, ("observation_timespans",))
         self.assertCountEqual(group.governors, {"instrument"})
         self.assertEqual(group.spatial.names, {"observation_regions"})
         self.assertEqual(group.temporal.names, {"observation_timespans"})
         self.assertEqual(next(iter(group.spatial)).governor, self.universe["instrument"])
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_exprParserLex.py` & `lsst_daf_butler-27.0.0rc1/tests/test_exprParserLex.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_exprParserYacc.py` & `lsst_daf_butler-27.0.0rc1/tests/test_exprParserYacc.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_expressions.py` & `lsst_daf_butler-27.0.0rc1/tests/test_expressions.py`

 * *Files 1% similar despite different names*

```diff
@@ -254,22 +254,24 @@
         self.assertEqual(summary.dimensions, {"instrument"})
         self.assertFalse(summary.columns)
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("instrument = 'LSST' AND visit = 1")
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter"})
+        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "day_obs"})
         self.assertFalse(summary.columns)
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("instrument = 'LSST' AND visit = 1 AND skymap = 'x'")
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "skymap"})
+        self.assertEqual(
+            summary.dimensions, {"instrument", "visit", "band", "physical_filter", "skymap", "day_obs"}
+        )
         self.assertFalse(summary.columns)
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
     def test_bind(self):
         """Test for simple expressions with binds."""
         universe = DimensionUniverse()
@@ -288,22 +290,24 @@
         summary = tree.visit(InspectionVisitor(universe, bind))
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("instrument = instr AND visit = visit_id")
         bind = {"instr": "LSST", "visit_id": 1}
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter"})
+        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "day_obs"})
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("instrument = 'LSST' AND visit = 1 AND skymap = skymap_name")
         bind = {"instr": "LSST", "visit_id": 1, "skymap_name": "x"}
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "skymap"})
+        self.assertEqual(
+            summary.dimensions, {"instrument", "visit", "band", "physical_filter", "skymap", "day_obs"}
+        )
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
     def test_in(self):
         """Test for IN expressions."""
         universe = DimensionUniverse()
         parser = ParserYacc()
@@ -323,29 +327,29 @@
         self.assertEqual(summary.dimensions, {"instrument"})
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("visit IN (1,2,3)")
         bind = {}
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter"})
+        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "day_obs"})
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("visit IN (visit1, visit2, visit3)")
         bind = {"visit1": 1, "visit2": 2, "visit3": 3}
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter"})
+        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "day_obs"})
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
         tree = parser.parse("visit IN (visits)")
         bind = {"visits": (1, 2, 3)}
         summary = tree.visit(InspectionVisitor(universe, bind))
-        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter"})
+        self.assertEqual(summary.dimensions, {"instrument", "visit", "band", "physical_filter", "day_obs"})
         self.assertIsNone(summary.dataIdKey)
         self.assertIsNone(summary.dataIdValue)
 
 
 class CheckVisitorTestCase(unittest.TestCase):
     """Tests for CheckVisitor class."""
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_formatter.py` & `lsst_daf_butler-27.0.0rc1/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_location.py` & `lsst_daf_butler-27.0.0rc1/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_logFormatter.py` & `lsst_daf_butler-27.0.0rc1/tests/test_logFormatter.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_logging.py` & `lsst_daf_butler-27.0.0rc1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_matplotlibFormatter.py` & `lsst_daf_butler-27.0.0rc1/tests/test_query_direct_sqlite.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This file is part of daf_butler.
 #
 # Developed for the LSST Data Management System.
 # This product includes software developed by the LSST Project
-# (http://www.lsst.org).
+# (https://www.lsst.org).
 # See the COPYRIGHT file at the top-level directory of this distribution
 # for details of code ownership.
 #
 # This software is dual licensed under the GNU General Public License and also
 # under a 3-clause BSD license. Recipients may choose which of these licenses
 # to use; please see the files gpl-3.0.txt and/or bsd_license.txt,
 # respectively.  If you choose the GPL option then the following text applies
@@ -19,76 +19,47 @@
 #
 # This program is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
-# along with this program.  If not, see <http://www.gnu.org/licenses/>.
+# along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
-"""Tests for MatplotlibFormatter.
+"""Tests for DirectButler._query with SQLite.
 """
 
+from __future__ import annotations
+
 import os
-import tempfile
 import unittest
-from random import Random
 
-try:
-    import matplotlib
+from lsst.daf.butler import Butler, ButlerConfig, StorageClassFactory
+from lsst.daf.butler.datastore import NullDatastore
+from lsst.daf.butler.direct_butler import DirectButler
+from lsst.daf.butler.registry.sql_registry import SqlRegistry
+from lsst.daf.butler.tests.butler_queries import ButlerQueryTests
 
-    matplotlib.use("Agg")
-    from matplotlib import pyplot
-except ImportError:
-    pyplot = None
+TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
-import filecmp
 
-from lsst.daf.butler import Butler, DatasetType
-from lsst.daf.butler.tests.utils import makeTestTempDir, removeTestTempDir
+class DirectButlerSQLiteTests(ButlerQueryTests, unittest.TestCase):
+    """Tests for DirectButler._query with SQLite."""
 
-TESTDIR = os.path.abspath(os.path.dirname(__file__))
+    data_dir = os.path.join(TESTDIR, "data/registry")
 
-
-@unittest.skipIf(pyplot is None, "skipping test because matplotlib import failed")
-class MatplotlibFormatterTestCase(unittest.TestCase):
-    """Test for MatplotlibFormatter."""
-
-    RANDOM_SEED = 10
-
-    def setUp(self):
-        self.root = makeTestTempDir(TESTDIR)
-        Butler.makeRepo(self.root)
-        # Create a random image for testing
-        self.rng = Random(self.RANDOM_SEED)
-
-    def tearDown(self):
-        removeTestTempDir(self.root)
-
-    def testMatplotlibFormatter(self):
-        butler = Butler.from_config(self.root, run="testrun")
-        datasetType = DatasetType("test_plot", [], "Plot", universe=butler.dimensions)
-        butler.registry.registerDatasetType(datasetType)
-        # Does not have to be a random image
-        pyplot.imshow(
-            [
-                self.rng.sample(range(50), 10),
-                self.rng.sample(range(50), 10),
-                self.rng.sample(range(50), 10),
-            ]
+    def make_butler(self, *args: str) -> Butler:
+        config = ButlerConfig()
+        config[".registry.db"] = "sqlite://"
+        registry = SqlRegistry.createFromConfig(config)
+        for arg in args:
+            self.load_data(registry, arg)
+        return DirectButler(
+            config=config,
+            registry=registry,
+            datastore=NullDatastore(None, None),
+            storageClasses=StorageClassFactory(),
         )
-        ref = butler.put(pyplot.gcf(), datasetType)
-        uri = butler.getURI(ref)
-
-        # Following test needs a local file
-        with uri.as_local() as local, tempfile.NamedTemporaryFile(suffix=".png") as file:
-            pyplot.gcf().savefig(file.name)
-            self.assertTrue(filecmp.cmp(local.ospath, file.name, shallow=True))
-        self.assertTrue(butler.exists(ref))
-        with self.assertRaises(ValueError):
-            butler.get(ref)
-        butler.pruneDatasets([ref], unstore=True, purge=True)
-        self.assertFalse(butler.exists(ref))
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_nonempty_mapping.py` & `lsst_daf_butler-27.0.0rc1/tests/test_nonempty_mapping.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_normalFormExpression.py` & `lsst_daf_butler-27.0.0rc1/tests/test_normalFormExpression.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_obscore.py` & `lsst_daf_butler-27.0.0rc1/tests/test_obscore.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,27 +86,31 @@
 
     def initialize_registry(self, registry: SqlRegistry) -> None:
         """Populate Registry with the things that we need for tests."""
         registry.insertDimensionData("instrument", {"name": "DummyCam"})
         registry.insertDimensionData(
             "physical_filter", {"instrument": "DummyCam", "name": "d-r", "band": "r"}
         )
+        registry.insertDimensionData("day_obs", {"instrument": "DummyCam", "id": 20200101})
         for detector in (1, 2, 3, 4):
             registry.insertDimensionData(
                 "detector", {"instrument": "DummyCam", "id": detector, "full_name": f"detector{detector}"}
             )
 
         for exposure in (1, 2, 3, 4):
+            registry.insertDimensionData("group", {"instrument": "DummyCam", "name": f"group{exposure}"})
             registry.insertDimensionData(
                 "exposure",
                 {
                     "instrument": "DummyCam",
                     "id": exposure,
                     "obs_id": f"exposure{exposure}",
                     "physical_filter": "d-r",
+                    "group": f"group{exposure}",
+                    "day_obs": 20200101,
                 },
             )
 
         registry.insertDimensionData("visit_system", {"instrument": "DummyCam", "id": 1, "name": "default"})
 
         for visit in (1, 2, 3, 4, 9):
             visit_start = astropy.time.Time(f"2020-01-01 08:0{visit}:00", scale="tai")
@@ -116,14 +120,15 @@
                 {
                     "instrument": "DummyCam",
                     "id": visit,
                     "name": f"visit{visit}",
                     "physical_filter": "d-r",
                     "datetime_begin": visit_start,
                     "datetime_end": visit_end,
+                    "day_obs": 20200101,
                 },
             )
             registry.insertDimensionData(
                 "visit_system_membership",
                 {"instrument": "DummyCam", "visit": visit, "visit_system": 1},
             )
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_packages.py` & `lsst_daf_butler-27.0.0rc1/tests/test_packages.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_parquet.py` & `lsst_daf_butler-27.0.0rc1/tests/test_parquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,18 +263,45 @@
     table["b"].description = "Description of column b"
 
     # Add some masked columns.
     if include_masked:
         nrow = len(table)
         mask = np.zeros(nrow, dtype=bool)
         mask[1] = True
-        table["m1"] = np.ma.masked_array(data=np.arange(nrow, dtype="i8"), mask=mask)
-        table["m2"] = np.ma.masked_array(data=np.arange(nrow, dtype="f4"), mask=mask)
-        table["mstrcol"] = np.ma.masked_array(data=np.array(["text"] * nrow), mask=mask)
-        table["mbytecol"] = np.ma.masked_array(data=np.array([b"bytes"] * nrow), mask=mask)
+        # We set the masked columns with the underlying sentinel value
+        # to be able test after serialization.
+
+        # Masked 64-bit integer.
+        arr = np.arange(nrow, dtype="i8")
+        arr[mask] = -1
+        table["m_i8"] = np.ma.masked_array(data=arr, mask=mask, fill_value=-1)
+        # Masked 32-bit float.
+        arr = np.arange(nrow, dtype="f4")
+        arr[mask] = np.nan
+        table["m_f4"] = np.ma.masked_array(data=arr, mask=mask, fill_value=np.nan)
+        # Unmasked 32-bit float with NaNs.
+        table["um_f4"] = arr
+        # Masked 64-bit float.
+        arr = np.arange(nrow, dtype="f8")
+        arr[mask] = np.nan
+        table["m_f8"] = np.ma.masked_array(data=arr, mask=mask, fill_value=np.nan)
+        # Unmasked 64-bit float with NaNs.
+        table["um_f8"] = arr
+        # Masked boolean.
+        arr = np.zeros(nrow, dtype=np.bool_)
+        arr[mask] = True
+        table["m_bool"] = np.ma.masked_array(data=arr, mask=mask, fill_value=True)
+        # Masked unsigned 32-bit unsigned int.
+        arr = np.arange(nrow, dtype="u4")
+        arr[mask] = 0
+        table["m_u4"] = np.ma.masked_array(data=arr, mask=mask, fill_value=0)
+        # Masked string.
+        table["m_str"] = np.ma.masked_array(data=np.array(["text"] * nrow), mask=mask, fill_value="")
+        # Masked bytes.
+        table["m_byte"] = np.ma.masked_array(data=np.array([b"bytes"] * nrow), mask=mask, fill_value=b"")
 
     return table
 
 
 def _makeSimpleArrowTable(include_multidim=False, include_masked=False):
     """Make an arrow table for testing.
 
@@ -1015,15 +1042,32 @@
 
         self.assertEqual(table1.meta, table2.meta)
         if not skip_units:
             for name in table1.columns:
                 self.assertEqual(table1[name].unit, table2[name].unit)
                 self.assertEqual(table1[name].description, table2[name].description)
                 self.assertEqual(table1[name].format, table2[name].format)
-        self.assertTrue(np.all(table1 == table2))
+                # We need to check masked/regular columns after filling.
+                has_masked = False
+                if isinstance(table1[name], atable.column.MaskedColumn):
+                    c1 = table1[name].filled()
+                    has_masked = True
+                else:
+                    c1 = np.array(table1[name])
+                if has_masked:
+                    self.assertIsInstance(table2[name], atable.column.MaskedColumn)
+                    c2 = table2[name].filled()
+                else:
+                    self.assertFalse(isinstance(table2[name], atable.column.MaskedColumn))
+                    c2 = np.array(table2[name])
+                np.testing.assert_array_equal(c1, c2)
+                # If we have a masked column then we test the underlying data.
+                if has_masked:
+                    np.testing.assert_array_equal(np.array(c1), np.array(c2))
+                    np.testing.assert_array_equal(table1[name].mask, table2[name].mask)
 
 
 @unittest.skipUnless(atable is not None, "Cannot test InMemoryArrowAstropyDelegate without astropy.")
 class InMemoryArrowAstropyDelegateTestCase(ParquetFormatterArrowAstropyTestCase):
     """Tests for InMemoryDatastore, using ArrowAstropyDelegate."""
 
     configFile = os.path.join(TESTDIR, "config/basic/butler-inmemory.yaml")
@@ -1334,15 +1378,21 @@
 
     def testArrowTable(self):
         tab1 = _makeSimpleArrowTable(include_multidim=True, include_masked=True)
 
         self.butler.put(tab1, self.datasetType, dataId={})
         # Read the whole Table.
         tab2 = self.butler.get(self.datasetType, dataId={})
-        self.assertEqual(tab2, tab1)
+        # We convert to use the numpy testing framework to handle nan
+        # comparisons.
+        self.assertEqual(tab1.schema, tab2.schema)
+        tab1_np = arrow_to_numpy(tab1)
+        tab2_np = arrow_to_numpy(tab2)
+        for col in tab1.column_names:
+            np.testing.assert_array_equal(tab2_np[col], tab1_np[col])
         # Read the columns.
         columns2 = self.butler.get(self.datasetType.componentTypeName("columns"), dataId={})
         self.assertEqual(len(columns2), len(tab1.schema.names))
         for i, name in enumerate(tab1.schema.names):
             self.assertEqual(columns2[i], name)
         # Read the rowcount.
         rowcount = self.butler.get(self.datasetType.componentTypeName("rowcount"), dataId={})
@@ -1575,15 +1625,32 @@
         table2 : `astropy.table.Table`
         """
         self.assertEqual(table1.dtype, table2.dtype)
         for name in table1.columns:
             self.assertEqual(table1[name].unit, table2[name].unit)
             self.assertEqual(table1[name].description, table2[name].description)
             self.assertEqual(table1[name].format, table2[name].format)
-        self.assertTrue(np.all(table1 == table2))
+            # We need to check masked/regular columns after filling.
+            has_masked = False
+            if isinstance(table1[name], atable.column.MaskedColumn):
+                c1 = table1[name].filled()
+                has_masked = True
+            else:
+                c1 = np.array(table1[name])
+            if has_masked:
+                self.assertIsInstance(table2[name], atable.column.MaskedColumn)
+                c2 = table2[name].filled()
+            else:
+                self.assertFalse(isinstance(table2[name], atable.column.MaskedColumn))
+                c2 = np.array(table2[name])
+            np.testing.assert_array_equal(c1, c2)
+            # If we have a masked column then we test the underlying data.
+            if has_masked:
+                np.testing.assert_array_equal(np.array(c1), np.array(c2))
+                np.testing.assert_array_equal(table1[name].mask, table2[name].mask)
 
     def _checkNumpyTableEquality(self, table1, table2):
         """Check if two numpy tables have the same columns/values
 
         Parameters
         ----------
         table1 : `numpy.ndarray`
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_postgresql.py` & `lsst_daf_butler-27.0.0rc1/tests/test_postgresql.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_progress.py` & `lsst_daf_butler-27.0.0rc1/tests/test_progress.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_quantum.py` & `lsst_daf_butler-27.0.0rc1/tests/test_quantum.py`

 * *Files 9% similar despite different names*

```diff
@@ -68,56 +68,65 @@
 
         band = universe["band"]
         bandRecord = band.RecordClass(name="r")
 
         physical_filter = universe["physical_filter"]
         physical_filter_record = physical_filter.RecordClass(name="r", instrument="test", band="r")
 
+        day_obs = universe["day_obs"]
+        day_obs_record = day_obs.RecordClass(instrument="test", id=20250101)
+
         visit_system = universe["visit_system"]
         visit_system_record = visit_system.RecordClass(id=9, instrument="test", name="test_visit_system")
 
         visit = universe["visit"]
         region = Circle()
         # create a synthetic value to mock as a visit hash
         visit_record_42 = visit.RecordClass(
             id=42,
             instrument="test",
             name="test_visit",
             physical_filter="r",
             region=region,
+            day_obs=20250101,
         )
         visit_record_43 = visit.RecordClass(
             id=43,
             instrument="test",
             name="test_visit",
             physical_filter="r",
             region=region,
+            day_obs=20250101,
         )
 
         records42 = {
             instrument: instrumentRecord,
             band: bandRecord,
             physical_filter: physical_filter_record,
             visit_system: visit_system_record,
             visit: visit_record_42,
+            day_obs: day_obs_record,
         }
 
         records43 = {
             instrument: instrumentRecord,
             band: bandRecord,
             physical_filter: physical_filter_record,
             visit_system: visit_system_record,
             visit: visit_record_43,
+            day_obs: day_obs_record,
         }
 
         dataId42 = DataCoordinate.standardize(
-            dict(instrument="test", visit=42), universe=universe  # type: ignore
+            dict(instrument="test", visit=42),
+            universe=universe,  # type: ignore
         )
         dataId43 = DataCoordinate.standardize(
-            dict(instrument="test", visit=43), universe=universe  # type: ignore
+            dict(instrument="test", visit=43),
+            universe=universe,  # type: ignore
         )
 
         if addRecords:
             dataId42 = dataId42.expanded(records42)  # type: ignore
             dataId43 = dataId43.expanded(records43)  # type: ignore
 
         datasetTypeInit = DatasetType(
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_quantumBackedButler.py` & `lsst_daf_butler-27.0.0rc1/tests/test_quantumBackedButler.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_query_relations.py` & `lsst_daf_butler-27.0.0rc1/tests/test_query_relations.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,20 +27,20 @@
 
 import difflib
 import os
 import os.path
 import re
 import unittest
 
-from lsst.daf.butler import (
+from lsst.daf.butler.registry import MissingSpatialOverlapError, RegistryConfig, _RegistryFactory
+from lsst.daf.butler.registry.queries import (
     DataCoordinateQueryResults,
+    DatasetQueryResults,
     DimensionRecordQueryResults,
-    SingleTypeDatasetQueryResults,
 )
-from lsst.daf.butler.registry import MissingSpatialOverlapError, RegistryConfig, _RegistryFactory
 from lsst.daf.butler.transfers import YamlRepoImportBackend
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
 
 class TestQueryRelationsTests(unittest.TestCase):
     """Tests for registry queries that check that the generated relation tree
@@ -92,21 +92,22 @@
             instrument=cls.instrument,
             skymap=cls.skymap,
             visit=cls.visit,
             tract=cls.tract,
             detector=cls.detector,
             patch=cls.patch,
         )
+        cls.day_obs = cls.data_id["day_obs"]
         cls.band = cls.data_id["band"]
         cls.physical_filter = cls.data_id["physical_filter"]
 
     def assert_relation_str(
         self,
         expected: str,
-        *results: DataCoordinateQueryResults | DimensionRecordQueryResults | SingleTypeDatasetQueryResults,
+        *results: DataCoordinateQueryResults | DimensionRecordQueryResults | DatasetQueryResults,
     ) -> None:
         """Assert that checks that one or more registry
         queries have relation trees that match the given string.
 
         Parameters
         ----------
         expected : `str`
@@ -151,14 +152,15 @@
                         select(
                             Π[band, patch, patch.region, skymap, tract, visit_detector_region.region](
                                 σ[
                                     instrument={self.instrument!r}
                                     and detector={self.detector!r}
                                     and visit={self.visit!r}
                                     and band={self.band!r}
+                                    and day_obs={self.day_obs!r}
                                     and physical_filter={self.physical_filter!r}
                                 ](
                                     patch_htm7_overlap
                                     ⋈ visit_detector_region_htm7_overlap
                                     ⋈ physical_filter
                                     ⋈ patch
                                     ⋈ visit
@@ -176,14 +178,15 @@
             self.registry.queryDataIds(
                 ["patch", "band"],
                 where=(
                     f"instrument={self.instrument!r} "
                     f"and detector={self.detector!r} "
                     f"and visit={self.visit!r}"
                     f"and band={self.band!r} "
+                    f"and day_obs={self.day_obs!r}"
                     f"and physical_filter={self.physical_filter!r} "
                 ),
             ),
         )
         # Constrain the special common skypix dimension from a regular
         # dimension.  This does not need any post-query filtering.
         self.assert_relation_str(
@@ -197,14 +200,15 @@
             select(
                 Π[htm7](
                     σ[
                         instrument={self.instrument!r}
                         and detector={self.detector!r}
                         and visit={self.visit!r}
                         and band={self.band!r}
+                        and day_obs={self.day_obs!r}
                         and physical_filter={self.physical_filter!r}
                     ](
                         visit_detector_region_htm7_overlap
                         ⋈ physical_filter
                         ⋈ visit
                     )
                 )
@@ -220,14 +224,15 @@
             self.registry.queryDataIds(
                 ["htm7"],
                 where=(
                     f"instrument={self.instrument!r} "
                     f"and detector={self.detector!r} "
                     f"and visit={self.visit!r}"
                     f"and band={self.band!r} "
+                    f"and day_obs={self.day_obs!r}"
                     f"and physical_filter={self.physical_filter!r} "
                 ),
             ),
         )
         # We can't constrain any other skypix system spatially, because we
         # don't have overlap rows for those in the database.  But in the future
         # we might be able to fake it with an iteration-engine spatial join, or
@@ -301,14 +306,15 @@
                     →[iteration](
                         select(
                             Π[detector, instrument, visit_detector_region.region](
                                 σ[
                                     instrument={self.instrument!r}
                                     and visit={self.visit!r}
                                     and band={self.band!r}
+                                    and day_obs={self.day_obs!r}
                                     and physical_filter={self.physical_filter!r}
                                     and htm7={self.htm7!r}
                                 ](
                                     visit_detector_region_htm7_overlap
                                     ⋈ physical_filter
                                     ⋈ visit
                                     ⋈ visit_detector_region
@@ -333,14 +339,15 @@
             select(
                 Π[detector, instrument](
                     σ[
                         htm7={self.htm7!r}
                         and instrument={self.instrument!r}
                         and visit={self.visit!r}
                         and band={self.band!r}
+                        and day_obs={self.day_obs!r}
                         and physical_filter={self.physical_filter!r}
                     ](
                         visit_detector_region_htm7_overlap
                         ⋈ physical_filter
                         ⋈ visit
                     )
                 )
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_remote_butler.py` & `lsst_daf_butler-27.0.0rc1/tests/test_remote_butler.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>.
 
 import os
 import unittest
 from unittest.mock import patch
 
 from lsst.daf.butler import Butler, Registry
+from lsst.daf.butler._exceptions import UnknownButlerUserError
 from lsst.daf.butler.datastores.file_datastore.retrieve_artifacts import (
     determine_destination_for_retrieved_artifact,
 )
 from lsst.daf.butler.registry.tests import RegistryTests
 from lsst.resources import ResourcePath
 from pydantic import ValidationError
 
@@ -62,22 +63,48 @@
             Butler({"cls": "lsst.daf.butler.remote_butler.RemoteButler", "remote_butler": {"url": "!"}})
 
 
 @unittest.skipIf(RemoteButler is None, "httpx is not installed")
 class RemoteButlerErrorHandlingTests(unittest.TestCase):
     """Test RemoteButler error handling."""
 
-    def test_internal_server_error(self):
-        butler = RemoteButlerFactory.create_factory_for_url(
+    def setUp(self):
+        self.butler = RemoteButlerFactory.create_factory_for_url(
             "https://doesntmatter"
         ).create_butler_for_access_token("dontcare")
-        with patch.object(butler._client, "request") as mock:
-            mock.side_effect = httpx.HTTPError("unhandled error")
-            with self.assertRaises(ButlerServerError):
-                butler.get_dataset_type("int")
+        self.mock = self.enterContext(patch.object(self.butler._connection._client, "request"))
+
+    def _mock_error_response(self, content: str) -> None:
+        self.mock.return_value = httpx.Response(
+            status_code=422, content=content, request=httpx.Request("GET", "/")
+        )
+
+    def test_internal_server_error(self):
+        self.mock.side_effect = httpx.HTTPError("unhandled error")
+        with self.assertRaises(ButlerServerError):
+            self.butler.get_dataset_type("int")
+
+    def test_unknown_error_type(self):
+        self.mock.return_value = httpx.Response(
+            status_code=422, json={"error_type": "not a known error type", "detail": "an error happened"}
+        )
+        with self.assertRaises(UnknownButlerUserError):
+            self.butler.get_dataset_type("int")
+
+    def test_non_json_error(self):
+        # Server returns a non-JSON body with an error
+        self._mock_error_response("notvalidjson")
+        with self.assertRaises(ButlerServerError):
+            self.butler.get_dataset_type("int")
+
+    def test_malformed_error(self):
+        # Server returns JSON, but not in the expected format.
+        self._mock_error_response("{}")
+        with self.assertRaises(ButlerServerError):
+            self.butler.get_dataset_type("int")
 
 
 class RemoteButlerMiscTests(unittest.TestCase):
     """Test miscellaneous RemoteButler functionality."""
 
     def test_retrieve_artifacts_security(self):
         # Make sure that the function used to determine output file paths for
@@ -102,14 +129,16 @@
         )
 
 
 @unittest.skipIf(create_test_server is None, "Server dependencies not installed.")
 class RemoteButlerRegistryTests(RegistryTests, unittest.TestCase):
     """Tests for RemoteButler's `Registry` shim."""
 
+    supportsCollectionRegex = False
+
     def setUp(self):
         self.server_instance = self.enterContext(create_test_server(TESTDIR))
 
     @classmethod
     def getDataDir(cls) -> str:
         return os.path.join(TESTDIR, "data", "registry")
 
@@ -128,14 +157,24 @@
         pass
 
     def testOpaque(self):
         # This tests an internal implementation detail that isn't exposed to
         # the client side.
         pass
 
+    def testCollectionChainPrependConcurrency(self):
+        # This tests an implementation detail that requires access to the
+        # collection manager object.
+        pass
+
+    def testCollectionChainReplaceConcurrency(self):
+        # This tests an implementation detail that requires access to the
+        # collection manager object.
+        pass
+
     def testAttributeManager(self):
         # Tests a non-public API that isn't relevant on the client side.
         pass
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_server.py` & `lsst_daf_butler-27.0.0rc1/tests/test_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,29 +30,29 @@
 import uuid
 
 from lsst.daf.butler.tests.dict_convertible_model import DictConvertibleModel
 
 try:
     # Failing to import any of these should disable the tests.
     import safir.dependencies.logger
-    from fastapi import HTTPException
     from fastapi.testclient import TestClient
     from lsst.daf.butler.remote_butler import RemoteButler
     from lsst.daf.butler.remote_butler._authentication import _EXPLICIT_BUTLER_ACCESS_TOKEN_ENVIRONMENT_KEY
     from lsst.daf.butler.remote_butler.server import create_app
     from lsst.daf.butler.remote_butler.server._dependencies import butler_factory_dependency
-    from lsst.daf.butler.tests.server import TEST_REPOSITORY_NAME, create_test_server
+    from lsst.daf.butler.tests.server import TEST_REPOSITORY_NAME, UnhandledServerError, create_test_server
 except ImportError:
     create_test_server = None
 
 from unittest.mock import NonCallableMock, patch
 
 from lsst.daf.butler import (
     Butler,
     DataCoordinate,
+    DatasetNotFoundError,
     DatasetRef,
     LabeledButlerFactory,
     MissingDatasetTypeError,
     NoDefaultCollectionError,
     StorageClassFactory,
 )
 from lsst.daf.butler.datastore import DatasetRefURIs
@@ -91,14 +91,20 @@
         # these imports do not point at real files.
         direct_butler = server_instance.direct_butler
         DatastoreMock.apply(direct_butler)
         direct_butler.import_(filename=os.path.join(TESTDIR, "data", "registry", "base.yaml"))
         direct_butler.import_(filename=os.path.join(TESTDIR, "data", "registry", "datasets.yaml"))
 
     def test_health_check(self):
+        try:
+            import importlib.metadata
+
+            importlib.metadata.metadata("lsst.daf.butler")
+        except ModuleNotFoundError:
+            raise self.skipTest("Standard python package metadata not available. Butler not pip installed.")
         response = self.client.get("/")
         self.assertEqual(response.status_code, 200)
         self.assertEqual(response.json()["name"], "butler")
 
     def test_dimension_universe(self):
         universe = self.butler.dimensions
         self.assertEqual(universe.namespace, "daf_butler")
@@ -194,16 +200,16 @@
                     collections=["collection1", "collection2"],
                     run="collection2",
                 )
             butler_factory = LabeledButlerFactory({"server": server_url})
             factory_created_butler = butler_factory.create_butler(label="server", access_token="token")
         self.assertIsInstance(butler, RemoteButler)
         self.assertIsInstance(factory_created_butler, RemoteButler)
-        self.assertEqual(butler._server_url, server_url)
-        self.assertEqual(factory_created_butler._server_url, server_url)
+        self.assertEqual(butler._connection.server_url, server_url)
+        self.assertEqual(factory_created_butler._connection.server_url, server_url)
 
         self.assertEqual(butler.collections, ("collection1", "collection2"))
         self.assertEqual(butler.run, "collection2")
 
     def test_get(self):
         dataset_type = "test_metric_comp"
         data_id = {"instrument": "DummyCamComp", "visit": 423}
@@ -226,15 +232,15 @@
         coordinate = DataCoordinate.make_empty(self.butler.dimensions)
         kwarg_data_coordinate_metric = self.butler.get(
             dataset_type, dataId=coordinate, collections=collections, instrument="DummyCamComp", visit=423
         )
         self.assertEqual(metric, kwarg_data_coordinate_metric)
         # Test get() of a non-existent DataId.
         invalid_data_id = {"instrument": "NotAValidlInstrument", "visit": 423}
-        with self.assertRaises(FileNotFoundError):
+        with self.assertRaises(DatasetNotFoundError):
             self.butler_without_error_propagation.get(
                 dataset_type, dataId=invalid_data_id, collections=collections
             )
 
         # Test get() by DataId with default collections.
         butler_with_default_collection = self.butler._clone(collections="ingest/run")
         default_collection_metric = butler_with_default_collection.get(dataset_type, dataId=data_id)
@@ -242,15 +248,15 @@
 
         # Test get() by DataId with no collections specified.
         with self.assertRaises(NoDefaultCollectionError):
             self.butler_without_error_propagation.get(dataset_type, dataId=data_id)
 
         # Test looking up a non-existent ref
         invalid_ref = ref.replace(id=uuid.uuid4())
-        with self.assertRaises(FileNotFoundError):
+        with self.assertRaises(DatasetNotFoundError):
             self.butler_without_error_propagation.get(invalid_ref)
 
         with self.assertRaises(RuntimeError):
             self.butler_without_error_propagation.get(self.dataset_with_corrupted_data)
 
         # Test storage class override
         new_sc = self.storageClassFactory.getStorageClass("MetricsConversion")
@@ -332,17 +338,17 @@
         check_uris(componentUris)
 
     def test_auth_check(self):
         # This is checking that the unit-test middleware for validating the
         # authentication headers is working.  It doesn't test actual server
         # functionality -- in a real deployment, the authentication headers are
         # handled by GafaelfawrIngress, not our app.
-        with self.assertRaises(HTTPException) as cm:
+        with self.assertRaises(UnhandledServerError) as cm:
             self.client.get("/v1/dataset_type/int")
-        self.assertEqual(cm.exception.status_code, 401)
+        self.assertEqual(cm.exception.__cause__.status_code, 401)
 
     def test_exception_logging(self):
         app = create_app()
 
         def raise_error():
             raise RuntimeError("An unhandled error")
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_simpleButler.py` & `lsst_daf_butler-27.0.0rc1/tests/test_simpleButler.py`

 * *Files 14% similar despite different names*

```diff
@@ -50,53 +50,38 @@
     DatasetType,
     StorageClass,
     Timespan,
 )
 from lsst.daf.butler.datastore.file_templates import FileTemplate
 from lsst.daf.butler.registry import RegistryConfig, RegistryDefaults, _RegistryFactory
 from lsst.daf.butler.tests import DatastoreMock
-from lsst.daf.butler.tests.utils import makeTestTempDir, removeTestTempDir
+from lsst.daf.butler.tests.utils import TestCaseMixin, makeTestTempDir, removeTestTempDir
+
+try:
+    from lsst.daf.butler.tests.server import create_test_server
+except ImportError:
+    create_test_server = None
 
 TESTDIR = os.path.abspath(os.path.dirname(__file__))
 
 
-class SimpleButlerTestCase(unittest.TestCase):
+class SimpleButlerTests(TestCaseMixin):
     """Tests for butler (including import/export functionality) that should not
     depend on the Registry Database backend or Datastore implementation, and
     can instead utilize an in-memory SQLite Registry and a mocked Datastore.
     """
 
-    datasetsManager = (
-        "lsst.daf.butler.registry.datasets.byDimensions.ByDimensionsDatasetRecordStorageManagerUUID"
-    )
     datasetsImportFile = "datasets.yaml"
 
-    def setUp(self):
-        self.root = makeTestTempDir(TESTDIR)
-
-    def tearDown(self):
-        removeTestTempDir(self.root)
-
-    def makeButler(self, **kwargs: Any) -> Butler:
-        """Return new Butler instance on each call."""
-        config = ButlerConfig()
-
-        # make separate temporary directory for registry of this instance
-        tmpdir = tempfile.mkdtemp(dir=self.root)
-        config["registry", "db"] = f"sqlite:///{tmpdir}/gen3.sqlite3"
-        config["registry", "managers", "datasets"] = self.datasetsManager
-        config["root"] = self.root
+    supportsCollectionRegex: bool = True
+    """True if the registry class being tested supports regex searches for
+    collections."""
 
-        # have to make a registry first
-        registryConfig = RegistryConfig(config.get("registry"))
-        _RegistryFactory(registryConfig).create_from_config()
-
-        butler = Butler.from_config(config, **kwargs)
-        DatastoreMock.apply(butler)
-        return butler
+    def makeButler(self, writeable: bool = False) -> Butler:
+        raise NotImplementedError()
 
     def comparableRef(self, ref: DatasetRef) -> DatasetRef:
         """Return a DatasetRef that can be compared to a DatasetRef from
         other repository.
 
         For repositories that do not support round-trip of ID values this
         method returns unresolved DatasetRef, for round-trip-safe repos it
@@ -368,53 +353,95 @@
         butler.import_(filename=os.path.join(TESTDIR, "data", "registry", self.datasetsImportFile))
         # Certify some biases into a CALIBRATION collection.
         registry = butler.registry
         registry.registerCollection("calibs", CollectionType.CALIBRATION)
         t1 = astropy.time.Time("2020-01-01T01:00:00", format="isot", scale="tai")
         t2 = astropy.time.Time("2020-01-01T02:00:00", format="isot", scale="tai")
         t3 = astropy.time.Time("2020-01-01T03:00:00", format="isot", scale="tai")
+        bias1a = registry.findDataset("bias", instrument="Cam1", detector=1, collections="imported_g")
         bias2a = registry.findDataset("bias", instrument="Cam1", detector=2, collections="imported_g")
         bias3a = registry.findDataset("bias", instrument="Cam1", detector=3, collections="imported_g")
         bias2b = registry.findDataset("bias", instrument="Cam1", detector=2, collections="imported_r")
         bias3b = registry.findDataset("bias", instrument="Cam1", detector=3, collections="imported_r")
+        registry.certify("calibs", [bias1a], Timespan(t1, t2))
         registry.certify("calibs", [bias2a, bias3a], Timespan(t1, t2))
         registry.certify("calibs", [bias2b], Timespan(t2, None))
         registry.certify("calibs", [bias3b], Timespan(t2, t3))
         # Insert some exposure dimension data.
         registry.insertDimensionData(
+            "group",
+            {"instrument": "Cam1", "group": "three"},
+            {"instrument": "Cam1", "group": "four"},
+        )
+        registry.insertDimensionData(
+            "day_obs",
+            {"instrument": "Cam1", "id": 20211114},
+        )
+        # Choose timespans for exposures within the above calibration ranges
+        # but make sure they are not identical to the full range.
+        exp_time = astropy.time.TimeDelta(15.0, format="sec", scale="tai")
+        span_delta = t2 - t1
+        exp3_begin = t1 + (span_delta / 2.0)
+        exp3_end = exp3_begin + exp_time
+        span_delta = t3 - t2
+        exp4_begin = t2 + (span_delta / 2.0)
+        exp4_end = exp4_begin + exp_time
+        registry.insertDimensionData(
             "exposure",
             {
                 "instrument": "Cam1",
                 "id": 3,
                 "obs_id": "three",
-                "timespan": Timespan(t1, t2),
+                "timespan": Timespan(exp3_begin, exp3_end),
                 "physical_filter": "Cam1-G",
-                "day_obs": 20201114,
+                "group": "three",
+                "day_obs": 20211114,
                 "seq_num": 55,
             },
             {
                 "instrument": "Cam1",
                 "id": 4,
                 "obs_id": "four",
-                "timespan": Timespan(t2, t3),
+                "timespan": Timespan(exp4_begin, exp4_end),
                 "physical_filter": "Cam1-G",
+                "group": "four",
                 "day_obs": 20211114,
                 "seq_num": 42,
             },
         )
         # Get some biases from raw-like data IDs.
         bias2a_id, _ = butler.get(
             "bias", {"instrument": "Cam1", "exposure": 3, "detector": 2}, collections="calibs"
         )
         self.assertEqual(bias2a_id, bias2a.id)
         bias3b_id, _ = butler.get(
             "bias", {"instrument": "Cam1", "exposure": 4, "detector": 3}, collections="calibs"
         )
         self.assertEqual(bias3b_id, bias3b.id)
 
+        # Use explicit timespan and no exposure record.
+        bias3b_id, _ = butler.get(
+            "bias",
+            {"instrument": "Cam1", "detector": 3},
+            collections="calibs",
+            timespan=Timespan(exp4_begin, exp4_end),
+        )
+        self.assertEqual(bias3b_id, bias3b.id)
+
+        # No timespan at all.
+        # Only one matching dataset in calibs collection so this works with
+        # a defaulted timespan.
+        bias1a_id, _ = butler.get("bias", {"instrument": "Cam1", "detector": 1}, collections="calibs")
+        self.assertEqual(bias1a_id, bias1a.id)
+
+        # Multiple datasets match in calibs collection with infinite timespan
+        # so this fails.
+        with self.assertRaises(LookupError):
+            bias3b_id, _ = butler.get("bias", {"instrument": "Cam1", "detector": 3}, collections="calibs")
+
         # Get using the kwarg form
         bias3b_id, _ = butler.get("bias", instrument="Cam1", exposure=4, detector=3, collections="calibs")
         self.assertEqual(bias3b_id, bias3b.id)
 
         # Do it again but using the record information
         bias2a_id, _ = butler.get(
             "bias",
@@ -632,15 +659,15 @@
         self.assertIn(butler.dimensions["visit_system"], records)
 
     def testJsonDimensionRecordsAndHtmlRepresentation(self):
         # Dimension Records
         butler = self.makeButler(writeable=True)
         butler.import_(filename=os.path.join(TESTDIR, "data", "registry", "hsc-rc2-subset.yaml"))
 
-        for dimension in ("detector", "visit", "exposure"):
+        for dimension in ("detector", "visit", "exposure", "day_obs", "group"):
             records = butler.registry.queryDimensionRecords(dimension, instrument="HSC")
             for r in records:
                 for minimal in (True, False):
                     json_str = r.to_json(minimal=minimal)
                     r_json = type(r).from_json(json_str, registry=butler.registry)
                     self.assertEqual(r_json, r)
                     # check with direct method
@@ -651,40 +678,63 @@
                     self.assertEqual(r_json.toDict(), r.toDict())
 
                     # check the html representation of records
                     r_html = r._repr_html_()
                     self.assertTrue(isinstance(r_html, str))
                     self.assertIn(dimension, r_html)
 
+    def test_dimension_records_import(self):
+        # Dimension Records
+        butler = self.makeButler(writeable=True)
+        butler.import_(filename=os.path.join(TESTDIR, "data", "registry", "hsc-rc2-subset-v0.yaml"))
+
+        # Count records and assume this means it worked.
+        dimensions = (
+            ("day_obs", 15),
+            ("group", 1),
+            ("exposure", 1),
+            ("visit", 160),
+            ("detector", 111),
+            ("visit_system_membership", 160),
+        )
+        for dimension, count in dimensions:
+            records = list(butler.registry.queryDimensionRecords(dimension, instrument="HSC"))
+            self.assertEqual(len(records), count)
+
     def testWildcardQueries(self):
         """Test that different collection type queries work."""
         # Import data to play with.
         butler = self.makeButler(writeable=True)
         butler.import_(filename=os.path.join(TESTDIR, "data", "registry", "base.yaml"))
 
         # Create some collections
         created = {"collection", "u/user/test", "coll3"}
         for collection in created:
             butler.registry.registerCollection(collection, type=CollectionType.RUN)
 
         collections = butler.registry.queryCollections()
         self.assertEqual(set(collections), created)
 
-        expressions = (
+        expressions = [
             ("collection", {"collection"}),
             (..., created),
             ("*", created),
             (("collection", "*"), created),
             ("u/*", {"u/user/test"}),
-            (re.compile("u.*"), {"u/user/test"}),
-            (re.compile(".*oll.*"), {"collection", "coll3"}),
             ("*oll*", {"collection", "coll3"}),
-            ((re.compile(r".*\d$"), "u/user/test"), {"coll3", "u/user/test"}),
             ("*[0-9]", {"coll3"}),
-        )
+        ]
+        if self.supportsCollectionRegex:
+            expressions.extend(
+                [
+                    (re.compile("u.*"), {"u/user/test"}),
+                    (re.compile(".*oll.*"), {"collection", "coll3"}),
+                    ((re.compile(r".*\d$"), "u/user/test"), {"coll3", "u/user/test"}),
+                ]
+            )
         for expression, expected in expressions:
             result = butler.registry.queryCollections(expression)
             self.assertEqual(set(result), expected)
 
     def test_skypix_templates(self):
         """Test that skypix templates can work."""
         # Dimension Records
@@ -703,9 +753,85 @@
 
         tmplstr = "{run}/{datasetType}/{visit.name}_{skypix}_{htm7}_{skypix.id}_{htm7.id}"
         file_template = FileTemplate(tmplstr)
         path = file_template.format(ref)
         self.assertEqual(path, "test/warp/HSCA02713600_12345_12345_12345_12345")
 
 
+class DirectSimpleButlerTestCase(SimpleButlerTests, unittest.TestCase):
+    """Run tests against DirectButler implementation."""
+
+    datasetsManager = (
+        "lsst.daf.butler.registry.datasets.byDimensions.ByDimensionsDatasetRecordStorageManagerUUID"
+    )
+
+    collectionsManager = "lsst.daf.butler.registry.collections.synthIntKey.SynthIntKeyCollectionManager"
+
+    def setUp(self):
+        self.root = makeTestTempDir(TESTDIR)
+
+    def tearDown(self):
+        removeTestTempDir(self.root)
+
+    def makeButler(self, writeable: bool = False) -> Butler:
+        config = ButlerConfig()
+
+        # make separate temporary directory for registry of this instance
+        tmpdir = tempfile.mkdtemp(dir=self.root)
+        config["registry", "db"] = f"sqlite:///{tmpdir}/gen3.sqlite3"
+        config["registry", "managers", "datasets"] = self.datasetsManager
+        config["registry", "managers", "collections"] = self.collectionsManager
+        config["root"] = self.root
+
+        # have to make a registry first
+        registryConfig = RegistryConfig(config.get("registry"))
+        _RegistryFactory(registryConfig).create_from_config()
+
+        butler = Butler.from_config(config, writeable=writeable)
+        DatastoreMock.apply(butler)
+        return butler
+
+
+class NameKeyCollectionManagerDirectSimpleButlerTestCase(DirectSimpleButlerTestCase, unittest.TestCase):
+    """Run tests against DirectButler implementation using the
+    NameKeyCollectionsManager.
+    """
+
+    collectionsManager = "lsst.daf.butler.registry.collections.nameKey.NameKeyCollectionManager"
+
+
+@unittest.skipIf(create_test_server is None, "Server dependencies not installed.")
+class RemoteSimpleButlerTestCase(SimpleButlerTests, unittest.TestCase):
+    """Run tests against Butler client/server."""
+
+    supportsCollectionRegex = False
+
+    def makeButler(self, writeable: bool = False) -> Butler:
+        server_instance = self.enterContext(create_test_server(TESTDIR))
+        butler = server_instance.hybrid_butler
+        DatastoreMock.apply(butler)
+        # Because RemoteButler doesn't have a Datastore object, we have to
+        # duplicate some of the functionality from DatastoreMock separately.
+        butler._remote_butler._get_dataset_as_python_object = _mock_get_dataset_as_python_object
+        return butler
+
+    def testRegistryDefaults(self):
+        # Registry defaults are not yet fully implemented in RemoteButler.
+        pass
+
+    def testJson(self):
+        # Needs registry defaults functionality that's not yet implemented in
+        # RemoteButler.
+        pass
+
+
+def _mock_get_dataset_as_python_object(
+    ref: DatasetRef,
+    model: Any,
+    parameters: dict[str, Any] | None,
+) -> Any:
+    """Mimic the functionality of DatastoreMock's get() mock."""
+    return (ref.id, parameters)
+
+
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_sqlite.py` & `lsst_daf_butler-27.0.0rc1/tests/test_sqlite.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_storageClass.py` & `lsst_daf_butler-27.0.0rc1/tests/test_storageClass.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_templates.py` & `lsst_daf_butler-27.0.0rc1/tests/test_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,20 @@
             StorageClass(storageClassName),
             parentStorageClass=parentStorageClass,
         )
         return DatasetRef(datasetType, dataId, id=REFUUID, run=run, conform=conform)
 
     def setUp(self):
         self.universe = DimensionUniverse()
-        self.dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "Most Amazing U Filter Ever"}
+        self.dataId = {
+            "instrument": "dummy",
+            "visit": 52,
+            "physical_filter": "Most Amazing U Filter Ever",
+            "day_obs": 20200101,
+        }
 
     def assertTemplate(self, template, answer, ref):
         fileTmpl = FileTemplate(template)
         path = fileTmpl.format(ref)
         self.assertEqual(path, answer)
 
     def testBasic(self):
@@ -136,15 +141,15 @@
         self.assertTemplate(
             tmplstr,
             "run/2/calexp/00052/Most_Amazing_U_Filter_Ever-trail-run_2",
             self.makeDatasetRef("calexp", run="run/2"),
         )
 
         # Check that "." are replaced in the file basename, but not directory.
-        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "g.10"}
+        dataId = {"instrument": "dummy", "visit": 52, "physical_filter": "g.10", "day_obs": 20250101}
         self.assertTemplate(
             tmplstr,
             "run.2/calexp/00052/g_10-trail-run_2",
             self.makeDatasetRef("calexp", run="run.2", dataId=dataId),
         )
 
         with self.assertRaises(FileTemplateValidationError):
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_testRepo.py` & `lsst_daf_butler-27.0.0rc1/tests/test_testRepo.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_thread_utils.py` & `lsst_daf_butler-27.0.0rc1/tests/test_thread_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_time_utils.py` & `lsst_daf_butler-27.0.0rc1/tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_timespan.py` & `lsst_daf_butler-27.0.0rc1/tests/test_timespan.py`

 * *Files 10% similar despite different names*

```diff
@@ -35,14 +35,15 @@
 # As of astropy 4.2, the erfa interface is shipped independently and
 # ErfaWarning is no longer an AstropyWarning
 try:
     import erfa
 except ImportError:
     erfa = None
 
+import pydantic
 from lsst.daf.butler import Timespan
 from lsst.daf.butler.time_utils import TimeConverter
 
 
 class TimespanTestCase(unittest.TestCase):
     """Tests for the `Timespan` class.
 
@@ -249,19 +250,46 @@
         # unittest can't test for no warnings so we run the test and
         # trigger our own warning and count all the warnings
         with self.assertWarns(Warning) as cm:
             self.assertEqual(ts1, ts2)
             warnings.warn("deliberate", stacklevel=1)
         self.assertEqual(str(cm.warning), "deliberate")
 
-    def testJson(self):
-        ts1 = Timespan(
+    def test_serialization(self):
+        ts = Timespan(
             begin=astropy.time.Time("2013-06-17 13:34:45.775000", scale="tai", format="iso"),
             end=astropy.time.Time("2013-06-17 13:35:17.947000", scale="tai", format="iso"),
         )
-        json_str = ts1.to_json()
-        ts_json = Timespan.from_json(json_str)
-        self.assertEqual(ts_json, ts1)
+        adapter = pydantic.TypeAdapter(Timespan)
+        self.assertIn("TAI", adapter.json_schema()["description"])
+        json_roundtripped = adapter.validate_json(adapter.dump_json(ts))
+        self.assertIsInstance(json_roundtripped, Timespan)
+        self.assertEqual(json_roundtripped, ts)
+        python_roundtripped = adapter.validate_python(adapter.dump_python(ts))
+        self.assertIsInstance(json_roundtripped, Timespan)
+        self.assertEqual(python_roundtripped, ts)
+        with self.assertRaises(ValueError):
+            adapter.validate_python(12)
+        with self.assertRaises(ValueError):
+            adapter.validate_json({})
+
+    def test_day_obs(self):
+        data = (
+            ((20240201, 0), ("2024-02-01T00:00:00.0", "2024-02-02T00:00:00.0")),
+            ((19801011, 3600), ("1980-10-11T01:00:00.0", "1980-10-12T01:00:00.0")),
+            ((20481231, -7200), ("2048-12-30T22:00:00.0", "2048-12-31T22:00:00.0")),
+            ((20481231, 7200), ("2048-12-31T02:00:00.0", "2049-01-01T02:00:00.0")),
+        )
+        for input, output in data:
+            ts1 = Timespan.from_day_obs(input[0], input[1])
+            ts2 = Timespan(
+                begin=astropy.time.Time(output[0], scale="tai", format="isot"),
+                end=astropy.time.Time(output[1], scale="tai", format="isot"),
+            )
+            self.assertEqual(ts1, ts2)
+
+            with self.assertRaises(ValueError):
+                Timespan.from_day_obs(19690101)
 
 
 if __name__ == "__main__":
     unittest.main()
```

### Comparing `lsst-daf-butler-26.2024.900/tests/test_utils.py` & `lsst_daf_butler-27.0.0rc1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `lsst-daf-butler-26.2024.900/tests/test_versioning.py` & `lsst_daf_butler-27.0.0rc1/tests/test_versioning.py`

 * *Files identical despite different names*

