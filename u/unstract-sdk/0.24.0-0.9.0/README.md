# Comparing `tmp/unstract_sdk-0.24.0.tar.gz` & `tmp/unstract_sdk-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstract_sdk-0.24.0.tar", last modified: Thu May  2 04:31:26 2024, max compression
+gzip compressed data, was "unstract_sdk-0.9.0.tar", last modified: Tue Feb 20 12:56:59 2024, max compression
```

## Comparing `unstract_sdk-0.24.0.tar` & `unstract_sdk-0.9.0.tar`

### file list

```diff
@@ -1,67 +1,67 @@
--rw-r--r--   0        0        0    34523 2024-05-02 04:31:06.798291 unstract_sdk-0.24.0/LICENSE
--rw-r--r--   0        0        0     2180 2024-05-02 04:31:06.798291 unstract_sdk-0.24.0/README.md
--rw-r--r--   0        0        0     2032 2024-05-02 04:31:26.182108 unstract_sdk-0.24.0/pyproject.toml
--rw-r--r--   0        0        0     1065 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/LICENSE
--rw-r--r--   0        0        0      106 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/__init__.py
--rw-r--r--   0        0        0     3800 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/adapters.py
--rw-r--r--   0        0        0     3831 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/audit.py
--rw-r--r--   0        0        0     3621 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/cache.py
--rw-r--r--   0        0        0     3551 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/constants.py
--rw-r--r--   0        0        0     2134 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/embedding.py
--rw-r--r--   0        0        0      524 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/exceptions.py
--rw-r--r--   0        0        0      556 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/helper.py
--rw-r--r--   0        0        0    13393 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/index.py
--rw-r--r--   0        0        0     4041 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/llm.py
--rw-r--r--   0        0        0     1318 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/ocr.py
--rw-r--r--   0        0        0     2701 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/platform.py
--rw-r--r--   0        0        0     4985 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/prompt.py
--rwxr-xr-x   0        0        0     2102 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/scripts/tool_gen.py
--rw-r--r--   0        0        0       18 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/.dockerignore
--rw-r--r--   0        0        0      387 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/Dockerfile
--rw-r--r--   0        0        0     3396 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/README.md
--rw-r--r--   0        0        0        0 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/data_dir/COPY_TO_FOLDER/.gitkeep
--rw-r--r--   0        0        0      327 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/data_dir/INFILE
--rw-r--r--   0        0        0      249 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/data_dir/METADATA.json
--rw-r--r--   0        0        0      216 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/data_dir/SOURCE
--rw-r--r--   0        0        0      120 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/requirements.txt
--rw-r--r--   0        0        0      175 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/sample.env
--rw-r--r--   0        0        0     1520 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/config/icon.svg
--rw-r--r--   0        0        0     2091 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/config/properties.json
--rw-r--r--   0        0        0      143 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/config/spec.json
--rw-r--r--   0        0        0     1039 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/main.py
--rw-r--r--   0        0        0        0 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/__init__.py
--rw-r--r--   0        0        0    10129 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/base.py
--rw-r--r--   0        0        0      899 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/entrypoint.py
--rw-r--r--   0        0        0     2352 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/executor.py
--rw-r--r--   0        0        0    38700 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/mime_types.py
--rw-r--r--   0        0        0     2098 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/mixin.py
--rw-r--r--   0        0        0     1696 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/parser.py
--rw-r--r--   0        0        0     7725 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/stream.py
--rw-r--r--   0        0        0     7568 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/tool/validator.py
--rw-r--r--   0        0        0       42 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/utils/__init__.py
--rw-r--r--   0        0        0     3681 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/utils/callback_manager.py
--rw-r--r--   0        0        0     3212 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/utils/tool_utils.py
--rw-r--r--   0        0        0     4364 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/utils/usage_handler.py
--rw-r--r--   0        0        0     3228 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/vector_db.py
--rw-r--r--   0        0        0     2104 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/src/unstract/sdk/x2txt.py
--rw-r--r--   0        0        0        0 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/__init__.py
--rw-r--r--   0        0        0     1673 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/config/properties.json
--rw-r--r--   0        0        0      314 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/config/runtime_variables.json
--rw-r--r--   0        0        0      143 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/config/spec.json
--rw-r--r--   0        0        0      292 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/sample.env
--rw-r--r--   0        0        0     1539 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/test_cache.py
--rw-r--r--   0        0        0     1344 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/test_embedding.py
--rw-r--r--   0        0        0     1987 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/test_llm.py
--rw-r--r--   0        0        0     1755 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/test_ocr.py
--rw-r--r--   0        0        0     1589 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/test_vector_db.py
--rw-r--r--   0        0        0     1862 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/test_x2text.py
--rw-r--r--   0        0        0        0 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/__init__.py
--rw-r--r--   0        0        0     1520 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/config/icon.svg
--rw-r--r--   0        0        0      795 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/config/properties.json
--rw-r--r--   0        0        0      314 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/config/runtime_variables.json
--rw-r--r--   0        0        0     1130 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/config/spec.json
--rw-r--r--   0        0        0      795 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/config/tool_properties.json
--rw-r--r--   0        0        0     1130 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/config/tool_spec.json
--rw-r--r--   0        0        0     3090 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/test_entrypoint.py
--rw-r--r--   0        0        0     2252 2024-05-02 04:31:06.810291 unstract_sdk-0.24.0/tests/tool/test_static.py
--rw-r--r--   0        0        0     3401 1970-01-01 00:00:00.000000 unstract_sdk-0.24.0/PKG-INFO
+-rw-r--r--   0        0        0     1978 2024-02-20 12:55:06.491043 unstract_sdk-0.9.0/README.md
+-rw-r--r--   0        0        0     1639 2024-02-20 12:56:59.576392 unstract_sdk-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1065 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/LICENSE
+-rw-r--r--   0        0        0      105 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/__init__.py
+-rw-r--r--   0        0        0     3799 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/adapters.py
+-rw-r--r--   0        0        0     3460 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/audit.py
+-rw-r--r--   0        0        0     3620 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/cache.py
+-rw-r--r--   0        0        0     3503 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/constants.py
+-rw-r--r--   0        0        0     3745 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/dbs.py
+-rw-r--r--   0        0        0    12834 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/documents.py
+-rw-r--r--   0        0        0     2518 2024-02-20 12:55:06.423043 unstract_sdk-0.9.0/src/unstract/sdk/embedding.py
+-rw-r--r--   0        0        0      417 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/exceptions.py
+-rw-r--r--   0        0        0     5446 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/file_system.py
+-rw-r--r--   0        0        0      556 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/helper.py
+-rw-r--r--   0        0        0    12935 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/index.py
+-rw-r--r--   0        0        0     4052 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/llm.py
+-rw-r--r--   0        0        0     2700 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/platform.py
+-rw-r--r--   0        0        0     4437 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/prompt.py
+-rwxr-xr-x   0        0        0     2102 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/scripts/tool_gen.py
+-rw-r--r--   0        0        0       18 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/.dockerignore
+-rw-r--r--   0        0        0      387 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/Dockerfile
+-rw-r--r--   0        0        0     3396 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/README.md
+-rw-r--r--   0        0        0        0 2024-02-20 12:55:06.427043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/data_dir/COPY_TO_FOLDER/.gitkeep
+-rw-r--r--   0        0        0      327 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/data_dir/INFILE
+-rw-r--r--   0        0        0      249 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/data_dir/METADATA.json
+-rw-r--r--   0        0        0      216 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/data_dir/SOURCE
+-rw-r--r--   0        0        0      120 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/requirements.txt
+-rw-r--r--   0        0        0      175 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/sample.env
+-rw-r--r--   0        0        0     1520 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/config/icon.svg
+-rw-r--r--   0        0        0     2091 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/config/properties.json
+-rw-r--r--   0        0        0      143 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/config/spec.json
+-rw-r--r--   0        0        0     1039 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/main.py
+-rw-r--r--   0        0        0        0 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/__init__.py
+-rw-r--r--   0        0        0     9959 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/base.py
+-rw-r--r--   0        0        0      899 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/entrypoint.py
+-rw-r--r--   0        0        0     2241 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/executor.py
+-rw-r--r--   0        0        0    38700 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/mime_types.py
+-rw-r--r--   0        0        0     2098 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/mixin.py
+-rw-r--r--   0        0        0     1695 2024-02-20 12:55:06.431043 unstract_sdk-0.9.0/src/unstract/sdk/tool/parser.py
+-rw-r--r--   0        0        0     7724 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/tool/stream.py
+-rw-r--r--   0        0        0     8079 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/tool/validator.py
+-rw-r--r--   0        0        0       42 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/utils/__init__.py
+-rw-r--r--   0        0        0     4170 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/utils/service_context.py
+-rw-r--r--   0        0        0     2518 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/utils/tool_utils.py
+-rw-r--r--   0        0        0     4631 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/utils/usage_handler.py
+-rw-r--r--   0        0        0     3370 2024-02-20 12:55:06.435043 unstract_sdk-0.9.0/src/unstract/sdk/vector_db.py
+-rw-r--r--   0        0        0        0 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0     1673 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/config/properties.json
+-rw-r--r--   0        0        0      314 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/config/runtime_variables.json
+-rw-r--r--   0        0        0      143 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/config/spec.json
+-rw-r--r--   0        0        0      192 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/sample.env
+-rw-r--r--   0        0        0     1539 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/test_cache.py
+-rw-r--r--   0        0        0     1650 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/test_dbs.py
+-rw-r--r--   0        0        0     2093 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/test_document.py
+-rw-r--r--   0        0        0     1348 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/test_embedding.py
+-rw-r--r--   0        0        0     1986 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/test_llm.py
+-rw-r--r--   0        0        0     1565 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/test_vector_db.py
+-rw-r--r--   0        0        0        0 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/tool/__init__.py
+-rw-r--r--   0        0        0     1520 2024-02-20 12:55:06.443043 unstract_sdk-0.9.0/tests/tool/config/icon.svg
+-rw-r--r--   0        0        0      795 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/config/properties.json
+-rw-r--r--   0        0        0      314 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/config/runtime_variables.json
+-rw-r--r--   0        0        0     1130 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/config/spec.json
+-rw-r--r--   0        0        0      795 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/config/tool_properties.json
+-rw-r--r--   0        0        0     1130 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/config/tool_spec.json
+-rw-r--r--   0        0        0     3090 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/test_entrypoint.py
+-rw-r--r--   0        0        0     2252 2024-02-20 12:55:06.447043 unstract_sdk-0.9.0/tests/tool/test_static.py
+-rw-r--r--   0        0        0     3590 1970-01-01 00:00:00.000000 unstract_sdk-0.9.0/PKG-INFO
```

### Comparing `unstract_sdk-0.24.0/pyproject.toml` & `unstract_sdk-0.9.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -4,56 +4,55 @@
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "unstract-sdk"
 dynamic = []
 description = "A framework for writing Unstract Tools/Apps"
