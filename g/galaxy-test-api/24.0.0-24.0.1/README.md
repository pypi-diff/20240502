# Comparing `tmp/galaxy-test-api-24.0.0.tar.gz` & `tmp/galaxy_test_api-24.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-test-api-24.0.0.tar", last modified: Wed Apr  3 02:46:08 2024, max compression
+gzip compressed data, was "galaxy_test_api-24.0.1.tar", last modified: Thu May  2 13:49:13 2024, max compression
```

## Comparing `galaxy-test-api-24.0.0.tar` & `galaxy_test_api-24.0.1.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    15479 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.135843 galaxy-test-api-24.0.0/galaxy_test/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.143843 galaxy-test-api-24.0.0/galaxy_test/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/_framework.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.143843 galaxy-test-api-24.0.0/galaxy_test/api/cwl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/cwl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/embed_test_1.gxwf.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/embed_test_1_tool.gxtool.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/sharable.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_container_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)    33392 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_dataset_collections.py
--rw-r--r--   0 runner    (1001) docker     (127)    38871 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_datatypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_display_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_drs.py
--rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_folder_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_folders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_group_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_group_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    51434 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_histories.py
--rw-r--r--   0 runner    (1001) docker     (127)    78017 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents_provenance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5771 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_item_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    53965 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_libraries.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_page_revisions.py
--rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_pages.py
--rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_short_term_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tool_data.py
--rw-r--r--   0 runner    (1001) docker     (127)   148593 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)    46383 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tools_upload.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_tours.py
--rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_visualizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_webhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)    27526 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflow_extraction.py
--rw-r--r--   0 runner    (1001) docker     (127)   289951 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflows.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflows_cwl.py
--rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/api/test_workflows_from_yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/galaxy_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17010 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-03 02:46:08.000000 galaxy-test-api-24.0.0/galaxy_test_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-03 02:46:08.147843 galaxy-test-api-24.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-03 02:43:42.000000 galaxy-test-api-24.0.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.242053 galaxy_test_api-24.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    17251 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    12875 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-05-02 13:49:13.242053 galaxy_test_api-24.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.230053 galaxy_test_api-24.0.1/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.238053 galaxy_test_api-24.0.1/galaxy_test/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/_framework.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.238053 galaxy_test_api-24.0.1/galaxy_test/api/cwl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/cwl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/embed_test_1.gxwf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/embed_test_1_tool.gxtool.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7592 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/sharable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_container_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33522 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_dataset_collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39575 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5103 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_datatypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_display_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5217 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_drs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19567 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_folder_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7524 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_folders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1775 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_group_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6054 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_group_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51434 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_histories.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78797 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents_provenance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5726 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_item_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54283 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29503 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_libraries.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_page_revisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_pages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8773 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_short_term_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5501 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tool_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)   148621 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46383 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tools_upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_tours.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16370 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6257 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_visualizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27526 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflow_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (127)   292809 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflows.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflows_cwl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11420 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/api/test_workflows_from_yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:13.238053 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    18782 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-02 13:49:13.000000 galaxy_test_api-24.0.1/galaxy_test_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-05-02 13:49:13.242053 galaxy_test_api-24.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-02 13:46:45.000000 galaxy_test_api-24.0.1/test-requirements.txt
```

### Comparing `galaxy-test-api-24.0.0/HISTORY.rst` & `galaxy_test_api-24.0.1/HISTORY.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,33 @@
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
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Always serialize element_count and populated when listing contents by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17890 <https://github.com/galaxyproject/galaxy/pull/17890>`_
+* Make `wait_for_history_jobs` look at jobs, not datasets by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17892 <https://github.com/galaxyproject/galaxy/pull/17892>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+* Fix get_content_as_text for compressed text datatypes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17976 <https://github.com/galaxyproject/galaxy/pull/17976>`_
+* Raise appropriate exception if user forces a collection that is not populated with elements as input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18023 <https://github.com/galaxyproject/galaxy/pull/18023>`_
+* Fix ``test_get_tags_histories_content`` test by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18026 <https://github.com/galaxyproject/galaxy/pull/18026>`_
+* Ensure that offset and limit are never negative by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18044 <https://github.com/galaxyproject/galaxy/pull/18044>`_
+* Fix history update time after bulk operation by `@davelopez <https://github.com/davelopez>`_ in `#18068 <https://github.com/galaxyproject/galaxy/pull/18068>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-api-24.0.0/LICENSE` & `galaxy_test_api-24.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/PKG-INFO` & `galaxy_test_api-24.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,14 +50,34 @@
 
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
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Always serialize element_count and populated when listing contents by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17890 <https://github.com/galaxyproject/galaxy/pull/17890>`_
+* Make `wait_for_history_jobs` look at jobs, not datasets by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17892 <https://github.com/galaxyproject/galaxy/pull/17892>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+* Fix get_content_as_text for compressed text datatypes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17976 <https://github.com/galaxyproject/galaxy/pull/17976>`_
+* Raise appropriate exception if user forces a collection that is not populated with elements as input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18023 <https://github.com/galaxyproject/galaxy/pull/18023>`_
+* Fix ``test_get_tags_histories_content`` test by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18026 <https://github.com/galaxyproject/galaxy/pull/18026>`_
+* Ensure that offset and limit are never negative by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18044 <https://github.com/galaxyproject/galaxy/pull/18044>`_
+* Fix history update time after bulk operation by `@davelopez <https://github.com/davelopez>`_ in `#18068 <https://github.com/galaxyproject/galaxy/pull/18068>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/_framework.py` & `galaxy_test_api-24.0.1/galaxy_test/api/_framework.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/sharable.py` & `galaxy_test_api-24.0.1/galaxy_test/api/sharable.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_authenticate.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_authenticate.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_configuration.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_configuration.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_container_resolution.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_container_resolution.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_dataset_collections.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_dataset_collections.py`

 * *Files 0% similar despite different names*

