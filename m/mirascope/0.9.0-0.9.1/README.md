# Comparing `tmp/mirascope-0.9.0.tar.gz` & `tmp/mirascope-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirascope-0.9.0.tar", max compression
+gzip compressed data, was "mirascope-0.9.1.tar", max compression
```

## Comparing `mirascope-0.9.0.tar` & `mirascope-0.9.1.tar`

### file list

```diff
@@ -1,62 +1,62 @@
--rw-r--r--   0        0        0     1072 2024-04-05 17:20:31.993416 mirascope-0.9.0/LICENSE
--rw-r--r--   0        0        0    10203 2024-04-05 17:20:31.993416 mirascope-0.9.0/docs/README.md
--rw-r--r--   0        0        0      524 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/__init__.py
--rw-r--r--   0        0        0      270 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/__init__.py
--rw-r--r--   0        0        0     6596 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/calls.py
--rw-r--r--   0        0        0     4068 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/extractors.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/py.typed
--rw-r--r--   0        0        0     3549 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/tools.py
--rw-r--r--   0        0        0     6006 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/anthropic/types.py
--rw-r--r--   0        0        0      453 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/__init__.py
--rw-r--r--   0        0        0     3645 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/calls.py
--rw-r--r--   0        0        0     8304 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/extractors.py
--rw-r--r--   0        0        0     5696 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/prompts.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/py.typed
--rw-r--r--   0        0        0     2890 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/tools.py
--rw-r--r--   0        0        0     5313 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/types.py
--rw-r--r--   0        0        0     5615 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/base/utils.py
--rw-r--r--   0        0        0       97 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/__init__.py
--rw-r--r--   0        0        0      199 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/__init__.py
--rw-r--r--   0        0        0     4213 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/add.py
--rw-r--r--   0        0        0     3002 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/init.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/py.typed
--rw-r--r--   0        0        0     3101 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/remove.py
--rw-r--r--   0        0        0     2008 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/status.py
--rw-r--r--   0        0        0     2801 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/commands/use.py
--rw-r--r--   0        0        0      118 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/constants.py
--rw-r--r--   0        0        0       86 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/generic/__init__.py
--rw-r--r--   0        0        0      494 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/generic/mirascope.ini.j2
--rw-r--r--   0        0        0     1554 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/generic/prompt_template.j2
--rw-r--r--   0        0        0     1067 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/main.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/py.typed
--rw-r--r--   0        0        0     1197 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/schemas.py
--rw-r--r--   0        0        0    24322 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/cli/utils.py
--rw-r--r--   0        0        0     1552 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/enums.py
--rw-r--r--   0        0        0      241 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/__init__.py
--rw-r--r--   0        0        0     6333 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/calls.py
--rw-r--r--   0        0        0     3730 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/extractors.py
--rw-r--r--   0        0        0     4081 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/tools.py
--rw-r--r--   0        0        0     4950 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/gemini/types.py
--rw-r--r--   0        0        0      223 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/__init__.py
--rw-r--r--   0        0        0     7211 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/calls.py
--rw-r--r--   0        0        0     3537 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/extractors.py
--rw-r--r--   0        0        0     3954 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/tools.py
--rw-r--r--   0        0        0     8845 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/groq/types.py
--rw-r--r--   0        0        0      239 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/__init__.py
--rw-r--r--   0        0        0     5900 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/calls.py
--rw-r--r--   0        0        0     3940 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/extractors.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/py.typed
--rw-r--r--   0        0        0     3898 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/tools.py
--rw-r--r--   0        0        0     6389 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/mistral/types.py
--rw-r--r--   0        0        0      232 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/__init__.py
--rw-r--r--   0        0        0     8720 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/calls.py
--rw-r--r--   0        0        0     3932 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/extractors.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/py.typed
--rw-r--r--   0        0        0     3860 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/tools.py
--rw-r--r--   0        0        0     9087 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/openai/types.py
--rw-r--r--   0        0        0        0 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/py.typed
--rw-r--r--   0        0        0      151 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/wandb/__init__.py
--rw-r--r--   0        0        0     9593 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/wandb/wandb.py
--rw-r--r--   0        0        0     1921 2024-04-05 17:20:31.997416 mirascope-0.9.0/mirascope/wandb/weave.py
--rw-r--r--   0        0        0     2861 2024-04-05 17:20:32.001416 mirascope-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    11730 1970-01-01 00:00:00.000000 mirascope-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-05 23:23:30.225953 mirascope-0.9.1/LICENSE
+-rw-r--r--   0        0        0    10203 2024-04-05 23:23:30.225953 mirascope-0.9.1/docs/README.md
+-rw-r--r--   0        0        0      524 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/__init__.py
+-rw-r--r--   0        0        0      270 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/anthropic/__init__.py
+-rw-r--r--   0        0        0     6596 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/anthropic/calls.py
+-rw-r--r--   0        0        0     4068 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/anthropic/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/anthropic/py.typed
+-rw-r--r--   0        0        0     3549 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/anthropic/tools.py
+-rw-r--r--   0        0        0     6006 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/anthropic/types.py
+-rw-r--r--   0        0        0      453 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/__init__.py
+-rw-r--r--   0        0        0     3645 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/calls.py
+-rw-r--r--   0        0        0     8304 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/extractors.py
+-rw-r--r--   0        0        0     5696 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/prompts.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/py.typed
+-rw-r--r--   0        0        0     2890 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/tools.py
+-rw-r--r--   0        0        0     5313 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/types.py
+-rw-r--r--   0        0        0     5615 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/base/utils.py
+-rw-r--r--   0        0        0       97 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/__init__.py
+-rw-r--r--   0        0        0     4213 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/add.py
+-rw-r--r--   0        0        0     3002 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/init.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/py.typed
+-rw-r--r--   0        0        0     3101 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/remove.py
+-rw-r--r--   0        0        0     2008 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/status.py
+-rw-r--r--   0        0        0     2801 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/commands/use.py
+-rw-r--r--   0        0        0      118 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/constants.py
+-rw-r--r--   0        0        0       86 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/generic/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/generic/mirascope.ini.j2
+-rw-r--r--   0        0        0     1554 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/generic/prompt_template.j2
+-rw-r--r--   0        0        0     1067 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/py.typed
+-rw-r--r--   0        0        0     1197 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/schemas.py
+-rw-r--r--   0        0        0    24338 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/cli/utils.py
+-rw-r--r--   0        0        0     1552 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/enums.py
+-rw-r--r--   0        0        0      241 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/gemini/__init__.py
+-rw-r--r--   0        0        0     6333 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/gemini/calls.py
+-rw-r--r--   0        0        0     3730 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/gemini/extractors.py
+-rw-r--r--   0        0        0     4081 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/gemini/tools.py
+-rw-r--r--   0        0        0     4950 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/gemini/types.py
+-rw-r--r--   0        0        0      223 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/groq/__init__.py
+-rw-r--r--   0        0        0     7211 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/groq/calls.py
+-rw-r--r--   0        0        0     3537 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/groq/extractors.py
+-rw-r--r--   0        0        0     3954 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/groq/tools.py
+-rw-r--r--   0        0        0     8845 2024-04-05 23:23:30.229953 mirascope-0.9.1/mirascope/groq/types.py
+-rw-r--r--   0        0        0      239 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/mistral/__init__.py
+-rw-r--r--   0        0        0     5900 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/mistral/calls.py
+-rw-r--r--   0        0        0     3940 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/mistral/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/mistral/py.typed
+-rw-r--r--   0        0        0     3898 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/mistral/tools.py
+-rw-r--r--   0        0        0     6389 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/mistral/types.py
+-rw-r--r--   0        0        0      232 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/openai/__init__.py
+-rw-r--r--   0        0        0     8720 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/openai/calls.py
+-rw-r--r--   0        0        0     3932 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/openai/extractors.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/openai/py.typed
+-rw-r--r--   0        0        0     3860 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/openai/tools.py
+-rw-r--r--   0        0        0     9087 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/openai/types.py
+-rw-r--r--   0        0        0        0 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/py.typed
+-rw-r--r--   0        0        0      151 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/wandb/__init__.py
+-rw-r--r--   0        0        0     9593 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/wandb/wandb.py
+-rw-r--r--   0        0        0     1921 2024-04-05 23:23:30.233953 mirascope-0.9.1/mirascope/wandb/weave.py
+-rw-r--r--   0        0        0     2861 2024-04-05 23:23:30.233953 mirascope-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0    11730 1970-01-01 00:00:00.000000 mirascope-0.9.1/PKG-INFO
```

### Comparing `mirascope-0.9.0/LICENSE` & `mirascope-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/docs/README.md` & `mirascope-0.9.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/__init__.py` & `mirascope-0.9.1/mirascope/__init__.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/anthropic/calls.py` & `mirascope-0.9.1/mirascope/anthropic/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/anthropic/extractors.py` & `mirascope-0.9.1/mirascope/anthropic/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/anthropic/tools.py` & `mirascope-0.9.1/mirascope/anthropic/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/anthropic/types.py` & `mirascope-0.9.1/mirascope/anthropic/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/base/calls.py` & `mirascope-0.9.1/mirascope/base/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/base/extractors.py` & `mirascope-0.9.1/mirascope/base/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/base/prompts.py` & `mirascope-0.9.1/mirascope/base/prompts.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/base/tools.py` & `mirascope-0.9.1/mirascope/base/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/base/types.py` & `mirascope-0.9.1/mirascope/base/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/base/utils.py` & `mirascope-0.9.1/mirascope/base/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/commands/add.py` & `mirascope-0.9.1/mirascope/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/commands/init.py` & `mirascope-0.9.1/mirascope/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/commands/remove.py` & `mirascope-0.9.1/mirascope/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/commands/status.py` & `mirascope-0.9.1/mirascope/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/commands/use.py` & `mirascope-0.9.1/mirascope/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/generic/prompt_template.j2` & `mirascope-0.9.1/mirascope/cli/generic/prompt_template.j2`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/main.py` & `mirascope-0.9.1/mirascope/cli/main.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/schemas.py` & `mirascope-0.9.1/mirascope/cli/schemas.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/cli/utils.py` & `mirascope-0.9.1/mirascope/cli/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 ignore_variables = {"prev_revision_id", "revision_id"}
 mirascope_prompt_bases = (
     "BasePrompt",
     "OpenAICall",
     "GeminiCall",
     "AnthropicCall",
     "WandbOpenAICall",
+    "GroqCall",
 )
 
 
 class PromptAnalyzer(ast.NodeVisitor):
     """Utility class for analyzing a Mirascope prompt file.
 
     The call to `ast.parse()` returns Python code as an AST, whereby each visitor method
```

