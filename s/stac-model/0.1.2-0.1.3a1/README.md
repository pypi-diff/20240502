# Comparing `tmp/stac_model-0.1.2.tar.gz` & `tmp/stac_model-0.1.3a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_model-0.1.2.tar", max compression
+gzip compressed data, was "stac_model-0.1.3a1.tar", max compression
```

## Comparing `stac_model-0.1.2.tar` & `stac_model-0.1.3a1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2024-04-19 16:28:59.671806 stac_model-0.1.2/LICENSE
--rw-r--r--   0        0        0    55385 2024-04-19 16:28:59.671806 stac_model-0.1.2/README.md
--rw-r--r--   0        0        0     5300 2024-04-19 17:04:43.667216 stac_model-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      265 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/__init__.py
--rw-r--r--   0        0        0     1215 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/__main__.py
--rw-r--r--   0        0        0     3035 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/base.py
--rw-r--r--   0        0        0     7036 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/examples.py
--rw-r--r--   0        0        0     2026 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/input.py
--rw-r--r--   0        0        0     3007 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/output.py
--rw-r--r--   0        0        0     1476 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/runtime.py
--rw-r--r--   0        0        0     9406 2024-04-19 16:28:59.671806 stac_model-0.1.2/stac_model/schema.py
--rw-r--r--   0        0        0    57086 1970-01-01 00:00:00.000000 stac_model-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-01 23:25:28.057036 stac_model-0.1.3a1/LICENSE
+-rw-r--r--   0        0        0    56030 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/README.md
+-rw-r--r--   0        0        0     7476 2024-05-02 20:48:44.991630 stac_model-0.1.3a1/pyproject.toml
+-rw-r--r--   0        0        0      265 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/__init__.py
+-rw-r--r--   0        0        0     1215 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/__main__.py
+-rw-r--r--   0        0        0     3035 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/base.py
+-rw-r--r--   0        0        0     7036 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/examples.py
+-rw-r--r--   0        0        0     2026 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/input.py
+-rw-r--r--   0        0        0     3007 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/output.py
+-rw-r--r--   0        0        0     1476 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/runtime.py
+-rw-r--r--   0        0        0     9408 2024-05-01 23:25:28.061036 stac_model-0.1.3a1/stac_model/schema.py
+-rw-r--r--   0        0        0    57733 1970-01-01 00:00:00.000000 stac_model-0.1.3a1/PKG-INFO
```

### Comparing `stac_model-0.1.2/LICENSE` & `stac_model-0.1.3a1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/README.md` & `stac_model-0.1.3a1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Machine Learning Model Extension Specification
 
