# Comparing `tmp/galaxy-tool-util-24.0.0.tar.gz` & `tmp/galaxy_tool_util-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-tool-util-24.0.0.tar", last modified: Wed Apr  3 02:45:02 2024, max compression
+gzip compressed data, was "galaxy_tool_util-24.0.1.tar", last modified: Thu May  2 13:48:07 2024, max compression
```

## Comparing `galaxy-tool-util-24.0.0.tar` & `galaxy_tool_util-24.0.1.tar`

### file list

```diff
@@ -1,184 +1,184 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    22206 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.407017 galaxy-tool-util-24.0.0/galaxy/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/source.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/client/staging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/cwltool_deps.py
--rw-r--r--   0 runner    (1001) docker     (127)    45945 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/representation.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runnable.py
--rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runtime_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    25745 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/data/
--rw-r--r--   0 runner    (1001) docker     (127)    59526 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.411017 galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.415017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/
--rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19566 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_exts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_compat.py
--rw-r--r--   0 runner    (1001) docker     (127)    27451 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.415017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/explicit.py
--rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/mulled.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18185 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/containers.py
--rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/docker_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dockerfiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/installable.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.419017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/get_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/invfile.lua
--rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_channel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_tool.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    15814 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
--rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/requirements.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.419017 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/conda.py
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/galaxy_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/homebrew.py
--rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/lmod.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/resolver_mixins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/singularity_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/deps/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/edam_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/fetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/lint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.423017 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/citations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/help.py
--rw-r--r--   0 runner    (1001) docker     (127)    52233 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)    22415 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xml_order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xsd.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/loader_directory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.423017 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/dockstore.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/locations/http.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.423017 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    53080 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/biotools_mappings.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
--rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/ontology_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/output_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_collection_def.py
--rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/stdio.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    54802 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/parser/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/provided_metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    65232 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/examples.py.sample
--rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/integrated_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/panel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/edam.py
--rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/sources.py
--rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/static.py
--rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/watcher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.427017 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/interactor.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.431017 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/
--rw-r--r--   0 runner    (1001) docker     (127)    21654 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.431017 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/archive.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/hdf5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/size.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/tabular.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)    75994 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/interactor.py
--rw-r--r--   0 runner    (1001) docker     (127)    22843 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/script.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_config.sample.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/verify/wait.py
--rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.431017 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.jxb
--rw-r--r--   0 runner    (1001) docker     (127)   343351 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.xsd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24392 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:45:02.000000 galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-03 02:45:02.435017 galaxy-tool-util-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-03 02:43:42.000000 galaxy-tool-util-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.457683 galaxy_tool_util-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    22442 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    24628 2024-05-02 13:48:07.457683 galaxy_tool_util-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.429683 galaxy_tool_util-24.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.429683 galaxy_tool_util-24.0.1/galaxy/tool_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.433683 galaxy_tool_util-24.0.1/galaxy/tool_util/biotools/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/biotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1699 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/biotools/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/biotools/source.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.433683 galaxy_tool_util-24.0.1/galaxy/tool_util/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14528 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/client/staging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.433683 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/cwltool_deps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45945 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18637 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/representation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9400 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/runtime_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4076 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25745 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.433683 galaxy_tool_util-24.0.1/galaxy/tool_util/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    59526 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/data/_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.433683 galaxy_tool_util-24.0.1/galaxy/tool_util/data/bundles/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/data/bundles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/data/bundles/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.437683 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/
+-rw-r--r--   0 runner    (1001) docker     (127)    20484 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    19566 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/brew_exts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/brew_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/conda_compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27451 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/conda_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22865 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.437683 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10890 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/explicit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29706 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/mulled.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18185 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6766 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/docker_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2673 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/dockerfiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/installable.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.441683 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11859 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/get_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/invfile.lua
+-rw-r--r--   0 runner    (1001) docker     (127)    22233 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build_channel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build_files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build_tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5062 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15814 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10081 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17250 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13328 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/requirements.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.441683 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11210 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5379 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20607 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/conda.py
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5389 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/galaxy_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/homebrew.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7972 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/lmod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/resolver_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7543 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/singularity_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18441 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/deps/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/edam_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/fetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13112 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/lint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.445683 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/citations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3408 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8665 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/help.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52233 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9940 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22415 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/xml_order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1173 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/linters/xsd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9921 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/loader_directory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.445683 galaxy_tool_util-24.0.1/galaxy/tool_util/locations/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/locations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/locations/dockstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/locations/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/locations/http.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.445683 galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53080 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/biotools_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/edam_operation_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/edam_topic_mappings.tsv
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/ontology_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8805 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/output_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.445683 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5857 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4558 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19354 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/output_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5866 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/output_collection_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16163 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/output_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4171 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/stdio.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54802 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/parser/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9462 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/provided_metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.449683 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      366 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65232 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.449683 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     4454 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4726 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/filters/examples.py.sample
+-rw-r--r--   0 runner    (1001) docker     (127)     6939 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/integrated_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.449683 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/lineages/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/lineages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/lineages/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2767 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/lineages/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10207 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/panel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4813 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.449683 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3941 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/edam.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/sources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9266 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/static.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/watcher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.449683 galaxy_tool_util-24.0.1/galaxy/tool_util/unittest_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/unittest_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/unittest_utils/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/unittest_utils/sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.453683 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/
+-rw-r--r--   0 runner    (1001) docker     (127)    21690 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.453683 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3184 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/archive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/hdf5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1429 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/size.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/tabular.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5350 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5371 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75994 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/interactor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22843 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/script.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/test_config.sample.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4113 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1430 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/verify/wait.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4877 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.453683 galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/galaxy.jxb
+-rw-r--r--   0 runner    (1001) docker     (127)   343351 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/galaxy.xsd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:48:07.453683 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24628 2024-05-02 13:48:07.000000 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-02 13:48:07.000000 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:48:07.000000 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-02 13:48:07.000000 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-02 13:48:07.000000 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:48:07.000000 galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-05-02 13:48:07.457683 galaxy_tool_util-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-02 13:46:45.000000 galaxy_tool_util-24.0.1/test-requirements.txt
```

### Comparing `galaxy-tool-util-24.0.0/HISTORY.rst` & `galaxy_tool_util-24.0.1/HISTORY.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,24 @@
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix conditional Image imports by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17899 <https://github.com/galaxyproject/galaxy/pull/17899>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-tool-util-24.0.0/LICENSE` & `galaxy_tool_util-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/PKG-INFO` & `galaxy_tool_util-24.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tool-util
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy tool and tool dependency utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,14 +64,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix conditional Image imports by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17899 <https://github.com/galaxyproject/galaxy/pull/17899>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/interface.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/biotools/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/biotools/source.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/biotools/source.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/client/staging.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/client/staging.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/cwltool_deps.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/cwltool_deps.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/parser.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/representation.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/representation.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runnable.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/runnable.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/runtime_actions.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/runtime_actions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/schema.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/cwl/util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/cwl/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/data/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/data/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/data/_schema.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/data/_schema.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/data/bundles/models.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/data/bundles/models.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_exts.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/brew_exts.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/brew_util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/brew_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_compat.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/conda_compat.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/conda_util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/conda_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_classes.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_classes.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/explicit.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/explicit.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/mulled.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/mulled.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_resolvers/test.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_resolvers/test.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/container_volumes.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/container_volumes.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/containers.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/containers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dependencies.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/dependencies.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/docker_util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/docker_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/dockerfiles.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/dockerfiles.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/installable.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/installable.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/get_tests.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/get_tests.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/invfile.lua` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/invfile.lua`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_channel.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build_channel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_files.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build_files.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_build_tool.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_build_tool.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_hash.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_hash.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_list.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_list.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_search.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_search.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/mulled_update_singularity_containers.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/mulled/util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/mulled/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/requirements.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/requirements.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/brewed_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/conda.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/conda.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/default_conda_mapping.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/galaxy_packages.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/galaxy_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/homebrew.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/homebrew.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/lmod.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/lmod.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/modules.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/modules.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/resolver_mixins.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/resolver_mixins.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/tool_shed_packages.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/resolvers/unlinked_tool_shed_packages.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/singularity_util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/singularity_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/deps/views.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/deps/views.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/edam_util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/edam_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/fetcher.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/fetcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/lint.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/lint.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/citations.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/citations.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/command.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/command.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/cwl.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/cwl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/general.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/general.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/help.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/help.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/inputs.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/inputs.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/outputs.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/outputs.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/stdio.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/tests.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/tests.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xml_order.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/xml_order.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/linters/xsd.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/linters/xsd.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/loader_directory.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/loader_directory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/locations/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/locations/dockstore.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/locations/dockstore.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/biotools_mappings.tsv` & `galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/biotools_mappings.tsv`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/ontologies/ontology_data.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/ontologies/ontology_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/output_checker.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/output_checker.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/cwl.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/cwl.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/factory.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/interface.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_actions.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/output_actions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_collection_def.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/output_collection_def.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/output_objects.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/output_objects.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/stdio.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/stdio.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/xml.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/xml.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/parser/yaml.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/provided_metadata.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/provided_metadata.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/base.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/base.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/filters/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/filters/examples.py.sample` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/filters/examples.py.sample`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/integrated_panel.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/integrated_panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/factory.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/lineages/factory.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/lineages/interface.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/lineages/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/panel.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/panel.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/parser.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/parser.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/definitions.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/definitions.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/edam.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/edam.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/interface.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/interface.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/sources.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/sources.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/views/static.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/views/static.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/toolbox/watcher.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/toolbox/watcher.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/unittest_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/unittest_utils/interactor.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/unittest_utils/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 try:
     import pysam
 except ImportError:
     pass
 try:
     from PIL import Image
 except ImportError:
-    pass
+    Image = None  # type: ignore[assignment]
 
 from galaxy.tool_util.parser.util import (
     DEFAULT_DELTA,
     DEFAULT_DELTA_FRAC,
     DEFAULT_EPS,
     DEFAULT_METRIC,
 )
```

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/__init__.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/_util.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/_util.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/archive.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/archive.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/hdf5.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/hdf5.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/json.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/json.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/size.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/size.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/tabular.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/tabular.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/text.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/text.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/asserts/xml.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/asserts/xml.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/interactor.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/interactor.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/script.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/script.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_config.sample.yml` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/test_config.sample.yml`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/test_data.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/test_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/verify/wait.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/verify/wait.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/version.py` & `galaxy_tool_util-24.0.1/galaxy/tool_util/version.py`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/LICENSE` & `galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/README.md` & `galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/README.md`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.jxb` & `galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/galaxy.jxb`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy/tool_util/xsd/galaxy.xsd` & `galaxy_tool_util-24.0.1/galaxy/tool_util/xsd/galaxy.xsd`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/PKG-INFO` & `galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-tool-util
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy tool and tool dependency utilities
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -64,14 +64,25 @@
 
 History
 -------
 
 .. to_doc
 
 -------------------
+24.0.1 (2024-05-02)
+-------------------
+
+
+=========
+Bug fixes
+=========
+
+* Fix conditional Image imports by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17899 <https://github.com/galaxyproject/galaxy/pull/17899>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/SOURCES.txt` & `galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/galaxy_tool_util.egg-info/entry_points.txt` & `galaxy_tool_util-24.0.1/galaxy_tool_util.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `galaxy-tool-util-24.0.0/setup.cfg` & `galaxy_tool_util-24.0.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-tool-util
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-util>=22.1
 	conda-package-streaming
 	lxml!=4.2.2
```

