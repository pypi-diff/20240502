# Comparing `tmp/openai_messages_token_helper-0.1.1.tar.gz` & `tmp/openai_messages_token_helper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_messages_token_helper-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai_messages_token_helper-0.1.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai_messages_token_helper-0.1.1.tar` & `openai_messages_token_helper-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      967 2024-05-02 10:25:36.174822 openai_messages_token_helper-0.1.1/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.1/.gitignore
--rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.1/.vscode/launch.json
--rw-r--r--   0        0        0      323 2024-05-02 10:25:36.179140 openai_messages_token_helper-0.1.1/.vscode/settings.json
--rw-r--r--   0        0        0     1620 2024-05-02 10:25:36.182883 openai_messages_token_helper-0.1.1/CHANGELOG.md
--rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.1/LICENSE
--rw-r--r--   0        0        0     4481 2024-05-02 08:43:27.104337 openai_messages_token_helper-0.1.1/README.md
--rw-r--r--   0        0        0     1326 2024-05-02 10:25:36.186065 openai_messages_token_helper-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/__init__.py
--rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/function_format.py
--rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/images_helper.py
--rw-r--r--   0        0        0     5561 2024-05-02 08:43:27.115625 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/message_builder.py
--rw-r--r--   0        0        0     6325 2024-05-02 10:25:36.189164 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/model_helper.py
--rw-r--r--   0        0        0        0 2024-05-02 10:25:36.189581 openai_messages_token_helper-0.1.1/src/py.typed
--rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.1/tests/functions.py
--rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.1/tests/image_large.png
--rw-r--r--   0        0        0     4034 2024-05-02 08:43:27.123570 openai_messages_token_helper-0.1.1/tests/messages.py
--rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.1/tests/test_imageshelper.py
--rw-r--r--   0        0        0     8562 2024-05-02 08:43:27.127154 openai_messages_token_helper-0.1.1/tests/test_messagebuilder.py
--rw-r--r--   0        0        0     3499 2024-05-02 08:43:27.130210 openai_messages_token_helper-0.1.1/tests/test_modelhelper.py
--rw-r--r--   0        0        0     2136 2024-05-02 10:25:36.191012 openai_messages_token_helper-0.1.1/tests/verify_functions.py
--rw-r--r--   0        0        0     2043 2024-05-02 10:25:36.191752 openai_messages_token_helper-0.1.1/tests/verify_openai.py
--rw-r--r--   0        0        0     5602 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      967 2024-05-02 10:25:36.174822 openai_messages_token_helper-0.1.2/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.2/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.2/.vscode/launch.json
+-rw-r--r--   0        0        0      323 2024-05-02 10:25:36.179140 openai_messages_token_helper-0.1.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1620 2024-05-02 10:29:52.485420 openai_messages_token_helper-0.1.2/CHANGELOG.md
+-rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4481 2024-05-02 08:43:27.104337 openai_messages_token_helper-0.1.2/README.md
+-rw-r--r--   0        0        0     1326 2024-05-02 10:29:58.793584 openai_messages_token_helper-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/function_format.py
+-rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/images_helper.py
+-rw-r--r--   0        0        0     5561 2024-05-02 08:43:27.115625 openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/message_builder.py
+-rw-r--r--   0        0        0     6325 2024-05-02 10:25:36.189164 openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/model_helper.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:25:36.189581 openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/py.typed
+-rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.2/tests/functions.py
+-rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.2/tests/image_large.png
+-rw-r--r--   0        0        0     4034 2024-05-02 08:43:27.123570 openai_messages_token_helper-0.1.2/tests/messages.py
+-rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.2/tests/test_imageshelper.py
+-rw-r--r--   0        0        0     8562 2024-05-02 08:43:27.127154 openai_messages_token_helper-0.1.2/tests/test_messagebuilder.py
+-rw-r--r--   0        0        0     3499 2024-05-02 08:43:27.130210 openai_messages_token_helper-0.1.2/tests/test_modelhelper.py
+-rw-r--r--   0        0        0     2136 2024-05-02 10:25:36.191012 openai_messages_token_helper-0.1.2/tests/verify_functions.py
+-rw-r--r--   0        0        0     2043 2024-05-02 10:25:36.191752 openai_messages_token_helper-0.1.2/tests/verify_openai.py
+-rw-r--r--   0        0        0     5602 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.2/PKG-INFO
```

### Comparing `openai_messages_token_helper-0.1.1/.github/workflows/python.yaml` & `openai_messages_token_helper-0.1.2/.github/workflows/python.yaml`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/.gitignore` & `openai_messages_token_helper-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/.vscode/launch.json` & `openai_messages_token_helper-0.1.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/CHANGELOG.md` & `openai_messages_token_helper-0.1.2/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
-## [0.1.1] - May 2, 2024
+## [0.1.2] - May 2, 2024
 
 - Add `py.typed` file so that mypy can find the type hints in this package.
 
 ## [0.1.0] - May 2, 2024
 
 - Add `count_tokens_for_system_and_tools` to count tokens for system message and tools. You should count the tokens for both together, since the token count for tools varies based off whether a system message is provided.
 - Updated `build_messages` to allow for `tools` and `tool_choice` to be passed in.
```

### Comparing `openai_messages_token_helper-0.1.1/LICENSE` & `openai_messages_token_helper-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/README.md` & `openai_messages_token_helper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/pyproject.toml` & `openai_messages_token_helper-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "openai-messages-token-helper"
 description = "A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API."
-version = "0.1.1"
+version = "0.1.2"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "openai",
     "tiktoken",
```

### Comparing `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/function_format.py` & `openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/function_format.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/images_helper.py` & `openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/images_helper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/message_builder.py` & `openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/message_builder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/model_helper.py` & `openai_messages_token_helper-0.1.2/src/openai_messages_token_helper/model_helper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/functions.py` & `openai_messages_token_helper-0.1.2/tests/functions.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/image_large.png` & `openai_messages_token_helper-0.1.2/tests/image_large.png`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/messages.py` & `openai_messages_token_helper-0.1.2/tests/messages.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/test_imageshelper.py` & `openai_messages_token_helper-0.1.2/tests/test_imageshelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/test_messagebuilder.py` & `openai_messages_token_helper-0.1.2/tests/test_messagebuilder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/test_modelhelper.py` & `openai_messages_token_helper-0.1.2/tests/test_modelhelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/verify_functions.py` & `openai_messages_token_helper-0.1.2/tests/verify_functions.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/tests/verify_openai.py` & `openai_messages_token_helper-0.1.2/tests/verify_openai.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.1/PKG-INFO` & `openai_messages_token_helper-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-messages-token-helper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API.
 Author: Pamela Fox
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