```diff
@@ -451,25 +451,27 @@
         assert dataset_collection["id"] == hdca_id
         assert dataset_collection["collection_type"] == "list"
 
     def test_show_dataset_collection_contents(self, history_id):
         # Get contents_url from history contents, use it to show the first level
         # of collection contents in the created HDCA, then use it again to drill
         # down into the nested collection contents
-        hdca = self.dataset_collection_populator.create_list_of_list_in_history(history_id).json()
+        hdca = self.dataset_collection_populator.create_list_of_list_in_history(history_id, wait=True).json()
         root_contents_url = self._get_contents_url_for_hdca(history_id, hdca)
 
         # check root contents for this collection
         root_contents = self._get(root_contents_url).json()
         assert len(root_contents) == len(hdca["elements"])
         self._compare_collection_contents_elements(root_contents, hdca["elements"])
 
         # drill down, retrieve nested collection contents
         assert "object" in root_contents[0]
         assert "contents_url" in root_contents[0]["object"]
+        assert root_contents[0]["object"]["element_count"] == 3
+        assert root_contents[0]["object"]["populated"]
         drill_contents_url = root_contents[0]["object"]["contents_url"]
         drill_contents = self._get(drill_contents_url).json()
         assert len(drill_contents) == len(hdca["elements"][0]["object"]["elements"])
         self._compare_collection_contents_elements(drill_contents, hdca["elements"][0]["object"]["elements"])
 
     def test_collection_contents_limit_offset(self, history_id):
         # check limit/offset params for collection contents endpoint
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_datasets.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_datasets.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 )
 
 from galaxy.model.unittest_utils.store_fixtures import (
     deferred_hda_model_store_dict,
     one_hda_model_store_dict,
     TEST_SOURCE_URI,
 )
+from galaxy.tool_util.verify.test_data import TestDataResolver
 from galaxy.util.unittest_utils import skip_if_github_down
 from galaxy_test.base.api_asserts import assert_has_keys
 from galaxy_test.base.decorators import (
     requires_admin,
     requires_new_history,
 )
 from galaxy_test.base.populators import (
@@ -352,14 +353,23 @@
         )
         hda1 = self.dataset_populator.new_dataset(history_id, content=contents, wait=True)
         get_content_as_text_response = self._get(f"datasets/{hda1['id']}/get_content_as_text")
         self._assert_status_code_is(get_content_as_text_response, 200)
         self._assert_has_key(get_content_as_text_response.json(), "item_data")
         assert get_content_as_text_response.json().get("item_data") == contents
 
+    def test_get_content_as_text_with_compressed_text_data(self, history_id):
+        test_data_resolver = TestDataResolver()
+        with open(test_data_resolver.get_filename("1.fasta.gz"), mode="rb") as fh:
+            hda1 = self.dataset_populator.new_dataset(history_id, content=fh, ftype="fasta.gz", wait=True)
+        get_content_as_text_response = self._get(f"datasets/{hda1['id']}/get_content_as_text")
+        self._assert_status_code_is(get_content_as_text_response, 200)
+        self._assert_has_key(get_content_as_text_response.json(), "item_data")
+        assert ">hg17" in get_content_as_text_response.json().get("item_data")
+
     def test_anon_get_content_as_text(self, history_id):
         contents = "accessible data"
         hda1 = self.dataset_populator.new_dataset(history_id, content=contents, wait=True)
         with self._different_user(anon=True):
             get_content_as_text_response = self._get(f"datasets/{hda1['id']}/get_content_as_text")
             self._assert_status_code_is(get_content_as_text_response, 200)
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_datatypes.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_display_applications.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_display_applications.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_drs.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_drs.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_folder_contents.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_folder_contents.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_folders.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_folders.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_framework.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_framework.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_group_roles.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_group_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_group_users.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_group_users.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_groups.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_groups.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_histories.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_histories.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents.py`

 * *Files 1% similar despite different names*

