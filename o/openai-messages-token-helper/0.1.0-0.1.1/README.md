# Comparing `tmp/openai_messages_token_helper-0.1.0.tar.gz` & `tmp/openai_messages_token_helper-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_messages_token_helper-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "openai_messages_token_helper-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `openai_messages_token_helper-0.1.0.tar` & `openai_messages_token_helper-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,27 @@
--rw-r--r--   0        0        0      913 2024-05-02 08:43:27.095494 openai_messages_token_helper-0.1.0/.github/workflows/python.yaml
--rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.0/.gitignore
--rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.0/.vscode/launch.json
--rw-r--r--   0        0        0      148 2024-04-21 22:10:10.823452 openai_messages_token_helper-0.1.0/.vscode/settings.json
--rw-r--r--   0        0        0     1517 2024-05-02 08:44:48.896748 openai_messages_token_helper-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.0/LICENSE
--rw-r--r--   0        0        0     4481 2024-05-02 08:43:27.104337 openai_messages_token_helper-0.1.0/README.md
--rw-r--r--   0        0        0     1314 2024-05-02 08:43:27.107170 openai_messages_token_helper-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/__init__.py
--rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/function_format.py
--rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/images_helper.py
--rw-r--r--   0        0        0     5561 2024-05-02 08:43:27.115625 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/message_builder.py
--rw-r--r--   0        0        0     6309 2024-05-02 08:43:27.117979 openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/model_helper.py
--rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.0/tests/functions.py
--rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.0/tests/image_large.png
--rw-r--r--   0        0        0     4034 2024-05-02 08:43:27.123570 openai_messages_token_helper-0.1.0/tests/messages.py
--rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.0/tests/test_imageshelper.py
--rw-r--r--   0        0        0     8562 2024-05-02 08:43:27.127154 openai_messages_token_helper-0.1.0/tests/test_messagebuilder.py
--rw-r--r--   0        0        0     3499 2024-05-02 08:43:27.130210 openai_messages_token_helper-0.1.0/tests/test_modelhelper.py
--rw-r--r--   0        0        0     1361 2024-05-02 08:43:27.134289 openai_messages_token_helper-0.1.0/tests/verify_functions.py
--rw-r--r--   0        0        0     1274 2024-05-02 08:43:27.136603 openai_messages_token_helper-0.1.0/tests/verify_openai.py
--rw-r--r--   0        0        0     5565 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      967 2024-05-02 10:25:36.174822 openai_messages_token_helper-0.1.1/.github/workflows/python.yaml
+-rw-r--r--   0        0        0     1799 2024-04-04 18:34:36.837611 openai_messages_token_helper-0.1.1/.gitignore
+-rw-r--r--   0        0        0      359 2024-04-21 22:10:10.818591 openai_messages_token_helper-0.1.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      536 2024-05-02 08:43:27.099990 openai_messages_token_helper-0.1.1/.vscode/launch.json
+-rw-r--r--   0        0        0      323 2024-05-02 10:25:36.179140 openai_messages_token_helper-0.1.1/.vscode/settings.json
+-rw-r--r--   0        0        0     1620 2024-05-02 10:25:36.182883 openai_messages_token_helper-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0      311 2024-04-24 16:19:50.746331 openai_messages_token_helper-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1078 2024-04-04 18:34:36.838438 openai_messages_token_helper-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4481 2024-05-02 08:43:27.104337 openai_messages_token_helper-0.1.1/README.md
+-rw-r--r--   0        0        0     1326 2024-05-02 10:25:36.186065 openai_messages_token_helper-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      360 2024-05-02 08:43:27.109262 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/__init__.py
+-rw-r--r--   0        0        0     2423 2024-05-02 08:43:27.112777 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/function_format.py
+-rw-r--r--   0        0        0     2020 2024-04-24 15:10:08.289382 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/images_helper.py
+-rw-r--r--   0        0        0     5561 2024-05-02 08:43:27.115625 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/message_builder.py
+-rw-r--r--   0        0        0     6325 2024-05-02 10:25:36.189164 openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/model_helper.py
+-rw-r--r--   0        0        0        0 2024-05-02 10:25:36.189581 openai_messages_token_helper-0.1.1/src/py.typed
+-rw-r--r--   0        0        0        0 2024-04-21 22:10:10.833586 openai_messages_token_helper-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-04 18:34:36.839523 openai_messages_token_helper-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    16187 2024-05-02 08:43:27.120583 openai_messages_token_helper-0.1.1/tests/functions.py
+-rw-r--r--   0        0        0   317320 2024-04-04 19:36:32.913476 openai_messages_token_helper-0.1.1/tests/image_large.png
+-rw-r--r--   0        0        0     4034 2024-05-02 08:43:27.123570 openai_messages_token_helper-0.1.1/tests/messages.py
+-rw-r--r--   0        0        0     1105 2024-04-26 13:30:53.397027 openai_messages_token_helper-0.1.1/tests/test_imageshelper.py
+-rw-r--r--   0        0        0     8562 2024-05-02 08:43:27.127154 openai_messages_token_helper-0.1.1/tests/test_messagebuilder.py
+-rw-r--r--   0        0        0     3499 2024-05-02 08:43:27.130210 openai_messages_token_helper-0.1.1/tests/test_modelhelper.py
+-rw-r--r--   0        0        0     2136 2024-05-02 10:25:36.191012 openai_messages_token_helper-0.1.1/tests/verify_functions.py
+-rw-r--r--   0        0        0     2043 2024-05-02 10:25:36.191752 openai_messages_token_helper-0.1.1/tests/verify_openai.py
+-rw-r--r--   0        0        0     5602 1970-01-01 00:00:00.000000 openai_messages_token_helper-0.1.1/PKG-INFO
```

### Comparing `openai_messages_token_helper-0.1.0/.github/workflows/python.yaml` & `openai_messages_token_helper-0.1.1/.github/workflows/python.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -27,7 +27,9 @@
         - name: Lint with ruff
           run: ruff .
         - name: Check formatting with black
           run: black . --check --verbose
         - name: Run unit tests
           run: |
             python3 -m pytest -s -vv --cov --cov-fail-under=99