### Comparing `mirascope-0.9.0/mirascope/enums.py` & `mirascope-0.9.1/mirascope/enums.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/gemini/calls.py` & `mirascope-0.9.1/mirascope/gemini/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/gemini/extractors.py` & `mirascope-0.9.1/mirascope/gemini/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/gemini/tools.py` & `mirascope-0.9.1/mirascope/gemini/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/gemini/types.py` & `mirascope-0.9.1/mirascope/gemini/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/groq/calls.py` & `mirascope-0.9.1/mirascope/groq/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/groq/extractors.py` & `mirascope-0.9.1/mirascope/groq/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/groq/tools.py` & `mirascope-0.9.1/mirascope/groq/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/groq/types.py` & `mirascope-0.9.1/mirascope/groq/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/mistral/calls.py` & `mirascope-0.9.1/mirascope/mistral/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/mistral/extractors.py` & `mirascope-0.9.1/mirascope/mistral/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/mistral/tools.py` & `mirascope-0.9.1/mirascope/mistral/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/mistral/types.py` & `mirascope-0.9.1/mirascope/mistral/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/openai/calls.py` & `mirascope-0.9.1/mirascope/openai/calls.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/openai/extractors.py` & `mirascope-0.9.1/mirascope/openai/extractors.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/openai/tools.py` & `mirascope-0.9.1/mirascope/openai/tools.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/openai/types.py` & `mirascope-0.9.1/mirascope/openai/types.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/wandb/wandb.py` & `mirascope-0.9.1/mirascope/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/mirascope/wandb/weave.py` & `mirascope-0.9.1/mirascope/wandb/weave.py`

 * *Files identical despite different names*

### Comparing `mirascope-0.9.0/pyproject.toml` & `mirascope-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mirascope"
-version = "0.9.0"
+version = "0.9.1"
 description = "LLM toolkit for lightning-fast, high-quality development"
 license = "MIT"
 authors = [
     "William Bakst <william@mirascope.io>",
     "Brendan Kao <brendan@mirascope.io>",
 ]
 readme = "docs/README.md"
```

### Comparing `mirascope-0.9.0/PKG-INFO` & `mirascope-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mirascope
-Version: 0.9.0
+Version: 0.9.1
 Summary: LLM toolkit for lightning-fast, high-quality development
 Home-page: https://github.com/Mirascope/mirascope
 License: MIT
 Author: William Bakst
 Author-email: william@mirascope.io
 Requires-Python: >=3.9,<3.13
 Classifier: License :: OSI Approved :: MIT License
```