```diff
@@ -1621,20 +1621,35 @@
     ) -> Optional[Any]:
         for item in history_contents:
             if item["history_content_type"] == history_content_type and item["id"] == dataset_id:
                 return item
         return None
 
     def _apply_bulk_operation(self, history_id: str, payload, query: str = "", expected_status_code: int = 200):
+        original_history_update_time = self._get_history_update_time(history_id)
         if query:
             query = f"?{query}"
         response = self._put(
             f"histories/{history_id}/contents/bulk{query}",
             data=payload,
             json=True,
         )
         self._assert_status_code_is(response, expected_status_code)
-        return response.json()
+        result = response.json()
+
+        if "err_msg" in result or result.get("success_count", 0) == 0:
+            # We don't need to check the history update time if there was an error or no items were updated
+            return result
+
+        # After a successful operation, history update time should be updated so the changes can be detected by the frontend
+        after_bulk_operation_history_update_time = self._get_history_update_time(history_id)
+        assert after_bulk_operation_history_update_time > original_history_update_time
+
+        return result
 
     def _assert_bulk_success(self, bulk_operation_result, expected_success_count: int):
         assert bulk_operation_result["success_count"] == expected_success_count, bulk_operation_result
         assert not bulk_operation_result["errors"]
+
+    def _get_history_update_time(self, history_id: str):
+        history = self._get(f"histories/{history_id}").json()
+        return history.get("update_time")
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_history_contents_provenance.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_history_contents_provenance.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_item_tags.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_item_tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,17 +131,17 @@
     def _create_valid_tag(self, prefix: str):
         url = f"{prefix}/tags/awesometagname"
         tag_data: Dict[str, Any] = {}  # Can also be dict(value="awesometagvalue")
         response = self._post(url, data=tag_data, json=True)
         return response
 
     def _create_history_contents(self, history_id):
-        history_content_id = self.dataset_collection_populator.create_list_in_history(
-            history_id, contents=["test_dataset"], direct_upload=True, wait=True
-        ).json()["outputs"][0]["id"]
+        history_content_id = self.dataset_populator.new_dataset(
+            history_id, contents="test_dataset", direct_upload=True, wait=True
+        )["id"]
         return history_content_id
 
     def _create_history(self):
         history_id = self.dataset_populator.new_history()
         return history_id
 
     def _create_workflow(self):
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_jobs.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,22 +178,27 @@
         workflow_jobs = self.__jobs_index(data={"workflow_id": workflow_id})
         second_invocation_jobs = self.__jobs_index(data={"invocation_id": second_invocation_id})
         assert len(workflow_jobs) == 2
         assert len(second_invocation_jobs) == 1
 
     @pytest.mark.require_new_history
     def test_index_limit_and_offset_filter(self, history_id):
+        # create 2 datasets
+        self.__history_with_new_dataset(history_id)
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(data={"history_id": history_id})
         assert len(jobs) > 0
         length = len(jobs)
         jobs = self.__jobs_index(data={"history_id": history_id, "offset": 1})
         assert len(jobs) == length - 1
-        jobs = self.__jobs_index(data={"history_id": history_id, "limit": 0})
-        assert len(jobs) == 0
+        jobs = self.__jobs_index(data={"history_id": history_id, "limit": 1})
+        assert len(jobs) == 1
+        response = self._get("jobs", data={"history_id": history_id, "limit": -1})
+        assert response.status_code == 400
+        assert response.json()["err_msg"] == "Input should be greater than or equal to 1 in ('query', 'limit')"
 
     @pytest.mark.require_new_history
     def test_index_search_filter_tool_id(self, history_id):
         self.__history_with_new_dataset(history_id)
         jobs = self.__jobs_index(data={"history_id": history_id})
         assert len(jobs) > 0
         length = len(jobs)
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_libraries.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_libraries.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_licenses.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_licenses.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_page_revisions.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_page_revisions.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_pages.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_pages.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_roles.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_roles.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_short_term_storage.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_short_term_storage.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_tags.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_tags.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_tool_data.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_tool_data.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_tools.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_tools.py`

 * *Files 0% similar despite different names*

