# Comparing `tmp/airbyte-source-wrike-0.2.0.tar.gz` & `tmp/airbyte_source_wrike-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte-source-wrike-0.2.0.tar", last modified: Thu Feb  1 09:45:44 2024, max compression
+gzip compressed data, was "airbyte_source_wrike-0.2.1.tar", max compression
```

## Comparing `airbyte-source-wrike-0.2.0.tar` & `airbyte_source_wrike-0.2.1.tar`

### file list

```diff
@@ -1,33 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:45:44.537717 airbyte-source-wrike-0.2.0/
--rw-r--r--   0 root         (0) root         (0)     4152 2024-02-01 09:45:44.537717 airbyte-source-wrike-0.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3979 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:45:44.537717 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4152 2024-02-01 09:45:44.000000 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      876 2024-02-01 09:45:44.000000 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-02-01 09:45:44.000000 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       54 2024-02-01 09:45:44.000000 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       78 2024-02-01 09:45:44.000000 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-02-01 09:45:44.000000 airbyte-source-wrike-0.2.0/airbyte_source_wrike.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:45:44.533717 airbyte-source-wrike-0.2.0/integration_tests/
--rw-r--r--   0 root         (0) root         (0)       61 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      584 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/abnormal_state.json
--rw-r--r--   0 root         (0) root         (0)      435 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/acceptance.py
--rw-r--r--   0 root         (0) root         (0)     1355 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/configured_catalog.json
--rw-r--r--   0 root         (0) root         (0)      128 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/invalid_config.json
--rw-r--r--   0 root         (0) root         (0)      129 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/sample_config.json
--rw-r--r--   0 root         (0) root         (0)       63 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/integration_tests/sample_state.json
--rw-r--r--   0 root         (0) root         (0)     4017 2024-02-01 09:45:44.537717 airbyte-source-wrike-0.2.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      903 2024-02-01 09:45:42.000000 airbyte-source-wrike-0.2.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:45:44.537717 airbyte-source-wrike-0.2.0/source_wrike/
--rw-r--r--   0 root         (0) root         (0)      122 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2159 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/manifest.yaml
--rw-r--r--   0 root         (0) root         (0)      227 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/run.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-02-01 09:45:44.537717 airbyte-source-wrike-0.2.0/source_wrike/schemas/
--rw-r--r--   0 root         (0) root         (0)      543 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/schemas/comments.json
--rw-r--r--   0 root         (0) root         (0)     1596 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/schemas/contacts.json
--rw-r--r--   0 root         (0) root         (0)     1401 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/schemas/customfields.json
--rw-r--r--   0 root         (0) root         (0)     1050 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/schemas/folders.json
--rw-r--r--   0 root         (0) root         (0)     1974 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/schemas/tasks.json
--rw-r--r--   0 root         (0) root         (0)     1095 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/schemas/workflows.json
--rw-r--r--   0 root         (0) root         (0)      474 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/source.py
--rw-r--r--   0 root         (0) root         (0)     1075 2024-02-01 09:38:30.000000 airbyte-source-wrike-0.2.0/source_wrike/spec.yaml
+-rw-r--r--   0        0        0     3979 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/README.md
+-rw-r--r--   0        0        0      731 2024-05-02 09:38:15.538648 airbyte_source_wrike-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/__init__.py
+-rw-r--r--   0        0        0     2158 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/run.py
+-rw-r--r--   0        0        0      543 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/comments.json
+-rw-r--r--   0        0        0     1596 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/contacts.json
+-rw-r--r--   0        0        0     1401 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/customfields.json
+-rw-r--r--   0        0        0     1050 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/folders.json
+-rw-r--r--   0        0        0     1974 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/tasks.json
+-rw-r--r--   0        0        0     1099 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/schemas/workflows.json
+-rw-r--r--   0        0        0      474 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/source.py
+-rw-r--r--   0        0        0     1075 2024-05-02 09:23:08.000000 airbyte_source_wrike-0.2.1/source_wrike/spec.yaml
+-rw-r--r--   0        0        0     4678 1970-01-01 00:00:00.000000 airbyte_source_wrike-0.2.1/PKG-INFO
```

### Comparing `airbyte-source-wrike-0.2.0/PKG-INFO` & `airbyte_source_wrike-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,67 @@
-Metadata-Version: 2.1
-Name: airbyte-source-wrike
-Version: 0.2.0
-Summary: Source implementation for Wrike.
-Author: Airbyte
-Author-email: contact@airbyte.io
-Description-Content-Type: text/markdown
-Requires-Dist: airbyte-cdk~=0.1
-Provides-Extra: tests
-Requires-Dist: requests-mock~=1.9.3; extra == "tests"
-Requires-Dist: pytest~=6.2; extra == "tests"
-Requires-Dist: pytest-mock~=3.6.1; extra == "tests"
-
 # Wrike Source
 
 This is the repository for the Wrike configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/wrike).
 