+authors = [
+    { name = "Zipstack Inc", email = "devsupport@zipstack.com" },
+]
 dependencies = [
+    "unstract-connectors~=0.0.2",
     "jsonschema~=4.18.2",
     "python-magic~=0.4.27",
     "python-dotenv==1.0.0",
-    "unstract-adapters~=0.12.1",
-    "llama-index==0.10.28",
+    "unstract-adapters~=0.1.1",
+    "llama-index==0.9.28",
     "tiktoken~=0.4.0",
     "transformers==4.37.0",
+    "filetype==1.2.0",
+    "pdfplumber==0.10.3",
+    "pytesseract==0.3.10",
 ]
+requires-python = ">=3.9,<3.11.1"
 readme = "README.md"
-authors = [
-    { name = "Zipstack Inc", email = "devsupport@zipstack.com" },
-]
 keywords = [
-    "unstract tools-development-kit apps development-kit sdk",
+    "unstract tools-development-kit apps -development-kit sdk",
 ]
-requires-python = ">=3.9,<3.11.1"
 classifiers = [
-    "Development Status :: 4 - Beta",
+    "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: GNU Affero General Public License v3",
-    "Operating System :: POSIX :: Linux",
-    "Operating System :: MacOS :: MacOS X",
-    "Programming Language :: Python",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.9",
     "Topic :: Scientific/Engineering",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-version = "0.24.0"
-
-[project.urls]
-Homepage = "https://unstract.com"
-"Release notes" = "https://github.com/Zipstack/unstract-sdk/releases"
-Source = "https://github.com/Zipstack/unstract-sdk"
+version = "0.9.0"
 
 [project.license]
-text = "AGPL v3"
+text = "MIT"
+
+[project.urls]
+Homepage = "https://unstract.com/sdk"
 
 [project.scripts]
 unstract-tool-gen = "unstract.sdk.scripts.tool_gen:main"
 
-[tool.pdm.dev-dependencies]
+[project.optional-dependencies]
 docs = [
     "lazydocs~=0.4.8",
 ]
 test = [
     "parameterized==0.9.0",
 ]
 lint = [
@@ -72,19 +71,7 @@
     "src",
 ]
 package-dir = "src"
 
 [tool.pdm.version]
 source = "file"
 path = "src/unstract/sdk/__init__.py"
-
-[tool.pdm.resolution.overrides]
-grpcio = ">=1.62.1"
-
-[tool.isort]
-line_length = 88
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-profile = "black"
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/LICENSE` & `unstract_sdk-0.9.0/src/unstract/sdk/LICENSE`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/adapters.py` & `unstract_sdk-0.9.0/src/unstract/sdk/adapters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Optional
 
 import requests
-
 from unstract.sdk.constants import AdapterKeys, LogLevel, ToolEnv
 from unstract.sdk.platform import PlatformBase
 from unstract.sdk.tool.base import BaseTool
 
 
 class ToolAdapter(PlatformBase):
     """Class to handle Adapters for Unstract Tools.
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/audit.py` & `unstract_sdk-0.9.0/src/unstract/sdk/audit.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,59 @@
 import requests
-from llama_index.core.callbacks import CBEventType, TokenCountingHandler
-
+from llama_index.callbacks import TokenCountingHandler
+from llama_index.callbacks.schema import CBEventType
 from unstract.sdk.constants import LogLevel, ToolEnv
 from unstract.sdk.helper import SdkHelper
 from unstract.sdk.tool.stream import StreamMixin
 
 
 class Audit(StreamMixin):
     """The 'Audit' class is responsible for pushing usage data to the platform
     service.
 
     Methods:
         - push_usage_data: Pushes the usage data to the platform service.
 
     Attributes:
         None
+
+    Example usage:
+        audit = Audit()
+        audit.push_usage_data(
+            token_counter,
+            workflow_id,
+            execution_id,
+            external_service,
+            event_type)
     """
 
     def __init__(self, log_level: LogLevel = LogLevel.INFO) -> None:
         super().__init__(log_level)
 
     def push_usage_data(
         self,
         platform_api_key: str,
         token_counter: TokenCountingHandler = None,
-        model_name: str = "",
+        workflow_id: str = "",
+        execution_id: str = "",
+        external_service: str = "",
         event_type: CBEventType = None,
-        **kwargs,
     ) -> None:
         """Pushes the usage data to the platform service.
 
         Args:
-            platform_api_key (str): The platform API key.
             token_counter (TokenCountingHandler, optional): The token counter
-                object. Defaults to None.
-            model_name (str, optional): The name of the model.
-                Defaults to "".
+              object. Defaults to None.
+            workflow_id (str, optional): The ID of the workflow. Defaults to "".
+            execution_id (str, optional): The ID of the execution. Defaults
+              to "".
+            external_service (str, optional): The name of the external service.
+              Defaults to "".
             event_type (CBEventType, optional): The type of the event. Defaults
-                to None.
-            **kwargs: Optional keyword arguments.
-                workflow_id (str, optional): The ID of the workflow.
-                    Defaults to "".
-                execution_id (str, optional): The ID of the execution. Defaults
-                    to "".
-                adapter_instance_id (str, optional): The adapter instance ID.
-                    Defaults to "".
-                run_id (str, optional): The run ID. Defaults to "".
+              to None.
 
         Returns:
             None
 
         Raises:
             requests.RequestException: If there is an error while pushing the
             usage details.
@@ -58,26 +62,19 @@
         platform_port = self.get_env_or_die(ToolEnv.PLATFORM_PORT)
 
         base_url = SdkHelper.get_platform_base_url(
             platform_host=platform_host, platform_port=platform_port
         )
         bearer_token = platform_api_key
 
-        workflow_id = kwargs.get("workflow_id", "")
-        execution_id = kwargs.get("execution_id", "")
-        adapter_instance_id = kwargs.get("adapter_instance_id", "")
-        run_id = kwargs.get("run_id", "")
-
         data = {
+            "usage_type": event_type,
+            "external_service": external_service,
             "workflow_id": workflow_id,
             "execution_id": execution_id,
-            "adapter_instance_id": adapter_instance_id,
-            "run_id": run_id,
-            "usage_type": event_type,
-            "model_name": model_name,
             "embedding_tokens": token_counter.total_embedding_token_count,
             "prompt_tokens": token_counter.prompt_llm_token_count,
             "completion_tokens": token_counter.completion_llm_token_count,
             "total_tokens": token_counter.total_llm_token_count,
         }
 
         url = f"{base_url}/usage"
@@ -99,10 +96,7 @@
                 self.stream_log("Successfully pushed usage details")
 
         except requests.RequestException as e:
             self.stream_log(
                 log=f"Error while pushing usage details: {e}",
                 level=LogLevel.ERROR,
             )
-
-        finally:
-            token_counter.reset_counts()
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/cache.py` & `unstract_sdk-0.9.0/src/unstract/sdk/cache.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Optional
 
 import requests
-
 from unstract.sdk.constants import LogLevel
 from unstract.sdk.platform import PlatformBase
 from unstract.sdk.tool.base import BaseTool
 
 
 class ToolCache(PlatformBase):
     """Class to handle caching for Unstract Tools.
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/constants.py` & `unstract_sdk-0.9.0/src/unstract/sdk/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,14 +135,16 @@
 class ToolSettingsKey:
     """A class representing the keys used in the tool settings.
 
     Attributes:
         LLM_ADAPTER_ID (str): The key for the LLM adapter ID.
         EMBEDDING_ADAPTER_ID (str): The key for the embedding adapter ID.
         VECTOR_DB_ADAPTER_ID (str): The key for the vector DB adapter ID.
-        X2TEXT_ADAPTER_ID (str): The key for the X2Text adapter ID.
     """
 
     LLM_ADAPTER_ID = "llmAdapterId"
     EMBEDDING_ADAPTER_ID = "embeddingAdapterId"
     VECTOR_DB_ADAPTER_ID = "vectorDbAdapterId"
-    X2TEXT_ADAPTER_ID = "x2TextAdapterId"
+
+
+class FileReaderSettings:
+    FILE_READER_CHUNK_SIZE = 8192
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/embedding.py` & `unstract_sdk-0.9.0/src/unstract/sdk/embedding.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,56 +1,64 @@
-from llama_index.core.embeddings import BaseEmbedding
+from typing import Optional
+
+from llama_index.embeddings.base import BaseEmbedding
 from unstract.adapters.constants import Common
 from unstract.adapters.embedding import adapters
-
 from unstract.sdk.adapters import ToolAdapter
-from unstract.sdk.constants import LogLevel
-from unstract.sdk.exceptions import SdkError
+from unstract.sdk.constants import LogLevel, ToolSettingsKey
 from unstract.sdk.tool.base import BaseTool
 
 
 class ToolEmbedding:
     __TEST_SNIPPET = "Hello, I am Unstract"
 
-    def __init__(self, tool: BaseTool):
+    def __init__(self, tool: BaseTool, tool_settings: dict[str, str] = {}):
         self.tool = tool
         self.max_tokens = 1024 * 16
         self.embedding_adapters = adapters
-
-    def get_embedding(self, adapter_instance_id: str) -> BaseEmbedding:
-        """Gets an instance of LlamaIndex's embedding object.
-
-        Args:
-            adapter_instance_id (str): UUID of the embedding adapter
-
-        Returns:
-            BaseEmbedding: Embedding instance
-        """
-        try:
-            embedding_config_data = ToolAdapter.get_adapter_config(
-                self.tool, adapter_instance_id
-            )
-            embedding_adapter_id = embedding_config_data.get(Common.ADAPTER_ID)
-            if embedding_adapter_id not in self.embedding_adapters:
-                raise SdkError(
-                    f"Embedding adapter not supported : "
-                    f"{embedding_adapter_id}"
+        self.embedding_adapter_instance_id = tool_settings.get(
+            ToolSettingsKey.EMBEDDING_ADAPTER_ID
+        )
+        self.embedding_adapter_id: Optional[str] = None
+
+    def get_embedding(
+        self, adapter_instance_id: Optional[str] = None
+    ) -> Optional[BaseEmbedding]:
+        adapter_instance_id = (
+            adapter_instance_id
+            if adapter_instance_id
+            else self.embedding_adapter_instance_id
+        )
+        if adapter_instance_id is not None:
+            try:
+                embedding_config_data = ToolAdapter.get_adapter_config(
+                    self.tool, adapter_instance_id
                 )
-
-            embedding_adapter = self.embedding_adapters[embedding_adapter_id][
-                Common.METADATA
-            ][Common.ADAPTER]
-            embedding_metadata = embedding_config_data.get(
-                Common.ADAPTER_METADATA
-            )
-            embedding_adapter_class = embedding_adapter(embedding_metadata)
-            return embedding_adapter_class.get_embedding_instance()
-        except Exception as e:
-            self.tool.stream_log(
-                log=f"Error getting embedding: {e}", level=LogLevel.ERROR
-            )
-            raise SdkError(f"Error getting embedding instance: {e}")
+                embedding_adapter_id = embedding_config_data.get(
+                    Common.ADAPTER_ID
+                )
+                self.embedding_adapter_id = embedding_adapter_id
+                if embedding_adapter_id in self.embedding_adapters:
+                    embedding_adapter = self.embedding_adapters[
+                        embedding_adapter_id
+                    ][Common.METADATA][Common.ADAPTER]
+                    embedding_metadata = embedding_config_data.get(
+                        Common.ADAPTER_METADATA
+                    )
+                    embedding_adapter_class = embedding_adapter(
+                        embedding_metadata
+                    )
+                    return embedding_adapter_class.get_embedding_instance()
+                else:
+                    return None
+            except Exception as e:
+                self.tool.stream_log(
+                    log=f"Error getting embedding: {e}", level=LogLevel.ERROR
+                )
+                return None
+        else:
+            return None
 
     def get_embedding_length(self, embedding: BaseEmbedding) -> int:
         embedding_list = embedding._get_text_embedding(self.__TEST_SNIPPET)
         embedding_dimension = len(embedding_list)
         return embedding_dimension
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/helper.py` & `unstract_sdk-0.9.0/src/unstract/sdk/helper.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/index.py` & `unstract_sdk-0.9.0/src/unstract/sdk/index.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,75 +1,77 @@
-import json
+import os
+import shutil
+import zipfile
 from typing import Optional
 
-from llama_index.core import Document
-from llama_index.core.indices.vector_store import VectorStoreIndex
-from llama_index.core.node_parser import SimpleNodeParser
-from llama_index.core.storage import StorageContext
-from llama_index.core.vector_stores import (
-    FilterOperator,
-    MetadataFilter,
-    MetadataFilters,
-    VectorStoreQuery,
-    VectorStoreQueryResult,
-)
-from unstract.adapters.exceptions import AdapterError
-from unstract.adapters.x2text.x2text_adapter import X2TextAdapter
+import filetype
+from llama_index import Document, StorageContext, VectorStoreIndex
+from llama_index.node_parser import SimpleNodeParser
+from llama_index.vector_stores import VectorStoreQuery, VectorStoreQueryResult
 
-from unstract.sdk.adapters import ToolAdapter
 from unstract.sdk.constants import LogLevel, ToolEnv
 from unstract.sdk.embedding import ToolEmbedding
-from unstract.sdk.exceptions import IndexingError, SdkError
+from unstract.sdk.exceptions import SdkException
 from unstract.sdk.tool.base import BaseTool
 from unstract.sdk.utils import ToolUtils
-from unstract.sdk.utils.callback_manager import CallbackManager as UNCallbackManager
+from unstract.sdk.utils.service_context import ServiceContext
 from unstract.sdk.vector_db import ToolVectorDB
-from unstract.sdk.x2txt import X2Text
+
+allowed_pdf_to_text_converters = [
+    "default",
+    "unstract_llm_whisperer",
+    "unstract_camelot",
+]
 
 
 class ToolIndex:
     def __init__(self, tool: BaseTool):
-        # TODO: Inherit from StreamMixin and avoid using BaseTool
         self.tool = tool
 
-    def get_text_from_index(self, embedding_type: str, vector_db: str, doc_id: str):
+    def get_text_from_index(
+        self, embedding_type: str, vector_db: str, doc_id: str
+    ):
         embedd_helper = ToolEmbedding(tool=self.tool)
-        embedding_li = embedd_helper.get_embedding(adapter_instance_id=embedding_type)
+        embedding_li = embedd_helper.get_embedding(
+            adapter_instance_id=embedding_type
+        )
+        if embedding_li is None:
+            self.tool.stream_log(
+                f"Error loading {embedding_type}", level=LogLevel.ERROR
+            )
+            raise SdkException(f"Error loading {embedding_type}")
         embedding_dimension = embedd_helper.get_embedding_length(embedding_li)
 
         vdb_helper = ToolVectorDB(
             tool=self.tool,
         )
         vector_db_li = vdb_helper.get_vector_db(
             adapter_instance_id=vector_db,
             embedding_dimension=embedding_dimension,
         )
 
+        if vector_db_li is None:
+            self.tool.stream_log(
+                f"Error loading {vector_db}", level=LogLevel.ERROR
+            )
+            raise SdkException(f"Error loading {vector_db}")
+
         try:
             self.tool.stream_log(f">>> Querying {vector_db}...")
             self.tool.stream_log(f">>> {doc_id}")
-            doc_id_eq_filter = MetadataFilter.from_dict(
-                {
-                    "key": "doc_id",
-                    "operator": FilterOperator.EQ,
-                    "value": doc_id,
-                }
-            )
-            filters = MetadataFilters(filters=[doc_id_eq_filter])
             q = VectorStoreQuery(
                 query_embedding=embedding_li.get_query_embedding(" "),
                 doc_ids=[doc_id],
-                filters=filters,
                 similarity_top_k=10000,
             )
         except Exception as e:
             self.tool.stream_log(
                 f"Error querying {vector_db}: {e}", level=LogLevel.ERROR
             )
-            raise SdkError(f"Error querying {vector_db}: {e}")
+            raise SdkException(f"Error querying {vector_db}: {e}")
 
         n: VectorStoreQueryResult = vector_db_li.query(query=q)
         if len(n.nodes) > 0:
             self.tool.stream_log(f"Found {len(n.nodes)} nodes for {doc_id}")
             all_text = ""
             for node in n.nodes:
                 all_text += node.get_content()
@@ -100,236 +102,249 @@
         return "\n".join(new_context_lines)
 
     def index_file(
         self,
         tool_id: str,
         embedding_type: str,
         vector_db: str,
-        x2text_adapter: str,
         file_path: str,
         chunk_size: int,
         chunk_overlap: int,
         reindex: bool = False,
+        converter: str = "default",
         file_hash: Optional[str] = None,
-        output_file_path: Optional[str] = None,
-    ) -> str:
-        """Indexes an individual file using the passed arguments.
+    ):
+        if converter not in allowed_pdf_to_text_converters:
+            self.tool.stream_log(
+                "pdf-to-text-converters must be one of "
+                f"{allowed_pdf_to_text_converters}",
+                level=LogLevel.ERROR,
+            )
+            raise SdkException(
+                "pdf-to-text-converters must be one of "
+                f"{allowed_pdf_to_text_converters}"
+            )
 
-        Args:
-            tool_id (str): UUID of the tool (workflow_id in case its called
-                from workflow)
-            embedding_type (str): UUID of the embedding service configured
-            vector_db (str): UUID of the vector DB configured
-            x2text_adapter (str): UUID of the x2text adapter configured.
-                This is to extract text from documents.
-            file_path (str): Path to the file that needs to be indexed.
-            chunk_size (int): Chunk size to be used for indexing
-            chunk_overlap (int): Overlap in chunks to be used for indexing
-            reindex (bool, optional): Flag to denote if document should be
-                re-indexed if its already indexed. Defaults to False.
-            file_hash (Optional[str], optional): SHA256 hash of the file.
-                Defaults to None. If None, the hash is generated.
-            output_file_path (Optional[str], optional): File path to write
-                the extracted contents into. Defaults to None.
+        input_file_type = None
+        input_file_type_mime = None
 
-        Returns:
-            str: A unique ID for the file and indexing arguments combination
-        """
-        doc_id = self.generate_file_id(
+        # Make file content hash if not available
+        if not file_hash:
+            file_hash = ToolUtils.get_hash_from_file(file_path=file_path)
+        with open(file_path, mode="rb") as input_file_obj:
+            sample_contents = input_file_obj.read(100)
+            input_file_type = filetype.guess(sample_contents)
+
+        if input_file_type is None:
+            input_file_type_mime = "text/plain"
+        else:
+            input_file_type_mime = input_file_type.MIME
+
+        self.tool.stream_log(f"Input file type: {input_file_type_mime}")
+
+        full_text = []
+
+        if input_file_type_mime == "text/plain":
+            with open(file_path) as input_file_obj:
+                full_text.append(
+                    {
+                        "section": "full",
+                        "text_contents": self._cleanup_text(
+                            input_file_obj.read()
+                        ),
+                    }
+                )
+
+        elif input_file_type_mime == "application/pdf":
+            raise SdkException(
+                "Indexing of PDF files is not supported currently"
+            )
+            # TODO: Make use of adapters to convert X2Text
+            # self.tool.stream_log(f"PDF to text converter: {converter}")
+            # if converter == "unstract_llm_whisperer" or converter == "default":  # noqa
+            #     full_text.append(
+            #         {
+            #             "section": "full",
+            #             "text_contents": self._cleanup_text(
+            #                 x2txt.generate_whisper(
+            #                     input_file=file_path,
+            #                     mode="text",
+            #                     dump_text=True,
+            #                 )
+            #             ),
+            #         }
+            #     )
+            # else:
+            #     # TODO : Support for Camelot
+            #     x2txt = X2Text(tool=self.tool)
+
+        elif input_file_type_mime == "application/zip":
+            self.tool.stream_log("Zip file extraction required")
+            with zipfile.ZipFile(file_path, "r") as zip_ref:
+                file_name_from_path = os.path.basename(file_path)
+                temp_directory = f"/tmp/unstract_zip/{file_name_from_path}"
+                # If temp_directory exists, delete it and create it again
+                if os.path.exists(temp_directory):
+                    shutil.rmtree(temp_directory)
+                os.makedirs(temp_directory)
+                zip_ref.extractall(temp_directory)
+        else:
+            self.tool.stream_log(
+                f"Unsupported file type: {input_file_type_mime}",
+                level=LogLevel.ERROR,
+            )
+            raise SdkException(f"Unsupported file type: {input_file_type_mime}")
+
+        doc_id = ToolIndex.generate_file_id(
             tool_id=tool_id,
+            file_hash=file_hash,
             vector_db=vector_db,
             embedding=embedding_type,
-            x2text=x2text_adapter,
-            chunk_size=str(chunk_size),
-            chunk_overlap=str(chunk_overlap),
-            file_path=file_path,
-            file_hash=file_hash,
+            chunk_size=chunk_size,
+            chunk_overlap=chunk_overlap,
         )
-        self.tool.stream_log(f"Checking if doc_id {doc_id} exists")
 
-        # Get embedding instance
-        embedd_helper = ToolEmbedding(tool=self.tool)
-        embedding_li = embedd_helper.get_embedding(adapter_instance_id=embedding_type)
-        embedding_dimension = embedd_helper.get_embedding_length(embedding_li)
+        self.tool.stream_log(f"Checking if doc_id {doc_id} exists")
 
-        # Get vectorDB instance
         vdb_helper = ToolVectorDB(
             tool=self.tool,
         )
+
+        embedd_helper = ToolEmbedding(tool=self.tool)
+
+        embedding_li = embedd_helper.get_embedding(
+            adapter_instance_id=embedding_type
+        )
+        if embedding_li is None:
+            self.tool.stream_log(
+                f"Error loading {embedding_type}", level=LogLevel.ERROR
+            )
+            raise SdkException(f"Error loading {embedding_type}")
+
+        embedding_dimension = embedd_helper.get_embedding_length(embedding_li)
         vector_db_li = vdb_helper.get_vector_db(
             adapter_instance_id=vector_db,
             embedding_dimension=embedding_dimension,
         )
+        if vector_db_li is None:
+            self.tool.stream_log(
+                f"Error loading {vector_db}", level=LogLevel.ERROR
+            )
+            raise SdkException(f"Error loading {vector_db}")
 
-        # Checking if document is already indexed against doc_id
-        doc_id_eq_filter = MetadataFilter.from_dict(
-            {"key": "doc_id", "operator": FilterOperator.EQ, "value": doc_id}
-        )
-        filters = MetadataFilters(filters=[doc_id_eq_filter])
         q = VectorStoreQuery(
             query_embedding=embedding_li.get_query_embedding(" "),
             doc_ids=[doc_id],
-            filters=filters,
         )
 
-        doc_id_found = False
+        doc_id_not_found = True
         try:
             n: VectorStoreQueryResult = vector_db_li.query(query=q)
             if len(n.nodes) > 0:
-                doc_id_found = True
+                doc_id_not_found = False
                 self.tool.stream_log(f"Found {len(n.nodes)} nodes for {doc_id}")
             else:
                 self.tool.stream_log(f"No nodes found for {doc_id}")
         except Exception as e:
             self.tool.stream_log(
                 f"Error querying {vector_db}: {e}", level=LogLevel.ERROR
             )
 
-        if doc_id_found and reindex:
+        if doc_id_not_found is False and reindex:
             # Delete the nodes for the doc_id
             try:
                 vector_db_li.delete(ref_doc_id=doc_id)
                 self.tool.stream_log(f"Deleted nodes for {doc_id}")
             except Exception as e:
                 self.tool.stream_log(
                     f"Error deleting nodes for {doc_id}: {e}",
                     level=LogLevel.ERROR,
                 )
-                raise SdkError(f"Error deleting nodes for {doc_id}: {e}")
-            doc_id_found = False
-
-        if doc_id_found:
-            self.tool.stream_log(f"File was indexed already under {doc_id}")
-            return doc_id
+                raise SdkException(f"Error deleting nodes for {doc_id}: {e}")
+            doc_id_not_found = True
 
-        # Extract text and index
-        self.tool.stream_log("Extracting text from input file")
-        full_text = []
-        extracted_text = ""
-        try:
-            mime_type = ToolUtils.get_file_mime_type(file_path)
-            if mime_type == "text/plain":
-                with open(file_path, encoding="utf-8") as file:
-                    extracted_text = file.read()
+        if doc_id_not_found:
+            # Check if chunking is required
+            documents = []
+            for item in full_text:
+                text = item["text_contents"]
+                self.tool.stream_log("Indexing file...")
+                document = Document(
+                    text=text,
+                    doc_id=doc_id,
+                    metadata={"section": item["section"]},
+                )
+                document.id_ = doc_id
+                documents.append(document)
+            self.tool.stream_log(f"Number of documents: {len(documents)}")
+            if chunk_size == 0:
+                parser = SimpleNodeParser.from_defaults(
+                    chunk_size=len(documents[0].text) + 10, chunk_overlap=0
+                )
+                nodes = parser.get_nodes_from_documents(
+                    documents, show_progress=True
+                )
+                node = nodes[0]
+                node.embedding = embedding_li.get_query_embedding(" ")
+                vector_db_li.add(nodes=[node])
+                self.tool.stream_log("Added node to vector db")
             else:
-                x2text = X2Text(tool=self.tool)
-                x2text_adapter_inst: X2TextAdapter = x2text.get_x2text(
-                    adapter_instance_id=x2text_adapter
+                storage_context = StorageContext.from_defaults(
+                    vector_store=vector_db_li
                 )
-                extracted_text = x2text_adapter_inst.process(
-                    input_file_path=file_path, output_file_path=output_file_path
+                parser = SimpleNodeParser.from_defaults(
+                    chunk_size=chunk_size, chunk_overlap=chunk_overlap
                 )
-        except AdapterError as e:
-            # Wrapping AdapterErrors with SdkError
-            raise IndexingError(str(e)) from e
-        full_text.append(
-            {
-                "section": "full",
-                "text_contents": self._cleanup_text(extracted_text),
-            }
-        )
 
-        # Check if chunking is required
-        documents = []
-        for item in full_text:
-            text = item["text_contents"]
-            self.tool.stream_log("Indexing file...")
-            document = Document(
-                text=text,
-                doc_id=doc_id,
-                metadata={"section": item["section"]},
-            )
-            document.id_ = doc_id
-            documents.append(document)
-        self.tool.stream_log(f"Number of documents: {len(documents)}")
-        if chunk_size == 0:
-            parser = SimpleNodeParser.from_defaults(
-                chunk_size=len(documents[0].text) + 10, chunk_overlap=0
-            )
-            nodes = parser.get_nodes_from_documents(documents, show_progress=True)
-            node = nodes[0]
-            node.embedding = embedding_li.get_query_embedding(" ")
-            vector_db_li.add(nodes=[node])
-            self.tool.stream_log("Added node to vector db")
-        else:
-            storage_context = StorageContext.from_defaults(vector_store=vector_db_li)
-            parser = SimpleNodeParser.from_defaults(
-                chunk_size=chunk_size, chunk_overlap=chunk_overlap
-            )
-
-            # Set callback_manager to collect Usage stats
-            callback_manager = UNCallbackManager.set_callback_manager(
-                platform_api_key=self.tool.get_env_or_die(ToolEnv.PLATFORM_API_KEY),
-                embedding=embedding_li,
-            )
-
-            self.tool.stream_log("Adding nodes to vector db...")
-            try:
-                VectorStoreIndex.from_documents(
-                    documents,
-                    storage_context=storage_context,
-                    show_progress=True,
+                service_context = ServiceContext.get_service_context(
+                    platform_api_key=self.tool.get_env_or_die(
+                        ToolEnv.PLATFORM_API_KEY
+                    ),
                     embed_model=embedding_li,
                     node_parser=parser,
-                    callback_manager=callback_manager,
-                )
-            except Exception as e:
-                self.tool.stream_log(
-                    f"Error adding nodes to vector db: {e}",
-                    level=LogLevel.ERROR,
                 )
-                raise IndexingError(str(e)) from e
-            self.tool.stream_log("Added nodes to vector db")
 
-        self.tool.stream_log("File has been indexed successfully")
+                self.tool.stream_log("Adding nodes to vector db...")
+                try:
+                    VectorStoreIndex.from_documents(
+                        documents,
+                        storage_context=storage_context,
+                        show_progress=True,
+                        service_context=service_context,
+                    )
+                except Exception as e:
+                    self.tool.stream_log(
+                        f"Error adding nodes to vector db: {e}",
+                        level=LogLevel.ERROR,
+                    )
+                    raise SdkException(f"Error adding nodes to vector db: {e}")
+                self.tool.stream_log("Added nodes to vector db")
+
+        self.tool.stream_log("Done indexing file")
         return doc_id
 
+    @staticmethod
     def generate_file_id(
-        self,
         tool_id: str,
+        file_hash: str,
         vector_db: str,
         embedding: str,
-        x2text: str,
         chunk_size: str,
         chunk_overlap: str,
-        file_path: Optional[str] = None,
-        file_hash: Optional[str] = None,
     ) -> str:
         """Generates a unique ID useful for identifying files during indexing.
 
         Args:
-            tool_id (str): Unique ID of the tool or workflow
+            tool_id (str): Unique ID of the tool developed / exported
+            file_hash (str): Hash of the file contents
             vector_db (str): UUID of the vector DB adapter
             embedding (str): UUID of the embedding adapter
-            x2text (str): UUID of the X2Text adapter
             chunk_size (str): Chunk size for indexing
             chunk_overlap (str): Chunk overlap for indexing
-            file_path (Optional[str]): Path to the file that needs to be indexed.
-                Defaults to None. One of file_path or file_hash needs to be specified.
-            file_hash (Optional[str], optional): SHA256 hash of the file.
-                Defaults to None. If None, the hash is generated with file_path.
 
         Returns:
             str: Key representing unique ID for a file
         """
-        if not file_path and not file_hash:
-            raise ValueError("One of `file_path` or `file_hash` need to be provided")
-
-        if not file_hash:
-            file_hash = ToolUtils.get_hash_from_file(file_path=file_path)
-
-        # Whole adapter config is used currently even though it contains some keys
-        # which might not be relevant to indexing. This is easier for now than
-        # marking certain keys of the adapter config as necessary.
-        index_key = {
-            "tool_id": tool_id,
-            "file_hash": file_hash,
-            "vector_db_config": ToolAdapter.get_adapter_config(self.tool, vector_db),
-            "embedding_config": ToolAdapter.get_adapter_config(self.tool, embedding),
-            "x2text_config": ToolAdapter.get_adapter_config(self.tool, x2text),
-            "chunk_size": chunk_size,
-            "chunk_overlap": chunk_overlap,
-        }
-        # JSON keys are sorted to ensure that the same key gets hashed even in
-        # case where the fields are reordered.
-        hashed_index_key = ToolUtils.hash_str(json.dumps(index_key, sort_keys=True))
-        return hashed_index_key
+        return (
+            f"{tool_id}|{vector_db}|{embedding}|"
+            f"{chunk_size}|{chunk_overlap}|{file_hash}"
+        )
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/llm.py` & `unstract_sdk-0.9.0/src/unstract/sdk/llm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,116 +1,115 @@
 import logging
-import re
 import time
 from typing import Any, Optional
 
-from llama_index.core.llms import LLM, CompletionResponse
+from llama_index.llms import LLM
+from llama_index.llms.base import CompletionResponse
 from unstract.adapters.constants import Common
 from unstract.adapters.llm import adapters
 from unstract.adapters.llm.llm_adapter import LLMAdapter
-
 from unstract.sdk.adapters import ToolAdapter
-from unstract.sdk.constants import LogLevel
-from unstract.sdk.exceptions import SdkError
+from unstract.sdk.constants import LogLevel, ToolSettingsKey
 from unstract.sdk.tool.base import BaseTool
-from unstract.sdk.utils.callback_manager import (
-    CallbackManager as UNCallbackManager,
-)
+from unstract.sdk.utils.service_context import ServiceContext
 
 logger = logging.getLogger(__name__)
 
 
 class ToolLLM:
     """Class to handle LLMs for Unstract Tools."""
 
-    json_regex = re.compile(r"\{(?:.|\n)*\}")
-
-    def __init__(self, tool: BaseTool):
-        """ToolLLM constructor.
+    def __init__(
+        self,
+        tool: BaseTool,
+        tool_settings: dict[str, str] = {},
+    ):
+        """
 
         Notes:
             - "Azure OpenAI" : Environment variables required
             OPENAI_API_KEY,OPENAI_API_BASE, OPENAI_API_VERSION,
             OPENAI_API_ENGINE, OPENAI_API_MODEL
 
         Args:
             tool (AbstractTool): Instance of AbstractTool
         """
         self.tool = tool
         self.max_tokens = 1024 * 4
         self.llm_adapters = adapters
-        self.llm_config_data: Optional[dict[str, Any]] = None
+        self.llm_adapter_instance_id = tool_settings.get(
+            ToolSettingsKey.LLM_ADAPTER_ID
+        )
 
-    @classmethod
+    @staticmethod
     def run_completion(
-        cls,
         llm: LLM,
         platform_api_key: str,
         prompt: str,
         retries: int = 3,
         **kwargs: Any,
     ) -> Optional[dict[str, Any]]:
-        # Setup callback manager to collect Usage stats
-        UNCallbackManager.set_callback_manager(
-            platform_api_key=platform_api_key, llm=llm, **kwargs
+        ServiceContext.get_service_context(
+            platform_api_key=platform_api_key, llm=llm
         )
-        # Removing specific keys from kwargs
-        new_kwargs = kwargs.copy()
-        for key in [
-            "workflow_id",
-            "execution_id",
-            "adapter_instance_id",
-            "run_id",
-        ]:
-            new_kwargs.pop(key, None)
         for i in range(retries):
             try:
-                response: CompletionResponse = llm.complete(
-                    prompt, **new_kwargs
-                )
-                match = cls.json_regex.search(response.text)
-                if match:
-                    response.text = match.group(0)
-                return {"response": response}
+                response: CompletionResponse = llm.complete(prompt, **kwargs)
+                result = {
+                    "response": response,
+                }
 
+                return result
             except Exception as e:
                 if i == retries - 1:
                     raise e
                 time.sleep(5)
         return None
 
-    def get_llm(self, adapter_instance_id: str) -> LLM:
+    def get_llm(
+        self, adapter_instance_id: Optional[str] = None
+    ) -> Optional[LLM]:
         """Returns the LLM object for the tool.
 
         Returns:
-            LLM: The LLM object for the tool.
+            Optional[LLM]: The LLM object for the tool.
             (llama_index.llms.base.LLM)
         """
-        try:
-            llm_config_data = ToolAdapter.get_adapter_config(
-                self.tool, adapter_instance_id
-            )
-            llm_adapter_id = llm_config_data.get(Common.ADAPTER_ID)
-            if llm_adapter_id not in self.llm_adapters:
-                raise SdkError(
-                    f"LLM adapter not supported : " f"{llm_adapter_id}"
+        adapter_instance_id = (
+            adapter_instance_id
+            if adapter_instance_id
+            else self.llm_adapter_instance_id
+        )
+        # Support for get_llm using adapter_instance_id
+        if adapter_instance_id is not None:
+            try:
+                llm_config_data = ToolAdapter.get_adapter_config(
+                    self.tool, adapter_instance_id
                 )
-
-            llm_adapter = self.llm_adapters[llm_adapter_id][
-                Common.METADATA
-            ][Common.ADAPTER]
-            llm_metadata = llm_config_data.get(Common.ADAPTER_METADATA)
-            llm_adapter_class: LLMAdapter = llm_adapter(llm_metadata)
-            llm_instance: LLM = llm_adapter_class.get_llm_instance()
-            return llm_instance
-        except Exception as e:
-            self.tool.stream_log(
-                log=f"Unable to get llm instance: {e}", level=LogLevel.ERROR
-            )
-            raise SdkError(f"Error getting llm instance: {e}")
+                llm_adapter_id = llm_config_data.get(Common.ADAPTER_ID)
+                if llm_adapter_id in self.llm_adapters:
+                    llm_adapter = self.llm_adapters[llm_adapter_id][
+                        Common.METADATA
+                    ][Common.ADAPTER]
+                    llm_metadata = llm_config_data.get(Common.ADAPTER_METADATA)
+                    llm_adapter_class: LLMAdapter = llm_adapter(llm_metadata)
+                    llm_instance: Optional[
+                        LLM
+                    ] = llm_adapter_class.get_llm_instance()
+                    return llm_instance
+                else:
+                    return None
+            except Exception as e:
+                self.tool.stream_log(
+                    log=f"Unable to get llm instance: {e}", level=LogLevel.ERROR
+                )
+                return None
+        else:
+            logger.error("The adapter_instance_id parameter is None")
+            return None
 
     def get_max_tokens(self, reserved_for_output: int = 0) -> int:
         """Returns the maximum number of tokens that can be used for the LLM.
 
         Args:
             reserved_for_output (int): The number of tokens reserved for the
                                         output.
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/platform.py` & `unstract_sdk-0.9.0/src/unstract/sdk/platform.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from typing import Any, Optional
 
 import requests
-
 from unstract.sdk.constants import LogLevel, ToolEnv
 from unstract.sdk.helper import SdkHelper
 from unstract.sdk.tool.base import BaseTool
 
 
 class PlatformBase:
     """Base class to handle interactions with Unstract's platform service.
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/prompt.py` & `unstract_sdk-0.9.0/src/unstract/sdk/prompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from typing import Any, Optional
 
 import requests
-from requests import RequestException, Response
-
 from unstract.sdk.constants import LogLevel, PromptStudioKeys, ToolEnv
 from unstract.sdk.helper import SdkHelper
 from unstract.sdk.tool.base import BaseTool
 
 
 class PromptTool:
     """Class to handle prompt service methods for Unstract Tools."""
@@ -26,23 +24,15 @@
         """
         self.tool = tool
         self.base_url = SdkHelper.get_platform_base_url(
             prompt_host, prompt_port
         )
         self.bearer_token = tool.get_env_or_die(ToolEnv.PLATFORM_API_KEY)
 
-    def answer_prompt(self, payload: dict[str, Any]) -> dict[str, Any]:
-        return self._post_call("answer-prompt", payload)
-
-    def single_pass_extraction(self, payload: dict[str, Any]) -> dict[str, Any]:
-        return self._post_call("single-pass-extraction", payload)
-
-    def _post_call(
-        self, url_path: str, payload: dict[str, Any]
-    ) -> dict[str, Any]:
+    def answer_prompt(self, payload: dict) -> dict:
         """Invokes and communicates to prompt service to fetch response for the
         prompt.
 
         Args:
             file_name (str): File in which the prompt is processed
             outputs (dict): dict of all input data for the tool
             tool_id (str): Unique ID of the tool to be processed
@@ -52,47 +42,44 @@
             {
                 "status": "OK",
                 "error": "",
                 "cost": 0,
                 structure_output : {}
             }
         """
-        result: dict[str, Any] = {
+        result = {
             "status": "ERROR",
             "error": "",
             "cost": 0,
             "structure_output": "",
         }
-        url: str = f"{self.base_url}/{url_path}"
-        headers: dict[str, str] = {
-            "Authorization": f"Bearer {self.bearer_token}"
-        }
+        # TODO : Implement authorization for prompt service
+        # headers = {"Authorization": f"Bearer {self.bearer_token}"}
+        # Upload file to platform
+        url = f"{self.base_url}/answer-prompt"
+        headers = {"Authorization": f"Bearer {self.bearer_token}"}
         try:
-            # TODO: Review timeout value
-            response: Response = requests.post(
-                url, json=payload, headers=headers, timeout=600
-            )
-            response.raise_for_status()
-            result["status"] = "OK"
-            result["structure_output"] = response.text
-        except RequestException as e:
-            # Extract error information from the response if available
-            error_message = str(e)
-            content_type = response.headers.get("Content-Type", "").lower()
-            if "application/json" in content_type:
-                response_json = response.json()
-                if "error" in response_json:
-                    error_message = response_json["error"]
-            elif response.text:
-                error_message = response.text
-            result["error"] = error_message
+            response = requests.post(url, json=payload, headers=headers)
+            if response.status_code != 200:
+                self.tool.stream_log(
+                    f"Error while fetching response: {response.text}",
+                    level=LogLevel.ERROR,
+                )
+                result["error"] = response.text
+                return result
+            else:
+                result["status"] = "OK"
+                result["structure_output"] = response.text
+        except Exception as e:
             self.tool.stream_log(
-                f"Error while fetching response for prompt: {result['error']}",
+                f"Error while fetching response for prompt: {e}",
                 level=LogLevel.ERROR,
             )
+            result["error"] = str(e)
+            return result
         return result
 
     @staticmethod
     def get_exported_tool(
         tool: BaseTool, prompt_registry_id: str
     ) -> Optional[dict[str, Any]]:
         """Get exported custom tool by the help of unstract DB tool.
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/scripts/tool_gen.py` & `unstract_sdk-0.9.0/src/unstract/sdk/scripts/tool_gen.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/README.md` & `unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/README.md`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/config/icon.svg` & `unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/config/icon.svg`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/config/properties.json` & `unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/config/properties.json`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/static/tool_template/v1/src/main.py` & `unstract_sdk-0.9.0/src/unstract/sdk/static/tool_template/v1/src/main.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/base.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import datetime
 import json
 from abc import ABC, abstractmethod
-from json import JSONDecodeError, loads
+from json import loads
 from pathlib import Path
 from typing import Any, Union
 
 from unstract.sdk.constants import (
     Command,
     LogLevel,
     MetadataKey,
@@ -166,18 +166,14 @@
         """
         base_path: Path = self._get_data_dir()
         metadata_path = base_path / ToolExecKey.METADATA_FILE
         metadata_json = {}
         try:
             with open(metadata_path, encoding="utf-8") as f:
                 metadata_json = loads(f.read())
-        except JSONDecodeError as e:
-            self.stream_error_and_exit(
-                f"JSON decode error for {metadata_path}: {e}"
-            )
         except FileNotFoundError:
             self.stream_error_and_exit(
                 f"Metadata file not found at {metadata_path}"
             )
         except OSError as e:
             self.stream_error_and_exit(
                 f"OS Error while opening {metadata_path}: {e}"
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/entrypoint.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/entrypoint.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/executor.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/executor.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 import argparse
 import shutil
 from json import loads
 from pathlib import Path
 from typing import Any
 
-from unstract.adapters import get_adapter_version
-
 from unstract.sdk import get_sdk_version
 from unstract.sdk.constants import Command
 from unstract.sdk.tool.base import BaseTool
 from unstract.sdk.tool.validator import ToolValidator
 
 
 class ToolExecutor:
@@ -53,18 +51,17 @@
         self._setup_for_run()
 
         validator = ToolValidator(self.tool)
         settings = validator.validate_pre_execution(settings=settings)
 
         self.tool.stream_log(
             f"Running tool for "
-            f"Workflow ID: {self.tool.workflow_id}, "
-            f"Execution ID: {self.tool.execution_id}, "
-            f"SDK Version: {get_sdk_version()}, "
-            f"adapter Version: {get_adapter_version()}"
+            f"Workflow ID: {self.tool.workflow_id} "
+            f"Execution ID: {self.tool.execution_id} "
+            f"SDK Version: {get_sdk_version()}"
         )
         self.tool.run(
             settings=settings,
             input_file=self.tool.get_input_file(),
             output_dir=self.tool.get_output_dir(),
         )
         # TODO: Call tool method to validate if output was written
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/mime_types.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/mime_types.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/mixin.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/mixin.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/parser.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import argparse
 from typing import Optional
 
 from dotenv import find_dotenv, load_dotenv
-
 from unstract.sdk.constants import LogLevel
 
 
 class ToolArgsParser:
     """Class to help with parsing arguments to a tool."""
 
     @staticmethod
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/stream.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import datetime
 import json
 import os
 from typing import Any
 
 from deprecated import deprecated
-
 from unstract.sdk.constants import Command, LogLevel, LogStage, ToolEnv
 
 
 class StreamMixin:
     """Helper class for streaming Unstract tool commands.
 
     A utility class to make writing Unstract tools easier. It provides
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/tool/validator.py` & `unstract_sdk-0.9.0/src/unstract/sdk/tool/validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import re
 from json import JSONDecodeError
 from pathlib import Path
 from typing import Any
 
+import magic
 from jsonschema import Draft202012Validator, ValidationError, validators
-
 from unstract.sdk.constants import MetadataKey, PropKey
 from unstract.sdk.tool.base import BaseTool
 from unstract.sdk.tool.mime_types import EXT_MIME_MAP
-from unstract.sdk.utils import ToolUtils
 
 
 def extend_with_default(validator_class: Any) -> Any:
     """Extend a JSON schema validator class with a default value functionality.
 
     Parameters:
     - validator_class (Any): The JSON schema validator class to be extended.
@@ -208,14 +207,30 @@
         for ext in allowed_exts:
             if ext not in EXT_MIME_MAP:
                 self.tool.stream_error_and_exit(
                     f"{ext} mentioned in tool PROPERTIES is not supported"
                 )
             allowed_mimes.append(EXT_MIME_MAP[ext])
 
-        input_file_mime = ToolUtils.get_file_mime_type(input_file=input_file)
-        self.tool.stream_log(f"Input file MIME: {input_file_mime}")
+        input_file_mime = self._get_file_mime(input_file=input_file)
         if input_file_mime not in allowed_mimes:
             self.tool.stream_error_and_exit(
                 f"File type of {input_file_mime} is not supported by"
                 " the tool, check its PROPERTIES for a list of supported types"
             )
+
+    def _get_file_mime(self, input_file: Path) -> str:
+        """Gets the file MIME type for an input file. Uses libmagic to perform
+        the same.
+
+        Args:
+            input_file (Path): Path object of the input file
+
+        Returns:
+            str: MIME type of the file
+        """
+        input_file_mime = ""
+        with open(input_file, mode="rb") as input_file_obj:
+            sample_contents = input_file_obj.read(100)
+            input_file_mime = magic.from_buffer(sample_contents, mime=True)
+        self.tool.stream_log(f"Input file MIME: {input_file_mime}")
+        return input_file_mime
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/utils/callback_manager.py` & `unstract_sdk-0.9.0/src/unstract/sdk/utils/service_context.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 import logging
-from typing import Callable, Optional, Union
+from typing import Any, Callable, Optional, Union
 
 import tiktoken
-from llama_index.core.callbacks import (
-    CallbackManager as LlamaIndexCallbackManager,
-)
-from llama_index.core.callbacks import TokenCountingHandler
-from llama_index.core.embeddings import BaseEmbedding
-from llama_index.core.llms import LLM
+from llama_index import ServiceContext as LlamaIndexServiceContext
+from llama_index.callbacks import CallbackManager, TokenCountingHandler
+from llama_index.core.embeddings.base import BaseEmbedding
+from llama_index.llms import LLM
+from llama_index.llms.utils import LLMType
 from transformers import AutoTokenizer
-
 from unstract.sdk.utils.usage_handler import UsageHandler
 
 logger = logging.getLogger(__name__)
 
 
-class CallbackManager:
-    """Class representing the CallbackManager to manage callbacks.
+class ServiceContext:
+    """Class representing the UNServiceContext.
 
     Use this over the default service context of llama index
 
-    This class supports a tokenizer, token counter,
+    This class provides a static method to get the service context for
+    UNstract Tools. The service context includes a tokenizer, token counter,
     usage handler, and  callback manager.
 
     Attributes:
         None
 
     Methods:
-        set_callback_manager: Returns a standard callback manager
+        get_service_context: Returns the service context for UNstract Tools.
 
     Example:
-        callback_manager = CallbackManager.
-                            set_callback_manager(
+        service_context = UNServiceContext.
+                            get_service_context(
+                                workflow_id="123",
+                                execution_id="456",
                                 llm="default",
-                                embedding="default")
+                                embed_model="default")
     """
 
     @staticmethod
-    def set_callback_manager(
+    def get_service_context(
         platform_api_key: str,
-        llm: Optional[LLM] = None,
-        embedding: Optional[BaseEmbedding] = None,
-        **kwargs,
-    ) -> LlamaIndexCallbackManager:
-        """Sets the standard callback manager for the llm. This is to be called
-        explicitly whenever there is a need for the callback handling defined
-        here as handlers is to be invoked.
+        workflow_id: str = "",
+        execution_id: str = "",
+        llm: Optional[LLMType] = None,
+        embed_model: Optional[Any] = None,
+        **kwargs: Any,
+    ) -> LlamaIndexServiceContext:
+        """Returns the service context for UNstract Tools.
 
         Parameters:
-            llm (LLM): The LLM type
+            workflow_id (str): The workflow ID. Default is an empty string.
+            execution_id (str): The execution ID. Default is an empty string.
+            llm (Optional[LLMType]): The LLM type. Default is None.
+            embed_model (Optional[Any]): The embedding model. Default is None.
 
         Returns:
-            CallbackManager type of llama index
+            ServiceContext: The service context for UNstract Tools.
 
         Example:
-            UNCallbackManager.set_callback_manager(
-                platform_api_key: "abc",
-                llm=llm,
-                embedding=embedding
+            service_context = UNServiceContext.get_service_context(
+                workflow_id="123",
+                execution_id="456",
+                llm="default",
+                embed_model="default"
             )
         """
-
         if llm:
-            tokenizer = CallbackManager.get_tokenizer(llm)
-        elif embedding:
-            tokenizer = CallbackManager.get_tokenizer(embedding)
+            tokenizer = ServiceContext.get_tokenizer(llm)
+        elif embed_model:
+            tokenizer = ServiceContext.get_tokenizer(embed_model)
 
         token_counter = TokenCountingHandler(tokenizer=tokenizer, verbose=True)
         usage_handler = UsageHandler(
             token_counter=token_counter,
             platform_api_key=platform_api_key,
             llm_model=llm,
-            embed_model=embedding,
-            **kwargs,
+            embed_model=embed_model,
+            workflow_id=workflow_id,
+            execution_id=execution_id,
         )
 
-        callback_manager: LlamaIndexCallbackManager = LlamaIndexCallbackManager(
+        callback_manager = CallbackManager(
             handlers=[token_counter, usage_handler]
         )
-
-        if llm is not None:
-            llm.callback_manager = callback_manager
-        if embedding is not None:
-            embedding.callback_manager = callback_manager
-
-        return callback_manager
+        return LlamaIndexServiceContext.from_defaults(
+            llm=llm,
+            embed_model=embed_model,
+            callback_manager=callback_manager,
+            **kwargs,
+        )
 
     @staticmethod
     def get_tokenizer(
         model: Optional[Union[LLM, BaseEmbedding, None]],
         fallback_tokenizer: Callable[[str], list] = tiktoken.encoding_for_model(
             "gpt-3.5-turbo"
         ).encode,
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/utils/usage_handler.py` & `unstract_sdk-0.9.0/src/unstract/sdk/utils/usage_handler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional
 
-from llama_index.core.callbacks import CBEventType, TokenCountingHandler
-from llama_index.core.callbacks.base_handler import BaseCallbackHandler
-from llama_index.core.embeddings import BaseEmbedding
-from llama_index.core.llms import LLM
-
+from llama_index.callbacks import TokenCountingHandler
+from llama_index.callbacks.base_handler import BaseCallbackHandler
+from llama_index.callbacks.schema import CBEventType
+from llama_index.core.embeddings.base import BaseEmbedding
+from llama_index.llms.llm import LLM
 from unstract.sdk.audit import Audit
 from unstract.sdk.constants import LogLevel
 from unstract.sdk.tool.stream import StreamMixin
 
 
 class UsageHandler(StreamMixin, BaseCallbackHandler):
     """UsageHandler class is a subclass of BaseCallbackHandler and is
@@ -32,22 +32,24 @@
 
     def __init__(
         self,
         token_counter: TokenCountingHandler,
         platform_api_key: str,
         llm_model: LLM = None,
         embed_model: BaseEmbedding = None,
+        workflow_id: str = "",
+        execution_id: str = "",
         event_starts_to_ignore: Optional[list[CBEventType]] = None,
         event_ends_to_ignore: Optional[list[CBEventType]] = None,
         verbose: bool = False,
         log_level: LogLevel = LogLevel.INFO,
-        **kwargs,
     ) -> None:
-        self.kwargs = kwargs
         self._verbose = verbose
+        self.workflow_id = workflow_id
+        self.execution_id = execution_id
         self.token_counter = token_counter
         self.llm_model = llm_model
         self.embed_model = embed_model
         self.platform_api_key = platform_api_key
         super().__init__(
             log_level=log_level,  # StreamMixin's args
             event_starts_to_ignore=event_starts_to_ignore or [],
@@ -90,26 +92,28 @@
             model_name = self.llm_model.metadata.model_name
             # Need to push the data to via platform service
             self.stream_log(log=f"Pushing llm usage llm for model {model_name}")
             Audit(log_level=self.log_level).push_usage_data(
                 platform_api_key=self.platform_api_key,
                 token_counter=self.token_counter,
                 event_type=event_type,
-                model_name=self.llm_model.metadata.model_name,
-                **self.kwargs,
+                external_service=self.llm_model.metadata.model_name,
+                workflow_id=self.workflow_id,
+                execution_id=self.execution_id,
             )
 
         elif (
             event_type == CBEventType.EMBEDDING
             and event_type not in self.event_ends_to_ignore
             and payload is not None
         ):
             model_name = self.embed_model.model_name
             # Need to push the data to via platform service
             self.stream_log(log=f"Pushing llm usage llm for model {model_name}")
             Audit(log_level=self.log_level).push_usage_data(
                 platform_api_key=self.platform_api_key,
                 token_counter=self.token_counter,
                 event_type=event_type,
-                model_name=self.embed_model.model_name,
-                **self.kwargs,
+                external_service=self.embed_model.model_name,
+                workflow_id=self.workflow_id,
+                execution_id=self.execution_id,
             )
```

### Comparing `unstract_sdk-0.24.0/src/unstract/sdk/vector_db.py` & `unstract_sdk-0.9.0/src/unstract/sdk/vector_db.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,84 +1,81 @@
 import logging
 from typing import Union
 
-from llama_index.core.vector_stores.types import (
-    BasePydanticVectorStore,
-    VectorStore,
-)
+from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
 from unstract.adapters.constants import Common
 from unstract.adapters.vectordb import adapters
 from unstract.adapters.vectordb.constants import VectorDbConstants
-
 from unstract.sdk.adapters import ToolAdapter
-from unstract.sdk.constants import LogLevel, ToolEnv
-from unstract.sdk.exceptions import SdkError
+from unstract.sdk.constants import LogLevel, ToolEnv, ToolSettingsKey
+from unstract.sdk.exceptions import SdkException
 from unstract.sdk.platform import PlatformHelper
 from unstract.sdk.tool.base import BaseTool
 
 logger = logging.getLogger(__name__)
 
 
 class ToolVectorDB:
     """Class to handle VectorDB for Unstract Tools."""
 
-    def __init__(self, tool: BaseTool):
+    def __init__(self, tool: BaseTool, tool_settings: dict[str, str] = {}):
         self.tool = tool
         self.vector_db_adapters = adapters
+        self.vector_db_adapter_instance_id = tool_settings.get(
+            ToolSettingsKey.VECTOR_DB_ADAPTER_ID
+        )
 
     def __get_org_id(self) -> str:
         platform_helper = PlatformHelper(
             tool=self.tool,
             platform_host=self.tool.get_env_or_die(ToolEnv.PLATFORM_HOST),
             platform_port=int(self.tool.get_env_or_die(ToolEnv.PLATFORM_PORT)),
         )
         # fetch org id from bearer token
         platform_details = platform_helper.get_platform_details()
         if not platform_details:
             # Errors are logged by the SDK itself
-            raise SdkError("Error getting platform details")
+            raise SdkException("Error getting platform details")
         account_id = platform_details.get("organization_id")
         return account_id
 
     def get_vector_db(
         self, adapter_instance_id: str, embedding_dimension: int
-    ) -> Union[BasePydanticVectorStore, VectorStore]:
-        """Gets an instance of LlamaIndex's VectorStore.
-
-        Args:
-            adapter_instance_id (str): UUID of the vector DB adapter
-            embedding_dimension (int): Embedding dimension for the vector store
-
-        Returns:
-            Union[BasePydanticVectorStore, VectorStore]: Vector store instance
-        """
-        try:
-            vector_db_config = ToolAdapter.get_adapter_config(
-                self.tool, adapter_instance_id
-            )
-            vector_db_adapter_id = vector_db_config.get(Common.ADAPTER_ID)
-            if vector_db_adapter_id not in self.vector_db_adapters:
-                raise SdkError(
-                    f"VectorDB adapter not supported : "
-                    f"{vector_db_adapter_id}"
+    ) -> Union[BasePydanticVectorStore, VectorStore, None]:
+        adapter_instance_id = (
+            adapter_instance_id
+            if adapter_instance_id
+            else self.vector_db_adapter_instance_id
+        )
+        if adapter_instance_id is not None:
+            try:
+                vector_db_config = ToolAdapter.get_adapter_config(
+                    self.tool, adapter_instance_id
                 )
-
-            vector_db_adapter = self.vector_db_adapters[vector_db_adapter_id][
-                Common.METADATA
-            ][Common.ADAPTER]
-            vector_db_metadata = vector_db_config.get(Common.ADAPTER_METADATA)
-            org = self.__get_org_id()
-            # Adding the collection prefix and embedding type
-            # to the metadata
-            vector_db_metadata[VectorDbConstants.VECTOR_DB_NAME] = org
-            vector_db_metadata[
-                VectorDbConstants.EMBEDDING_DIMENSION
-            ] = embedding_dimension
-
-            vector_db_adapter_class = vector_db_adapter(vector_db_metadata)
-            return vector_db_adapter_class.get_vector_db_instance()
-        except Exception as e:
-            self.tool.stream_log(
-                log=f"Unable to get vector_db {adapter_instance_id}: {e}",
-                level=LogLevel.ERROR,
-            )
-            raise SdkError(f"Error getting vectorDB instance: {e}")
+                vector_db_adapter_id = vector_db_config.get(Common.ADAPTER_ID)
+                if vector_db_adapter_id in self.vector_db_adapters:
+                    vector_db_adapter = self.vector_db_adapters[
+                        vector_db_adapter_id
+                    ][Common.METADATA][Common.ADAPTER]
+                    vector_db_metadata = vector_db_config.get(
+                        Common.ADAPTER_METADATA
+                    )
+                    org = self.__get_org_id()
+                    # Adding the collection prefix and embedding type
+                    # to the metadata
+                    vector_db_metadata[VectorDbConstants.VECTOR_DB_NAME] = org
+                    vector_db_metadata[
+                        VectorDbConstants.EMBEDDING_DIMENSION
+                    ] = embedding_dimension
+
+                    vector_db_adapter_class = vector_db_adapter(
+                        vector_db_metadata
+                    )
+                    return vector_db_adapter_class.get_vector_db_instance()
+                else:
+                    return None
+            except Exception as e:
+                self.tool.stream_log(
+                    log=f"Unable to get vector_db {adapter_instance_id}: {e}",
+                    level=LogLevel.ERROR,
+                )
+                return None
```

### Comparing `unstract_sdk-0.24.0/tests/config/properties.json` & `unstract_sdk-0.9.0/tests/config/properties.json`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/test_cache.py` & `unstract_sdk-0.9.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/test_embedding.py` & `unstract_sdk-0.9.0/tests/test_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import json
 import os
 import unittest
 
 from dotenv import load_dotenv
-from llama_index.core.embeddings import BaseEmbedding
+from llama_index.core.embeddings.base import BaseEmbedding
 from parameterized import parameterized
-
 from unstract.sdk.embedding import ToolEmbedding
 from unstract.sdk.tool.base import BaseTool
 
 load_dotenv()
 
 
 def get_test_values(env_key: str) -> list[str]:
```

### Comparing `unstract_sdk-0.24.0/tests/test_llm.py` & `unstract_sdk-0.9.0/tests/test_llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import unittest
 from typing import Any
 
 from dotenv import load_dotenv
 from parameterized import parameterized
 from unstract.adapters.llm.helper import LLMHelper
-
 from unstract.sdk.llm import ToolLLM
 from unstract.sdk.tool.base import BaseTool
 
 load_dotenv()
 
 logger = logging.getLogger(__name__)
```

### Comparing `unstract_sdk-0.24.0/tests/test_vector_db.py` & `unstract_sdk-0.9.0/tests/test_vector_db.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 import json
 import logging
 import os
 import unittest
 
 from dotenv import load_dotenv
-from llama_index.core import MockEmbedding
-from llama_index.core.vector_stores.types import (
-    BasePydanticVectorStore,
-    VectorStore,
-)
+from llama_index import MockEmbedding
+from llama_index.vector_stores.types import BasePydanticVectorStore, VectorStore
 from parameterized import parameterized
 from unstract.adapters.vectordb.helper import VectorDBHelper
-
 from unstract.sdk.tool.base import BaseTool
 from unstract.sdk.vector_db import ToolVectorDB
 
 load_dotenv()
 
 logger = logging.getLogger(__name__)
```

### Comparing `unstract_sdk-0.24.0/tests/tool/config/icon.svg` & `unstract_sdk-0.9.0/tests/tool/config/icon.svg`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/tool/config/properties.json` & `unstract_sdk-0.9.0/tests/tool/config/properties.json`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/tool/config/spec.json` & `unstract_sdk-0.9.0/tests/tool/config/spec.json`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/tool/config/tool_properties.json` & `unstract_sdk-0.9.0/tests/tool/config/tool_properties.json`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/tool/config/tool_spec.json` & `unstract_sdk-0.9.0/tests/tool/config/tool_spec.json`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/tool/test_entrypoint.py` & `unstract_sdk-0.9.0/tests/tool/test_entrypoint.py`

 * *Files identical despite different names*

### Comparing `unstract_sdk-0.24.0/tests/tool/test_static.py` & `unstract_sdk-0.9.0/tests/tool/test_static.py`

 * *Files identical despite different names*