```diff
@@ -1655,17 +1655,16 @@
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         self._run_and_check_simple_collection_mapping(history_id, inputs)
 
     @skip_without_tool("cat1")
     def test_map_over_empty_collection(self, history_id):
-        hdca_id = self.dataset_collection_populator.create_list_in_history(history_id, contents=[]).json()["outputs"][
-            0
-        ]["id"]
+        response = self.dataset_collection_populator.create_list_in_history(history_id, contents=[], wait=True).json()
+        hdca_id = response["output_collections"][0]["id"]
         inputs = {
             "input1": {"batch": True, "values": [{"src": "hdca", "id": hdca_id}]},
         }
         create = self._run_cat1(history_id, inputs=inputs, assert_ok=True)
         outputs = create["outputs"]
         jobs = create["jobs"]
         implicit_collections = create["implicit_collections"]
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_tools_upload.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_tools_upload.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_tours.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_tours.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_users.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_users.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_visualizations.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_visualizations.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_webhooks.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_webhooks.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_workflow_extraction.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_workflow_extraction.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_workflows.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_workflows.py`

 * *Files 0% similar despite different names*

```diff
@@ -899,14 +899,41 @@
         data = {"name": "", "steps": {}}
         update_response = self._update_workflow(workflow["id"], data)
         assert update_response.json()["err_msg"] == "Workflow must have a valid name"
         self._assert_status_code_is(update_response, 400)
         workflow_dict = self.workflow_populator.download_workflow(workflow["id"])
         assert workflow_dict["name"] == original_name
 
+    @skip_without_tool("select_from_dataset_in_conditional")
+    def test_workflow_run_form_with_broken_dataset(self):
+        workflow_id = self.workflow_populator.upload_yaml_workflow(
+            """
+class: GalaxyWorkflow
+inputs:
+  dataset: data
+steps:
+  select_from_dataset_in_conditional:
+    tool_id: select_from_dataset_in_conditional
+    in:
+      single: dataset
+    state:
+      cond:
+        cond: single
+        select_single: abc
+        inner_cond:
+          inner_cond: single
+          select_single: abc
+"""
+        )
+        with self.dataset_populator.test_history() as history_id:
+            self.dataset_populator.new_dataset(history_id, content="a", file_type="tabular", wait=True)
+            workflow = self._download_workflow(workflow_id, style="run", history_id=history_id)
+            assert not workflow["has_upgrade_messages"]
+            assert workflow["steps"][1]["inputs"][0]["value"] == {"__class__": "ConnectedValue"}
+
     def test_refactor(self):
         workflow_id = self.workflow_populator.upload_yaml_workflow(
             """
 class: GalaxyWorkflow
 inputs:
   test_input: data
 steps:
@@ -939,14 +966,44 @@
         refactor_response.raise_for_status()
         assert refactor_response.json()["workflow"]["steps"]["0"]["label"] == "new_label"
 
         # this time dry_run was default of False, so the label is indeed changed
         workflow_dict = self.workflow_populator.download_workflow(workflow_id)
         assert workflow_dict["steps"]["0"]["label"] == "new_label"
 
+    def test_refactor_tool_state_upgrade(self):
+        workflow_id = self.workflow_populator.upload_yaml_workflow(
+            """
+class: GalaxyWorkflow
+inputs: {}
+steps:
+  multiple_versions_changes:
+    tool_id: multiple_versions_changes
+    tool_version: "0.1"
+    state:
+      inttest: 1
+      cond:
+        bool_to_select: false
+"""
+        )
+        actions = [{"action_type": "upgrade_all_steps"}]
+        refactor_response = self.workflow_populator.refactor_workflow(workflow_id, actions, dry_run=True)
+        refactor_response.raise_for_status()
+        refactor_result = refactor_response.json()
+        upgrade_result = refactor_result["action_executions"][0]
+        assert upgrade_result["action"]["action_type"] == "upgrade_all_steps"
+        message_one, message_two = upgrade_result["messages"]
+        assert message_one["message"] == "No value found for 'floattest'. Using default: '1.0'."
+        assert message_one["input_name"] == "floattest"
+        assert message_two["message"] == "The selected case is unavailable/invalid. Using default: 'b'."
+        assert message_two["input_name"] == "cond|bool_to_select"
+
+        refactor_response = self.workflow_populator.refactor_workflow(workflow_id, actions, dry_run=False)
+        refactor_response.raise_for_status()
+
     def test_update_no_tool_id(self):
         workflow_object = self.workflow_populator.load_workflow(name="test_import")
         upload_response = self.__test_upload(workflow=workflow_object)
         workflow_id = upload_response.json()["id"]
         del workflow_object["steps"]["2"]["tool_id"]
         put_response = self._update_workflow(workflow_id, workflow_object)
         self._assert_status_code_is(put_response, 400)
@@ -3966,14 +4023,39 @@
         ext: tabular
 """,
                 history_id=history_id,
                 wait=True,
                 assert_ok=True,
             )
 
+    @skip_without_tool("implicit_conversion_format_input")
+    def test_run_with_implicit_collection_map_over(self):
+        with self.dataset_populator.test_history() as history_id:
+            self._run_workflow(
+                """
+class: GalaxyWorkflow
+inputs:
+  collection: collection
+steps:
+  map_over:
+    tool_id: implicit_conversion_format_input
+    in:
+      input1: collection
+test_data:
+  collection:
+    collection_type: list
+    elements:
+      - identifier: 1
+        value: 1.fasta.gz
+        type: File
+""",
+                history_id=history_id,
+                assert_ok=True,
+            )
+
     @skip_without_tool("random_lines1")
     def test_change_datatype_collection_map_over(self):
         with self.dataset_populator.test_history() as history_id:
             jobs_summary = self._run_workflow(
                 """
 class: GalaxyWorkflow
 inputs:
@@ -5473,15 +5555,15 @@
   wf_output_1:
     outputSource: output_filter/out_1
 steps:
   output_filter:
     tool_id: output_filter
     state:
       produce_out_1: False
-      filter_text_1: '1'
+      filter_text_1: 'foo'
       produce_collection: False
 """,
                 test_data={},
                 history_id=history_id,
                 wait=False,
             )
             self.workflow_populator.wait_for_invocation_and_jobs(
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test/api/test_workflows_from_yaml.py` & `galaxy_test_api-24.0.1/galaxy_test/api/test_workflows_from_yaml.py`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/galaxy_test_api.egg-info/PKG-INFO` & `galaxy_test_api-24.0.1/galaxy_test_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galaxy-test-api
-Version: 24.0.0
+Version: 24.0.1
 Summary: Galaxy API tests
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
 Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