+        - name: Run type checks
+          run: mypy .
```

### Comparing `openai_messages_token_helper-0.1.0/.gitignore` & `openai_messages_token_helper-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/.vscode/launch.json` & `openai_messages_token_helper-0.1.1/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/CHANGELOG.md` & `openai_messages_token_helper-0.1.1/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## [0.1.1] - May 2, 2024
+
+- Add `py.typed` file so that mypy can find the type hints in this package.
+
 ## [0.1.0] - May 2, 2024
 
 - Add `count_tokens_for_system_and_tools` to count tokens for system message and tools. You should count the tokens for both together, since the token count for tools varies based off whether a system message is provided.
 - Updated `build_messages` to allow for `tools` and `tool_choice` to be passed in.
 - Breaking change: Changed `new_user_message` to `new_user_content` in `build_messages` for clarity.
 
 ## [0.0.6] - April 24, 2024
```

### Comparing `openai_messages_token_helper-0.1.0/LICENSE` & `openai_messages_token_helper-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/README.md` & `openai_messages_token_helper-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/pyproject.toml` & `openai_messages_token_helper-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "openai-messages-token-helper"
 description = "A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API."
-version = "0.1.0"
+version = "0.1.1"
 authors = [{name = "Pamela Fox"}]
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE"}
 dependencies = [
     "openai",
     "tiktoken",
@@ -29,15 +29,16 @@
     "pytest",
     "pytest-cov",
     "pre-commit",
     "ruff",
     "black",
     "flit",
     "azure-identity",
-    "python-dotenv"
+    "python-dotenv",
+    "mypy"
 ]
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [tool.ruff]
```

### Comparing `openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/function_format.py` & `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/function_format.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/images_helper.py` & `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/images_helper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/message_builder.py` & `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/message_builder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/src/openai_messages_token_helper/model_helper.py` & `openai_messages_token_helper-0.1.1/src/openai_messages_token_helper/model_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
             num_tokens += 1
     num_tokens += 3  # every reply is primed with <|start|>assistant<|message|>
     return num_tokens
 
 
 def count_tokens_for_system_and_tools(
     model: str,
-    system_message: dict | None = None,
+    system_message: Mapping[str, object] | None = None,
     tools: list[dict[str, dict]] | None = None,
     tool_choice: str | dict | None = None,
     default_to_cl100k: bool = False,
 ) -> int:
     """
     Calculate the number of tokens required to encode a system message and tools.
     Both must be calculated together because the count is lower if both are present.
```

### Comparing `openai_messages_token_helper-0.1.0/tests/functions.py` & `openai_messages_token_helper-0.1.1/tests/functions.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/tests/image_large.png` & `openai_messages_token_helper-0.1.1/tests/image_large.png`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/tests/messages.py` & `openai_messages_token_helper-0.1.1/tests/messages.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/tests/test_imageshelper.py` & `openai_messages_token_helper-0.1.1/tests/test_imageshelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/tests/test_messagebuilder.py` & `openai_messages_token_helper-0.1.1/tests/test_messagebuilder.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/tests/test_modelhelper.py` & `openai_messages_token_helper-0.1.1/tests/test_modelhelper.py`

 * *Files identical despite different names*

### Comparing `openai_messages_token_helper-0.1.0/PKG-INFO` & `openai_messages_token_helper-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-messages-token-helper
-Version: 0.1.0
+Version: 0.1.1
 Summary: A helper library for estimating tokens used by messages sent through OpenAI Chat Completions API.
 Author: Pamela Fox
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -19,14 +19,15 @@
 Requires-Dist: pytest-cov ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff ; extra == "dev"
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: flit ; extra == "dev"
 Requires-Dist: azure-identity ; extra == "dev"
 Requires-Dist: python-dotenv ; extra == "dev"
+Requires-Dist: mypy ; extra == "dev"
 Project-URL: Home, https://github.com/pamelafox/openai-messages-token-helper
 Provides-Extra: dev
 
 # openai-messages-token-helper
 
 A helper library for estimating tokens used by messages and building messages lists that fit within the token limits of a model.
 Currently designed to work with the OpenAI GPT models (including GPT-4 turbo with vision).
```