-[![hackmd-github-sync-badge](https://hackmd.io/lekSD_RVRiquNHRloXRzeg/badge)](https://hackmd.io/lekSD_RVRiquNHRloXRzeg?both)
+[![hackmd-github-sync-badge](https://hackmd.io/N1cWyDM2S9eaAQtSvS0J_A/badge)](https://hackmd.io/N1cWyDM2S9eaAQtSvS0J_A?both)
 
 - **Title:** Machine Learning Model Extension
-- **Identifier:** [https://stac-extensions.github.io/mlm/v1.0.0/schema.json](https://stac-extensions.github.io/mlm/v1.0.0/schema.json)
+- **Identifier:** [https://crim-ca.github.io/mlm-extension/v1.1.0/schema.json](https://crim-ca.github.io/mlm-extension/v1.1.0/schema.json)
 - **Field Name Prefix:** mlm
 - **Scope:** Collection, Item, Asset, Links
-- **Extension Maturity Classification:** Proposal
+- **Extension Maturity Classification:** Pilot
 - **Owner:**
   - [@fmigneault](https://github.com/fmigneault)
   - [@rbavery](https://github.com/rbavery)
   - [@ymoisan](https://github.com/ymoisan)
   - [@sfoucher](https://github.com/sfoucher)
 
 The STAC Machine Learning Model (MLM) Extension provides a standard set of fields to describe machine learning models
@@ -61,20 +61,22 @@
 ## Item Properties and Collection Fields
 
 The fields in the table below can be used in these parts of STAC documents:
 
 - [ ] Catalogs
 - [x] Collections
 - [x] Item Properties (incl. Summaries in Collections)
-- [x] Assets (for both Collections and Items, incl. Item Asset Definitions in Collections, except `mlm:name`)
+- [x] Assets (for both Collections and Items, incl. [Item-Assets][item-assets] definitions in Collections)
 - [ ] Links
 
+[item-assets]: https://github.com/stac-extensions/item-assets
+
 | Field Name                  | Type                                                          | Description                                                                                                                                                                                                                                                                                 |
 |-----------------------------|---------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| mlm:name                    | string                                                        | **REQUIRED** A unique name for the model. This can include, but must be distinct, from simply naming the model architecture. If there is a publication or other published work related to the model, use the official name of the model.                                                    |
+| mlm:name                    | string                                                        | **REQUIRED** A name for the model. This can include, but must be distinct, from simply naming the model architecture. If there is a publication or other published work related to the model, use the official name of the model.                                                    |
 | mlm:architecture            | [Model Architecture](#model-architecture) string              | **REQUIRED** A generic and well established architecture name of the model.                                                                                                                                                                                                                 | 
 | mlm:tasks                   | \[[Task Enum](#task-enum)]                                    | **REQUIRED** Specifies the Machine Learning tasks for which the model can be used for. If multi-tasks outputs are provided by distinct model heads, specify all available tasks under the main properties and specify respective tasks in each [Model Output Object](#model-output-object). |
 | mlm:framework               | string                                                        | Framework used to train the model (ex: PyTorch, TensorFlow).                                                                                                                                                                                                                   |
 | mlm:framework_version       | string                                                        | The `framework` library version. Some models require a specific version of the machine learning `framework` to run.                                                                                                                                                                         |
 | mlm:memory_size             | integer                                                       | The in-memory size of the model on the accelerator during inference (bytes).                                                                                                                                                                                                                |
 | mlm:total_parameters        | integer                                                       | Total number of model parameters, including trainable and non-trainable parameters.                                                                                                                                                                                                         |
 | mlm:pretrained              | boolean                                                       | Indicates if the model was pretrained. If the model was pretrained, consider providing `pretrained_source` if it is known.                                                                                                                                                                  |
@@ -165,16 +167,16 @@
 
 This should correspond to the common library name of a well-established ML framework.
 No "Enum" are *enforced* to allow easy addition of newer frameworks, but it is **STRONGLY** recommended
 to use common names when applicable. Below are a few notable entries.
 
 - `PyTorch`
 - `TensorFlow`
-- `Scikit-learn`
-- `Huggingface`
+- `scikit-learn`
+- `Hugging Face`
 - `Keras`
 - `ONNX`
 - `rgee`
 - `spatialRF`
 - `JAX`
 - `MXNet`
 - `Caffe`
@@ -205,17 +207,18 @@
 set to `true`, there would be no `accelerator` to contain against. To avoid confusion, it is suggested to set the
 `mlm:accelerator_constrained = false` or omit the field entirely in this case.
 
 ### Model Input Object
 
 | Field Name              | Type                                                    | Description                                                                                                                                                                                                                                   |
 |-------------------------|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| name                    | string                                                  | **REQUIRED** Name of the input variable defined by the model. If no explicit name is defined by the model, an informative name (e.g.: `"RGB Time Series"`) can be used instead.                                                                 | 
+| name                    | string                                                  | **REQUIRED** Name of the input variable defined by the model. If no explicit name is defined by the model, an informative name (e.g.: `"RGB Time Series"`) can be used instead.                                                               | 
 | bands                   | \[string]                                               | **REQUIRED** The names of the raster bands used to train or fine-tune the model, which may be all or a subset of bands available in a STAC Item's [Band Object](#bands-and-statistics). If no band applies for one input, use an empty array. |
 | input                   | [Input Structure Object](#input-structure-object)       | **REQUIRED** The N-dimensional array definition that describes the shape, dimension ordering, and data type.                                                                                                                                  |
+| description             | string                                                  | Additional details about the input such as describing its purpose or expected source that cannot be represented by other properties.                                                                                                          | 
 | norm_by_channel         | boolean                                                 | Whether to normalize each channel by channel-wise statistics or to normalize by dataset statistics. If True, use an array of `statistics` of same dimensionality and order as the `bands` field in this object.                               |
 | norm_type               | [Normalize Enum](#normalize-enum) \| null               | Normalization method. Select an appropriate option or `null` when none applies. Consider using `pre_processing_function` for custom implementations or more complex combinations.                                                             |
 | norm_clip               | \[number]                                               | When `norm_type = "clip"`, this array supplies the value for each `bands` item, which is used to divide each band before clipping values between 0 and 1.                                                                                     |
 | resize_type             | [Resize Enum](#resize-enum) \| null                     | High-level descriptor of the rescaling method to change image shape. Select an appropriate option or `null` when none applies. Consider using `pre_processing_function` for custom implementations or more complex combinations.              |
 | statistics              | \[[Statistics Object](#bands-and-statistics)]           | Dataset statistics for the training dataset used to normalize the inputs.                                                                                                                                                                     |
 | pre_processing_function | [Processing Expression](#processing-expression) \| null | Custom preprocessing function where normalization and rescaling, and any other significant operations takes place.                                                                                                                            |
 
@@ -396,14 +399,15 @@
 ### Model Output Object
 
 | Field Name               | Type                                                    | Description                                                                                                                                                                     |
 |--------------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | name                     | string                                                  | **REQUIRED** Name of the output variable defined by the model. If no explicit name is defined by the model, an informative name (e.g.: `"CLASSIFICATION"`) can be used instead. |
 | tasks                    | \[[Task Enum](#task-enum)]                              | **REQUIRED** Specifies the Machine Learning tasks for which the output can be used for. This can be a subset of `mlm:tasks` defined under the Item `properties` as applicable.  |
 | result                   | [Result Structure Object](#result-structure-object)     | **REQUIRED** The structure that describes the resulting output arrays/tensors from one model head.                                                                              |
+| description              | string                                                  | Additional details about the output such as describing its purpose or expected result that cannot be represented by other properties.                                           |
 | classification:classes   | \[[Class Object](#class-object)]                        | A list of class objects adhering to the [Classification Extension](https://github.com/stac-extensions/classification).                                                          |
 | post_processing_function | [Processing Expression](#processing-expression) \| null | Custom postprocessing function where normalization and rescaling, and any other significant operations takes place.                                                             |
 
 While only `tasks` is a required field, all fields are recommended for tasks that produce a fixed
 shape tensor and have output classes. Outputs that have variable dimensions, can define the `result` with the
 appropriate dimension value `-1` in the `shape` field. When the model does not produce specific classes, such 
 as for `regression`, `image-captioning`, `super-resolution` and some `generative` tasks, to name a few, the
```

### Comparing `stac_model-0.1.2/pyproject.toml` & `stac_model-0.1.3a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "stac-model"
-version = "0.1.2"
+version = "0.1.3-alpha.1"
 description = "A PydanticV2 validation and serialization libary for the STAC ML Model Extension"
 readme = "README.md"
 authors = ["Ryan Avery <ryan@wherobots.com>"]
 license = "Apache Software License 2.0"
 repository = "https://github.com/rbavery/stac-model"
 homepage = "https://github.com/rbavery/stac-model"
 packages = [
@@ -78,14 +78,107 @@
 pytest-timeout = "^2.2.0"
 pytest-benchmark = "^4.0.0"
 pytest-sugar = "^0.9.7"
 pytest-click = "^1.1.0"
 pytest-pikachu = "^1.0.0"
 coverage = "^7.3.0"
 ruff = "^0.2.2"
+bump-my-version = "^0.21"
+
+[tool.bumpversion]
+current_version = "1.1.0"
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)"
+serialize = ["{major}.{minor}.{patch}"]
+search = "{current_version}"
+replace = "{new_version}"
+regex = false
+ignore_missing_version = true
+ignore_missing_files = false
+tag = true
+sign_tags = false
+tag_name = "v{new_version}"
+tag_message = "Bump version: {current_version} → {new_version}"
+allow_dirty = false
+commit = true
+commit_args = "--no-verify"
+message = "Bump version: {current_version} → {new_version}"
+
+[[tool.bumpversion.files]]
+glob = "**/*.json"
+glob_exclude = [
+  ".git/**",
+  "**/__pycache__/**",
+  ".mypy_cache/**",
+  ".tox/**",
+  ".venv/**",
+  "_build/**",
+  "build/**",
+  "dist/**",
+  "node_modules/**",
+]
+search = "https://crim-ca.github.io/mlm-extension/v{current_version}/schema.json"
+replace = "https://crim-ca.github.io/mlm-extension/v{new_version}/schema.json"
+
+[[tool.bumpversion.files]]
+glob = "**/*.md"
+glob_exclude = [
+  ".git/**",
+  "**/__pycache__/**",
+  ".mypy_cache/**",
+  ".tox/**",
+  ".venv/**",
+  "_build/**",
+  "build/**",
+  "dist/**",
+  "node_modules/**",
+]
+search = "https://crim-ca.github.io/mlm-extension/v{current_version}/schema.json"
+replace = "https://crim-ca.github.io/mlm-extension/v{new_version}/schema.json"
+
+[[tool.bumpversion.files]]
+glob = "**/*.py"
+glob_exclude = [
+  ".git/**",
+  "**/__pycache__/**",
+  ".mypy_cache/**",
+  ".tox/**",
+  ".venv/**",
+  "_build/**",
+  "build/**",
+  "dist/**",
+  "node_modules/**",
+]
+search = "https://crim-ca.github.io/mlm-extension/v{current_version}/schema.json"
+replace = "https://crim-ca.github.io/mlm-extension/v{new_version}/schema.json"
+
+[[tool.bumpversion.files]]
+filename = "CHANGELOG.md"
+search = """
+## [Unreleased](https://github.com/crim-ca/mlm-extension/tree/main)
+"""
+replace = """
+## [Unreleased](https://github.com/crim-ca/mlm-extension/tree/main)
+
+### Added
+- n/a
+
+### Changed
+- n/a
+
+### Deprecated
+- n/a
+
+### Removed
+- n/a
+
+### Fixed
+- n/a
+
+## [v{new_version}](https://github.com/crim-ca/mlm-extension/tree/v{new_version})
+"""
 
 [tool.ruff]
 exclude = [
     ".git",
     "__pycache__",
     ".mypy_cache",
     ".tox",
@@ -114,14 +207,18 @@
     "B",
     # flake8-simplify
     "SIM",
     # isort
     "I",
 ]
 
+[tool.ruff.lint.isort]
+known-local-folder = ["tests", "conftest"]
+known-first-party = ["stac_model"]
+
 [tool.mypy]
 # https://github.com/python/mypy
 # https://mypy.readthedocs.io/en/latest/config_file.html#using-a-pyproject-toml-file
 python_version = "3.10"
 pretty = true
 show_traceback = true
 color_output = true
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `stac_model-0.1.2/stac_model/__main__.py` & `stac_model-0.1.3a1/stac_model/__main__.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/stac_model/base.py` & `stac_model-0.1.3a1/stac_model/base.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/stac_model/examples.py` & `stac_model-0.1.3a1/stac_model/examples.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/stac_model/input.py` & `stac_model-0.1.3a1/stac_model/input.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/stac_model/output.py` & `stac_model-0.1.3a1/stac_model/output.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/stac_model/runtime.py` & `stac_model-0.1.3a1/stac_model/runtime.py`

 * *Files identical despite different names*

### Comparing `stac_model-0.1.2/stac_model/schema.py` & `stac_model-0.1.3a1/stac_model/schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     "T",
     pystac.Collection,
     pystac.Item,
     pystac.Asset,  # item_assets.AssetDefinition,
 )
 
 SchemaName = Literal["mlm"]
-SCHEMA_URI: str = "https://stac-extensions.github.io/mlm/v1.0.0/schema.json"
+SCHEMA_URI: str = "https://crim-ca.github.io/mlm-extension/v1.1.0/schema.json"
 PREFIX = f"{get_args(SchemaName)[0]}:"
 
 
 def mlm_prefix_adder(field_name: str) -> str:
     return "mlm:" + field_name
```

### Comparing `stac_model-0.1.2/PKG-INFO` & `stac_model-0.1.3a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-model
-Version: 0.1.2
+Version: 0.1.3a1
 Summary: A PydanticV2 validation and serialization libary for the STAC ML Model Extension
 Home-page: https://github.com/rbavery/stac-model
 License: Apache Software License 2.0
 Author: Ryan Avery
 Author-email: ryan@wherobots.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -34,21 +34,21 @@
 Requires-Dist: shapely (>=2,<3)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Project-URL: Repository, https://github.com/rbavery/stac-model
 Description-Content-Type: text/markdown
 
 # Machine Learning Model Extension Specification
 
-[![hackmd-github-sync-badge](https://hackmd.io/lekSD_RVRiquNHRloXRzeg/badge)](https://hackmd.io/lekSD_RVRiquNHRloXRzeg?both)
+[![hackmd-github-sync-badge](https://hackmd.io/N1cWyDM2S9eaAQtSvS0J_A/badge)](https://hackmd.io/N1cWyDM2S9eaAQtSvS0J_A?both)
 
 - **Title:** Machine Learning Model Extension
-- **Identifier:** [https://stac-extensions.github.io/mlm/v1.0.0/schema.json](https://stac-extensions.github.io/mlm/v1.0.0/schema.json)
+- **Identifier:** [https://crim-ca.github.io/mlm-extension/v1.1.0/schema.json](https://crim-ca.github.io/mlm-extension/v1.1.0/schema.json)
 - **Field Name Prefix:** mlm
 - **Scope:** Collection, Item, Asset, Links
-- **Extension Maturity Classification:** Proposal
+- **Extension Maturity Classification:** Pilot
 - **Owner:**
   - [@fmigneault](https://github.com/fmigneault)
   - [@rbavery](https://github.com/rbavery)
   - [@ymoisan](https://github.com/ymoisan)
   - [@sfoucher](https://github.com/sfoucher)
 
 The STAC Machine Learning Model (MLM) Extension provides a standard set of fields to describe machine learning models
@@ -99,20 +99,22 @@
 ## Item Properties and Collection Fields
 
 The fields in the table below can be used in these parts of STAC documents:
 
 - [ ] Catalogs
 - [x] Collections
 - [x] Item Properties (incl. Summaries in Collections)
-- [x] Assets (for both Collections and Items, incl. Item Asset Definitions in Collections, except `mlm:name`)
+- [x] Assets (for both Collections and Items, incl. [Item-Assets][item-assets] definitions in Collections)
 - [ ] Links
 
+[item-assets]: https://github.com/stac-extensions/item-assets
+
 | Field Name                  | Type                                                          | Description                                                                                                                                                                                                                                                                                 |
 |-----------------------------|---------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| mlm:name                    | string                                                        | **REQUIRED** A unique name for the model. This can include, but must be distinct, from simply naming the model architecture. If there is a publication or other published work related to the model, use the official name of the model.                                                    |
+| mlm:name                    | string                                                        | **REQUIRED** A name for the model. This can include, but must be distinct, from simply naming the model architecture. If there is a publication or other published work related to the model, use the official name of the model.                                                    |
 | mlm:architecture            | [Model Architecture](#model-architecture) string              | **REQUIRED** A generic and well established architecture name of the model.                                                                                                                                                                                                                 | 
 | mlm:tasks                   | \[[Task Enum](#task-enum)]                                    | **REQUIRED** Specifies the Machine Learning tasks for which the model can be used for. If multi-tasks outputs are provided by distinct model heads, specify all available tasks under the main properties and specify respective tasks in each [Model Output Object](#model-output-object). |
 | mlm:framework               | string                                                        | Framework used to train the model (ex: PyTorch, TensorFlow).                                                                                                                                                                                                                   |
 | mlm:framework_version       | string                                                        | The `framework` library version. Some models require a specific version of the machine learning `framework` to run.                                                                                                                                                                         |
 | mlm:memory_size             | integer                                                       | The in-memory size of the model on the accelerator during inference (bytes).                                                                                                                                                                                                                |
 | mlm:total_parameters        | integer                                                       | Total number of model parameters, including trainable and non-trainable parameters.                                                                                                                                                                                                         |
 | mlm:pretrained              | boolean                                                       | Indicates if the model was pretrained. If the model was pretrained, consider providing `pretrained_source` if it is known.                                                                                                                                                                  |
@@ -203,16 +205,16 @@
 
 This should correspond to the common library name of a well-established ML framework.
 No "Enum" are *enforced* to allow easy addition of newer frameworks, but it is **STRONGLY** recommended
 to use common names when applicable. Below are a few notable entries.
 
 - `PyTorch`
 - `TensorFlow`
-- `Scikit-learn`
-- `Huggingface`
+- `scikit-learn`
+- `Hugging Face`
 - `Keras`
 - `ONNX`
 - `rgee`
 - `spatialRF`
 - `JAX`
 - `MXNet`
 - `Caffe`
@@ -243,17 +245,18 @@
 set to `true`, there would be no `accelerator` to contain against. To avoid confusion, it is suggested to set the
 `mlm:accelerator_constrained = false` or omit the field entirely in this case.
 
 ### Model Input Object
 
 | Field Name              | Type                                                    | Description                                                                                                                                                                                                                                   |
 |-------------------------|---------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
-| name                    | string                                                  | **REQUIRED** Name of the input variable defined by the model. If no explicit name is defined by the model, an informative name (e.g.: `"RGB Time Series"`) can be used instead.                                                                 | 
+| name                    | string                                                  | **REQUIRED** Name of the input variable defined by the model. If no explicit name is defined by the model, an informative name (e.g.: `"RGB Time Series"`) can be used instead.                                                               | 
 | bands                   | \[string]                                               | **REQUIRED** The names of the raster bands used to train or fine-tune the model, which may be all or a subset of bands available in a STAC Item's [Band Object](#bands-and-statistics). If no band applies for one input, use an empty array. |
 | input                   | [Input Structure Object](#input-structure-object)       | **REQUIRED** The N-dimensional array definition that describes the shape, dimension ordering, and data type.                                                                                                                                  |
+| description             | string                                                  | Additional details about the input such as describing its purpose or expected source that cannot be represented by other properties.                                                                                                          | 
 | norm_by_channel         | boolean                                                 | Whether to normalize each channel by channel-wise statistics or to normalize by dataset statistics. If True, use an array of `statistics` of same dimensionality and order as the `bands` field in this object.                               |
 | norm_type               | [Normalize Enum](#normalize-enum) \| null               | Normalization method. Select an appropriate option or `null` when none applies. Consider using `pre_processing_function` for custom implementations or more complex combinations.                                                             |
 | norm_clip               | \[number]                                               | When `norm_type = "clip"`, this array supplies the value for each `bands` item, which is used to divide each band before clipping values between 0 and 1.                                                                                     |
 | resize_type             | [Resize Enum](#resize-enum) \| null                     | High-level descriptor of the rescaling method to change image shape. Select an appropriate option or `null` when none applies. Consider using `pre_processing_function` for custom implementations or more complex combinations.              |
 | statistics              | \[[Statistics Object](#bands-and-statistics)]           | Dataset statistics for the training dataset used to normalize the inputs.                                                                                                                                                                     |
 | pre_processing_function | [Processing Expression](#processing-expression) \| null | Custom preprocessing function where normalization and rescaling, and any other significant operations takes place.                                                                                                                            |
 
@@ -434,14 +437,15 @@
 ### Model Output Object
 
 | Field Name               | Type                                                    | Description                                                                                                                                                                     |
 |--------------------------|---------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | name                     | string                                                  | **REQUIRED** Name of the output variable defined by the model. If no explicit name is defined by the model, an informative name (e.g.: `"CLASSIFICATION"`) can be used instead. |
 | tasks                    | \[[Task Enum](#task-enum)]                              | **REQUIRED** Specifies the Machine Learning tasks for which the output can be used for. This can be a subset of `mlm:tasks` defined under the Item `properties` as applicable.  |
 | result                   | [Result Structure Object](#result-structure-object)     | **REQUIRED** The structure that describes the resulting output arrays/tensors from one model head.                                                                              |
+| description              | string                                                  | Additional details about the output such as describing its purpose or expected result that cannot be represented by other properties.                                           |
 | classification:classes   | \[[Class Object](#class-object)]                        | A list of class objects adhering to the [Classification Extension](https://github.com/stac-extensions/classification).                                                          |
 | post_processing_function | [Processing Expression](#processing-expression) \| null | Custom postprocessing function where normalization and rescaling, and any other significant operations takes place.                                                             |
 
 While only `tasks` is a required field, all fields are recommended for tasks that produce a fixed
 shape tensor and have output classes. Outputs that have variable dimensions, can define the `result` with the
 appropriate dimension value `-1` in the `shape` field. When the model does not produce specific classes, such 
 as for `regression`, `image-captioning`, `super-resolution` and some `generative` tasks, to name a few, the
```