@@ -50,14 +50,34 @@
 
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
+* Fix tool version switch in editor by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17858 <https://github.com/galaxyproject/galaxy/pull/17858>`_
+* Fix workflow run form failing on certain histories by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17869 <https://github.com/galaxyproject/galaxy/pull/17869>`_
+* Always serialize element_count and populated when listing contents by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17890 <https://github.com/galaxyproject/galaxy/pull/17890>`_
+* Make `wait_for_history_jobs` look at jobs, not datasets by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17892 <https://github.com/galaxyproject/galaxy/pull/17892>`_
+* Fix missing implicit conversion for mapped over jobs by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17952 <https://github.com/galaxyproject/galaxy/pull/17952>`_
+* Fix get_content_as_text for compressed text datatypes by `@mvdbeek <https://github.com/mvdbeek>`_ in `#17976 <https://github.com/galaxyproject/galaxy/pull/17976>`_
+* Raise appropriate exception if user forces a collection that is not populated with elements as input by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18023 <https://github.com/galaxyproject/galaxy/pull/18023>`_
+* Fix ``test_get_tags_histories_content`` test by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18026 <https://github.com/galaxyproject/galaxy/pull/18026>`_
+* Ensure that offset and limit are never negative by `@mvdbeek <https://github.com/mvdbeek>`_ in `#18044 <https://github.com/galaxyproject/galaxy/pull/18044>`_
+* Fix history update time after bulk operation by `@davelopez <https://github.com/davelopez>`_ in `#18068 <https://github.com/galaxyproject/galaxy/pull/18068>`_
+
+-------------------
 24.0.0 (2024-04-02)
 -------------------
 
 
 =========
 Bug fixes
 =========
```

### Comparing `galaxy-test-api-24.0.0/galaxy_test_api.egg-info/SOURCES.txt` & `galaxy_test_api-24.0.1/galaxy_test_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `galaxy-test-api-24.0.0/setup.cfg` & `galaxy_test_api-24.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 license = AFL
 license_files = 
 	LICENSE
 long_description = file: README.rst, HISTORY.rst
 long_description_content_type = text/x-rst
 name = galaxy-test-api
 url = https://github.com/galaxyproject/galaxy
-version = 24.0.0
+version = 24.0.1
 
 [options]
 include_package_data = True
 install_requires = 
 	galaxy-test-base
 	pytest
 	python-dateutil
```