+## Local development
 
+#### Create credentials
 **If you are a community contributor**, follow the instructions in the [documentation](https://docs.airbyte.com/integrations/sources/wrike)
 to generate the necessary credentials. Then create a file `secrets/config.json` conforming to the `source_wrike/spec.yaml` file.
 Note that any directory named `secrets` is gitignored across the entire Airbyte repo, so there is no danger of accidentally checking in sensitive information.
 See `integration_tests/sample_config.json` for a sample config file.
 
 **If you are an Airbyte core member**, copy the credentials in Lastpass under the secret name `source wrike test creds`
 and place them into `secrets/config.json`.
 
+### Locally running the connector docker image
 
 
+#### Build
 **Via [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md) (recommended):**
 ```bash
 airbyte-ci connectors --name=source-wrike build
 ```
 
 An image will be built with the tag `airbyte/source-wrike:dev`.
 
 **Via `docker build`:**
 ```bash
 docker build -t airbyte/source-wrike:dev .
 ```
 
+#### Run
 Then run any of the connector commands as follows:
 ```
 docker run --rm airbyte/source-wrike:dev spec
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-wrike:dev check --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets airbyte/source-wrike:dev discover --config /secrets/config.json
 docker run --rm -v $(pwd)/secrets:/secrets -v $(pwd)/integration_tests:/integration_tests airbyte/source-wrike:dev read --config /secrets/config.json --catalog /integration_tests/configured_catalog.json
 ```
 
+## Testing
 You can run our full test suite locally using [`airbyte-ci`](https://github.com/airbytehq/airbyte/blob/master/airbyte-ci/connectors/pipelines/README.md):
 ```bash
 airbyte-ci connectors --name=source-wrike test
 ```
 
+### Customizing acceptance Tests
 Customize `acceptance-test-config.yml` file to configure tests. See [Connector Acceptance Tests](https://docs.airbyte.com/connector-development/testing-connectors/connector-acceptance-tests-reference) for more information.
 If your connector requires to create or destroy resources for use during acceptance tests create fixtures for it and place them inside integration_tests/acceptance.py.
 
+## Dependency Management
 All of your dependencies should go in `setup.py`, NOT `requirements.txt`. The requirements file is only used to connect internal Airbyte dependencies in the monorepo for local development.
 We split dependencies between two groups, dependencies that are:
 * required for your connector to work need to go to `MAIN_REQUIREMENTS` list.
 * required for the testing need to go to `TEST_REQUIREMENTS` list
 
+### Publishing a new version of the connector
 You've checked out the repo, implemented a million dollar feature, and you're ready to share your changes with the world. Now what?
 1. Make sure your changes are passing our test suite: `airbyte-ci connectors --name=source-wrike test`
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/wrike.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
+
```

### Comparing `airbyte-source-wrike-0.2.0/README.md` & `airbyte_source_wrike-0.2.1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: airbyte-source-wrike
+Version: 0.2.1
+Summary: Source implementation for Wrike.
+Home-page: https://airbyte.com
+License: MIT
+Author: Airbyte
+Author-email: contact@airbyte.io
+Requires-Python: >=3.9,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: airbyte-cdk (>=0,<1)
+Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/wrike
+Project-URL: Repository, https://github.com/airbytehq/airbyte
+Description-Content-Type: text/markdown
+
 # Wrike Source
 
 This is the repository for the Wrike configuration based source connector.
 For information about how to use this connector within Airbyte, see [the documentation](https://docs.airbyte.com/integrations/sources/wrike).
 
 ## Local development
 
@@ -61,7 +80,8 @@
 2. Bump the connector version in `metadata.yaml`: increment the `dockerImageTag` value. Please follow [semantic versioning for connectors](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#semantic-versioning-for-connectors).
 3. Make sure the `metadata.yaml` content is up to date.
 4. Make the connector documentation and its changelog is up to date (`docs/integrations/sources/wrike.md`).
 5. Create a Pull Request: use [our PR naming conventions](https://docs.airbyte.com/contributing-to-airbyte/resources/pull-requests-handbook/#pull-request-title-convention).
 6. Pat yourself on the back for being an awesome contributor.
 7. Someone from Airbyte will take a look at your PR and iterate with you to merge it into master.
 
+
```

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/manifest.yaml` & `airbyte_source_wrike-0.2.1/source_wrike/manifest.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-version: "0.29.0"
+version: "0.85.0"
 
 definitions:
   selector:
     type: RecordSelector
     extractor:
       type: DpathExtractor
       field_path: ["data"]
@@ -15,15 +15,15 @@
       type: BearerAuthenticator
       api_token: "{{ config['access_token'] }}"
 
   base_paginator:
     type: "DefaultPaginator"
     pagination_strategy:
       type: "CursorPagination"
-      cursor_value: "{{ last_records['nextPageToken'] }}"
+      cursor_value: "{{ last_record['nextPageToken'] }}"
     page_token_option:
       type: "RequestPath"
       field_name: "nextPageToken"
       inject_into: "request_parameter"
 
   retriever:
     type: SimpleRetriever
```

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/schemas/comments.json` & `airbyte_source_wrike-0.2.1/source_wrike/schemas/comments.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/schemas/contacts.json` & `airbyte_source_wrike-0.2.1/source_wrike/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/schemas/customfields.json` & `airbyte_source_wrike-0.2.1/source_wrike/schemas/customfields.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/schemas/folders.json` & `airbyte_source_wrike-0.2.1/source_wrike/schemas/folders.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/schemas/tasks.json` & `airbyte_source_wrike-0.2.1/source_wrike/schemas/tasks.json`

 * *Files identical despite different names*

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/schemas/workflows.json` & `airbyte_source_wrike-0.2.1/source_wrike/schemas/workflows.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9930245535714286%*

 * *Differences: {"'properties'": "{'standard': {'type': {insert: [(0, 'boolean')], delete: [0]}}, 'hidden': "*

 * *                 "{'type': {insert: [(0, 'boolean')], delete: [0]}}, 'customStatuses': {'items': "*

 * *                 "{'properties': {'standard': {'type': {insert: [(0, 'boolean')], delete: [0]}}, "*

 * *                 "'hidden': {'type': {insert: [(0, 'boolean')], delete: [0]}}}}}}"}*

```diff
@@ -15,15 +15,15 @@
                         "type": [
                             "string",
                             "null"
                         ]
                     },
                     "hidden": {
                         "type": [
-                            "string",
+                            "boolean",
                             "null"
                         ]
                     },
                     "id": {
                         "type": [
                             "string",
                             "null"
@@ -33,15 +33,15 @@
                         "type": [
                             "string",
                             "null"
                         ]
                     },
                     "standard": {
                         "type": [
-                            "string",
+                            "boolean",
                             "null"
                         ]
                     },
                     "standardName": {
                         "type": [
                             "boolean",
                             "null"
@@ -56,15 +56,15 @@
             "type": [
                 "array",
                 "null"
             ]
         },
         "hidden": {
             "type": [
-                "string",
+                "boolean",
                 "null"
             ]
         },
         "id": {
             "type": [
                 "string",
                 "null"
@@ -74,15 +74,15 @@
             "type": [
                 "string",
                 "null"
             ]
         },
         "standard": {
             "type": [
-                "string",
+                "boolean",
                 "null"
             ]
         },
         "title": {
             "type": [
                 "string",
                 "null"
```

### Comparing `airbyte-source-wrike-0.2.0/source_wrike/spec.yaml` & `airbyte_source_wrike-0.2.1/source_wrike/spec.yaml`

 * *Files identical despite different names*

