# Comparing `tmp/lmwrapper-0.8.7.6.tar.gz` & `tmp/lmwrapper-0.9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lmwrapper-0.8.7.6.tar", last modified: Sat Apr  6 07:17:32 2024, max compression
+gzip compressed data, was "lmwrapper-0.9.0.2.tar", last modified: Thu May  2 00:41:41 2024, max compression
```

## Comparing `lmwrapper-0.8.7.6.tar` & `lmwrapper-0.9.0.2.tar`

### file list

```diff
@@ -1,43 +1,45 @@
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 07:17:32.123488 lmwrapper-0.8.7.6/
--rw-r--r--   0 dgros      (501) staff       (20)     6730 2024-04-06 07:17:32.123185 lmwrapper-0.8.7.6/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.8.7.6/README.md
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 07:17:32.116200 lmwrapper-0.8.7.6/lmwrapper/
--rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/_TokenStoppingCriteria.py
--rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     4259 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/abstract_predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/env.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 07:17:32.118702 lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/
--rw-r--r--   0 dgros      (501) staff       (20)      177 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/prediction.py
--rw-r--r--   0 dgros      (501) staff       (20)    34304 2024-04-06 06:54:30.000000 lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/predictor.py
--rw-r--r--   0 dgros      (501) staff       (20)      304 2024-04-06 06:54:30.000000 lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/utilstorch.py
--rw-r--r--   0 dgros      (501) staff       (20)    27235 2024-04-06 06:54:30.000000 lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/wrapper.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 07:17:32.119212 lmwrapper-0.8.7.6/lmwrapper/openai_wrapper/
--rw-r--r--   0 dgros      (501) staff       (20)      139 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/lmwrapper/openai_wrapper/__init__.py
--rw-r--r--   0 dgros      (501) staff       (20)    18610 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/lmwrapper/openai_wrapper/wrapper.py
--rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/runtime.py
--rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/secrets_manager.py
--rw-r--r--   0 dgros      (501) staff       (20)    16083 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.8.7.6/lmwrapper/togethertoy.py
--rw-r--r--   0 dgros      (501) staff       (20)     2227 2024-04-06 06:54:30.000000 lmwrapper-0.8.7.6/lmwrapper/utils.py
--rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/lmwrapper/wrapping_config.py
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 07:17:32.122034 lmwrapper-0.8.7.6/lmwrapper.egg-info/
--rw-r--r--   0 dgros      (501) staff       (20)     6730 2024-04-06 07:17:32.000000 lmwrapper-0.8.7.6/lmwrapper.egg-info/PKG-INFO
--rw-r--r--   0 dgros      (501) staff       (20)      987 2024-04-06 07:17:32.000000 lmwrapper-0.8.7.6/lmwrapper.egg-info/SOURCES.txt
--rw-r--r--   0 dgros      (501) staff       (20)        1 2024-04-06 07:17:32.000000 lmwrapper-0.8.7.6/lmwrapper.egg-info/dependency_links.txt
--rw-r--r--   0 dgros      (501) staff       (20)      402 2024-04-06 07:17:32.000000 lmwrapper-0.8.7.6/lmwrapper.egg-info/requires.txt
--rw-r--r--   0 dgros      (501) staff       (20)       10 2024-04-06 07:17:32.000000 lmwrapper-0.8.7.6/lmwrapper.egg-info/top_level.txt
--rw-r--r--   0 dgros      (501) staff       (20)     4912 2024-04-06 06:57:34.000000 lmwrapper-0.8.7.6/pyproject.toml
--rw-r--r--   0 dgros      (501) staff       (20)       38 2024-04-06 07:17:32.123545 lmwrapper-0.8.7.6/setup.cfg
-drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-04-06 07:17:32.121496 lmwrapper-0.8.7.6/test/
--rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/test/test_caching.py
--rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/test/test_docs.py
--rw-r--r--   0 dgros      (501) staff       (20)    30472 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/test/test_huggingface.py
--rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/test/test_huggingface_memory.py
--rw-r--r--   0 dgros      (501) staff       (20)    17741 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/test/test_models_common.py
--rw-r--r--   0 dgros      (501) staff       (20)    10251 2024-03-30 04:33:51.000000 lmwrapper-0.8.7.6/test/test_openai.py
--rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.8.7.6/test/test_prompt_trimming.py
--rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.8.7.6/test/test_structs.py
--rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.8.7.6/test/test_util.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-02 00:41:41.182948 lmwrapper-0.9.0.2/
+-rw-r--r--   0 dgros      (501) staff       (20)     6730 2024-05-02 00:41:41.182724 lmwrapper-0.9.0.2/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     5312 2024-04-06 05:06:05.000000 lmwrapper-0.9.0.2/README.md
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-02 00:41:41.176178 lmwrapper-0.9.0.2/lmwrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)     2416 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/_TokenStoppingCriteria.py
+-rw-r--r--   0 dgros      (501) staff       (20)        0 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4461 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/abstract_predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1654 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      294 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/env.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-02 00:41:41.178210 lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)       90 2024-04-29 23:28:16.000000 lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1712 2024-03-30 04:33:51.000000 lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/prediction.py
+-rw-r--r--   0 dgros      (501) staff       (20)    41344 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/predictor.py
+-rw-r--r--   0 dgros      (501) staff       (20)      305 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/utilstorch.py
+-rw-r--r--   0 dgros      (501) staff       (20)    27146 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3920 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/interals.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-02 00:41:41.178692 lmwrapper-0.9.0.2/lmwrapper/openai_wrapper/
+-rw-r--r--   0 dgros      (501) staff       (20)       74 2024-05-01 22:58:02.000000 lmwrapper-0.9.0.2/lmwrapper/openai_wrapper/__init__.py
+-rw-r--r--   0 dgros      (501) staff       (20)    18567 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/openai_wrapper/wrapper.py
+-rw-r--r--   0 dgros      (501) staff       (20)     3646 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)      583 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/runtime.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1149 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/secrets_manager.py
+-rw-r--r--   0 dgros      (501) staff       (20)    16301 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/lmwrapper/structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      710 2024-03-19 21:15:58.000000 lmwrapper-0.9.0.2/lmwrapper/togethertoy.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2227 2024-04-06 06:54:30.000000 lmwrapper-0.9.0.2/lmwrapper/utils.py
+-rw-r--r--   0 dgros      (501) staff       (20)     1098 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/lmwrapper/wrapping_config.py
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-02 00:41:41.181692 lmwrapper-0.9.0.2/lmwrapper.egg-info/
+-rw-r--r--   0 dgros      (501) staff       (20)     6730 2024-05-02 00:41:41.000000 lmwrapper-0.9.0.2/lmwrapper.egg-info/PKG-INFO
+-rw-r--r--   0 dgros      (501) staff       (20)     1044 2024-05-02 00:41:41.000000 lmwrapper-0.9.0.2/lmwrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 dgros      (501) staff       (20)        1 2024-05-02 00:41:41.000000 lmwrapper-0.9.0.2/lmwrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 dgros      (501) staff       (20)      402 2024-05-02 00:41:41.000000 lmwrapper-0.9.0.2/lmwrapper.egg-info/requires.txt
+-rw-r--r--   0 dgros      (501) staff       (20)       10 2024-05-02 00:41:41.000000 lmwrapper-0.9.0.2/lmwrapper.egg-info/top_level.txt
+-rw-r--r--   0 dgros      (501) staff       (20)     4912 2024-05-02 00:40:39.000000 lmwrapper-0.9.0.2/pyproject.toml
+-rw-r--r--   0 dgros      (501) staff       (20)       38 2024-05-02 00:41:41.182992 lmwrapper-0.9.0.2/setup.cfg
+drwxr-xr-x   0 dgros      (501) staff       (20)        0 2024-05-02 00:41:41.181194 lmwrapper-0.9.0.2/test/
+-rw-r--r--   0 dgros      (501) staff       (20)     1244 2024-03-30 04:33:51.000000 lmwrapper-0.9.0.2/test/test_caching.py
+-rw-r--r--   0 dgros      (501) staff       (20)      547 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/test/test_docs.py
+-rw-r--r--   0 dgros      (501) staff       (20)    31215 2024-05-02 00:01:14.000000 lmwrapper-0.9.0.2/test/test_huggingface.py
+-rw-r--r--   0 dgros      (501) staff       (20)     4965 2024-05-02 00:39:14.000000 lmwrapper-0.9.0.2/test/test_huggingface_internals.py
+-rw-r--r--   0 dgros      (501) staff       (20)     6534 2024-03-30 04:33:51.000000 lmwrapper-0.9.0.2/test/test_huggingface_memory.py
+-rw-r--r--   0 dgros      (501) staff       (20)    17737 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/test/test_models_common.py
+-rw-r--r--   0 dgros      (501) staff       (20)    10394 2024-04-29 22:31:00.000000 lmwrapper-0.9.0.2/test/test_openai.py
+-rw-r--r--   0 dgros      (501) staff       (20)      512 2024-03-28 22:03:47.000000 lmwrapper-0.9.0.2/test/test_prompt_trimming.py
+-rw-r--r--   0 dgros      (501) staff       (20)     2080 2024-02-10 07:57:44.000000 lmwrapper-0.9.0.2/test/test_structs.py
+-rw-r--r--   0 dgros      (501) staff       (20)      237 2024-02-10 00:21:07.000000 lmwrapper-0.9.0.2/test/test_util.py
```

### Comparing `lmwrapper-0.8.7.6/PKG-INFO` & `lmwrapper-0.9.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.8.7.6
+Version: 0.9.0.2
 Summary: Wrapper around language model APIs
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lmwrapper-0.8.7.6/README.md` & `lmwrapper-0.9.0.2/README.md`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/_TokenStoppingCriteria.py` & `lmwrapper-0.9.0.2/lmwrapper/_TokenStoppingCriteria.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/abstract_predictor.py` & `lmwrapper-0.9.0.2/lmwrapper/abstract_predictor.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,18 @@
 
     def predict(
         self,
         prompt: str | LmPrompt,
     ) -> LmPrediction:
         prompt = self._cast_prompt(prompt)
         should_cache = self._cache_default if prompt.cache is None else prompt.cache
+        if should_cache and prompt.model_internals_request is not None:
+            raise NotImplementedError(
+                "Cannot yet cache predictions with model internals request",
+            )
         self._validate_prompt(prompt, raise_on_invalid=True)
         if should_cache:
             cache_key = (prompt, self._get_cache_key_metadata())
             if cache_key in self._disk_cache:
                 cache_copy = self._disk_cache.get(cache_key)
                 if cache_copy:
                     cache_copy = cache_copy.mark_as_cached()
```

### Comparing `lmwrapper-0.8.7.6/lmwrapper/caching.py` & `lmwrapper-0.9.0.2/lmwrapper/caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/prediction.py` & `lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/prediction.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/predictor.py` & `lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/predictor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import inspect
 import logging
 from collections.abc import Sequence
 from functools import cached_property
 from typing import TYPE_CHECKING
 
+import numpy as np
 import torch
 from transformers import GenerationConfig, PreTrainedModel, PreTrainedTokenizerFast
 from transformers.utils.generic import TensorType
 
 from lmwrapper._TokenStoppingCriteria import _TokenStoppingCriteria
 from lmwrapper.abstract_predictor import LmPredictor
 from lmwrapper.huggingface_wrapper.prediction import HuggingFacePrediction
+from lmwrapper.huggingface_wrapper.utilstorch import log_cuda_mem
+from lmwrapper.interals import ModelInternalsRequest, ModelInternalsResults
 from lmwrapper.prompt_trimming import PromptTrimmer
 from lmwrapper.runtime import Runtime
 from lmwrapper.structs import LmPrediction, LmPrompt
-from lmwrapper.huggingface_wrapper.utilstorch import log_cuda_mem
 
 if TYPE_CHECKING:
     from transformers.generation.utils import GenerateOutput
 
 
 class HuggingFacePredictor(LmPredictor):
     def __init__(
@@ -42,75 +44,91 @@
 
     def _get_cache_key_metadata(self):
         return {
             "model": "HuggingFacePredictor",
             "name_or_path": self._model.name_or_path,
         }
 
-    def _predict_hf(
-        self,
-        prompt: LmPrompt,
-    ) -> LmPrediction | list[LmPrediction]:
+    def _verify_initial_prompt(self, prompt: LmPrompt):
         if not isinstance(prompt.text, str) and len(prompt.text) != 1:
             msg = "Prompt batches other than size 1 are not supported."
             raise NotImplementedError(
                 msg,
             )
 
         if prompt.echo and not self.allow_patch_model_forward:
             msg = (
                 "Prompt echo is only supported with `allow_patch_model_forward` = True."
             )
             raise NotImplementedError(
                 msg,
             )
-
-        patch_model_forward = False
-        if self.allow_patch_model_forward:
-            patch_model_forward = prompt.echo
-
-        is_encoder_decoder = self._model.config.is_encoder_decoder
-
-        will_add_bos = prompt.add_bos_token or (
-            prompt.add_bos_token is None
-            and self._tokenizer.bos_token
-            and not is_encoder_decoder
-            and not self._does_this_tokenizer_seem_add_a_bos(prompt.add_special_tokens)
-        )
-        will_have_bos = will_add_bos or self._does_this_tokenizer_seem_add_a_bos(
-            prompt.add_special_tokens,
-        )
-
         if prompt.logprobs > 1:
             msg = (
                 "Retrieving more than 1 logprob is not yet supported for HuggingFace"
                 " models."
             )
             raise NotImplementedError(
                 msg,
             )
-
         if prompt.logprobs and prompt.top_p != 1.0:
             logging.warning("Logprobs may not be correct if top_p != 1.0")
 
         if prompt.presence_penalty != 0.0:
             msg = "Presence penalty not implemented"
             raise NotImplementedError(msg)
 
+    def _will_add_and_have_bos(self, prompt: LmPrompt):
+        will_add_bos = prompt.add_bos_token or (
+            prompt.add_bos_token is None
+            and self._tokenizer.bos_token
+            and not self.is_encoder_decoder
+            and not self._does_this_tokenizer_seem_add_a_bos(prompt.add_special_tokens)
+        )
+        will_have_bos = will_add_bos or self._does_this_tokenizer_seem_add_a_bos(
+            prompt.add_special_tokens,
+        )
         if prompt.text == "" and not will_have_bos:
             msg = "Cannot do unconditional generation without `add_bos_token`."
             raise Exception(
                 msg,
             )
 
-        if is_encoder_decoder and will_add_bos:
+        if self.is_encoder_decoder and will_add_bos:
             msg = "Encoder/decoder models should not have bos tokens added manually."
             raise Exception(
                 msg,
             )
+        return will_add_bos, will_have_bos
+
+    @property
+    def is_encoder_decoder(self) -> bool:
+        return self._model.config.is_encoder_decoder
+
+    def _optional_args_for_internals(self, prompt: LmPrompt):
+        args = {}
+        if prompt.model_internals_request is None:
+            return args
+        if prompt.model_internals_request.return_hidden_states:
+            args["output_hidden_states"] = True
+        if prompt.model_internals_request.return_attentions:
+            args["output_attentions"] = True
+        return args
+
+    def _predict_hf(
+        self,
+        prompt: LmPrompt,
+    ) -> LmPrediction | list[LmPrediction]:
+        self._verify_initial_prompt(prompt)
+
+        patch_model_forward = False
+        if self.allow_patch_model_forward:
+            patch_model_forward = prompt.echo
+
+        will_add_bos, will_have_bos = self._will_add_and_have_bos(prompt)
 
         if will_add_bos:
             assert self._tokenizer.bos_token
             prompt_text = self._tokenizer.bos_token + prompt.text
         else:
             prompt_text = prompt.text
 
@@ -138,15 +156,15 @@
                 )
             else:
                 msg = "Prompt is too long for model. Please pass in a trimmer."
                 raise ValueError(
                     msg,
                 )
 
-        if is_encoder_decoder:
+        if self.is_encoder_decoder:
             encoded_input["decoder_input_ids"] = encoded_input["input_ids"].clone()
 
         logging.debug("Pre moving encoded tokens")
         log_cuda_mem()
         if self.runtime != Runtime.ACCELERATE:
             encoded_input = encoded_input.to(
                 self._device,
@@ -209,14 +227,16 @@
         elif num_beams > 1 and do_sample is True:
             logging.info("Decoding strategy: beam-search multinomial sampling")
         elif num_beams > 1 and num_beam_groups > 1:
             logging.info("Decoding strategy: diverse beam-search")
         else:
             logging.info("Unable to predict decoding strategy!")
 
+        optional_generation_kwargs |= self._optional_args_for_internals(prompt)
+
         # Ref https://gist.github.com/kinoc/8a042d8c5683725aa8c372274c02ea2f
         gen_config = GenerationConfig(
             max_new_tokens=(
                 self.default_tokens_generated
                 if prompt.max_tokens is None
                 else prompt.max_tokens
             ),
@@ -258,15 +278,15 @@
 
         stopping_criteria = None
         # input_length is the length of the input prompt for decoder-only models,
         # like the GPT family, and 1 ?? for encoder-decoder models, like BART or T5.
         # we add 2 to consider the </s> at the end of the prompt and the first <s> as input
         input_length = (
             encoded_input.input_ids.shape[1] + 2
-            if is_encoder_decoder
+            if self.is_encoder_decoder
             else encoded_input.input_ids.shape[1]
         )
         if prompt.stop:
             stopping_criteria = [
                 _TokenStoppingCriteria(
                     prompt.stop,
                     decode=True,
@@ -366,15 +386,15 @@
 
         logprobs_dicts = []
         # Calculate the logprobs if needed
         logprobs = None
         if need_log_prob:
             if patch_model_forward:
                 assert prompt.echo
-                assert not is_encoder_decoder
+                assert not self.is_encoder_decoder
 
                 assert cached_logits.shape[0] == 1  # batch
                 assert cached_logits.shape[1] == len(model_output_sequence[1:])
                 output_logprobs = _gather_logprobs_from_logits(
                     cached_logits[0],
                     model_output_sequence[1:],
                 )
@@ -397,15 +417,15 @@
                     normalize_logits=True,
                 )[0]
 
                 logprobs = output_logprobs.detach().cpu()
                 # Free memory
                 del output_logprobs
 
-                if is_encoder_decoder:
+                if self.is_encoder_decoder:
                     # we need to chop off the <s> first token
                     # as its probability will throw off uncertainty estimates
                     if stop_token_idx_generated:
                         # if a stop token is defined, we need to step one further due to the <s>
                         # TODO: we can clean this up with better input_length logic
                         logprobs = logprobs[1 : stop_token_idx_generated + 1]
                     else:
@@ -462,33 +482,176 @@
             if isinstance(value, tuple):
                 return tuple([numpy_tuple(v) for v in value])
             return None
 
         for key, value in generation_output.items():
             updated_output[key] = numpy_tuple(value)
 
+        internals = self._parse_model_internals_results(
+            prompt,
+            generation_output,
+            will_have_bos,
+            output_tokens,
+        )
+
         del generation_output
         del logprobs
         del encoded_input
 
         logging.debug("Post del statements")
         log_cuda_mem()
 
         return HuggingFacePrediction(
             completion_text=clean_generated_text,
             prompt=prompt,
             metad=updated_output,
+            internals=internals,
             _completion_with_special_tok=generated_text,
             _num_prompt_tokens=(int(input_length) - (1 if will_have_bos else 0)),
             _prompt_encoding=np_encoded_input,
             _tokens=output_tokens,
             _log_probs=np_logprobs,
             _logprobs_dict=logprobs_dicts,
         )
 
+    def _parse_model_internals_results(
+        self,
+        prompt: LmPrompt,
+        generation_output,
+        will_have_bos,
+        output_tokens,
+    ):
+        if prompt.model_internals_request is None:
+            return None
+        request: ModelInternalsRequest = prompt.model_internals_request
+        internal_args = {}
+        if request.return_hidden_states:
+            hidden_states = self._get_hidden_states_combined(
+                generation_output.hidden_states,
+                output_tokens,
+            )
+            hidden_states = request.select_layer_sequence(hidden_states)
+            internal_args["hidden_states"] = hidden_states
+        if request.return_attentions:
+            attentions = self._get_attentions_combined(
+                generation_output.attentions,
+                output_tokens,
+            )
+            attentions = request.select_layer_sequence(attentions)
+            internal_args["attentions"] = attentions
+        internal_args["has_a_bos"] = will_have_bos
+
+        return ModelInternalsResults(**internal_args)
+
+    def _get_attentions_combined(
+        self,
+        attentions,
+        output_tokens,
+    ):
+        """
+        Attentions is a tuple
+        (token_output: tuple, layers: tuple, (batch, head, seq, seq_prompt): tensor).
+        We want to transform a single to (layers, head, seq, seq_prompt): ndarray
+        with the future tokens appropriately masked out.
+
+        Note: that this precludes some more weird schemes such as a different
+        number of heads per layer or some weird sparse attentions where each
+        token_output has different dimensions. We will have to potentially
+        handle those latter.
+        """
+        if len(output_tokens) == 0:
+            return None
+        last_token_attentions = attentions[-1]
+        seems_to_be_token_by_token = last_token_attentions[1].shape[2] == 1
+        if seems_to_be_token_by_token and len(attentions) > 1:
+            # We have something like
+            # ( for each token gen
+            #   (layers, (batch, head, seq_prompt, seq_prompt)),
+            #   (layers, (batch, head, 1, seq_prompt + 1)),
+            #   (layers, (batch, head, 1, seq_prompt + 2)),
+            #   ...
+            # )
+            # We need to combine these and fill any of the added tokens with zeros
+            num_layers = len(attentions[0])
+            num_heads = attentions[0][1].shape[1]
+            total_seq_length = sum(
+                att[1].shape[2] for att in attentions
+            )  # Total sequence length including prompt
+            seq_prompt_length = attentions[0][1].shape[
+                3
+            ]  # Sequence length of the prompt
+
+            # Initialize a tensor to hold the combined attentions for all layers
+            combined_attentions = torch.zeros(
+                (num_layers, num_heads, total_seq_length, total_seq_length),
+            )
+
+            # Fill in the combined attentions tensor
+            seq_offset = 0
+            for tok_gen_i, tok_gen_atten in enumerate(attentions):
+                for layer_idx, att_tensor in enumerate(tok_gen_atten):
+                    batch, head, seq_length_in_this_generation, seq_attend = (
+                        att_tensor.shape
+                    )
+                    assert batch == 1
+                    assert head == num_heads
+                    combined_attentions[
+                        layer_idx,
+                        :,
+                        seq_offset : seq_offset + seq_length_in_this_generation,
+                        :seq_attend,
+                    ] = att_tensor[0, :, :, :]
+
+                seq_offset += seq_length_in_this_generation
+
+            return combined_attentions.cpu().numpy()
+        else:
+            # The last token should have everything
+            # So last token should be (layers [tuple], (batch, head, seq, seq_prompt) [tensor])
+            # We want to be (layers, head, seq, seq_prompt)
+            layers = [layer.squeeze(0).cpu().numpy() for layer in last_token_attentions]
+            # combine the layers
+            return np.stack(layers, axis=0)
+
+    def _get_hidden_states_combined(
+        self,
+        hidden_states,
+        output_tokens,
+    ) -> tuple[np.ndarray, ...] | None:
+        """
+        Different models seem to treat the hidden states differently.
+        Try to parse that out and return (layers: tuple, (seq, hidden): ndarray)
+        """
+        if len(output_tokens) == 0:
+            return None
+        last_token_states = hidden_states[-1]
+        seems_to_be_token_by_token = last_token_states[1].shape[1] == 1
+        if seems_to_be_token_by_token and len(hidden_states) > 1:
+            #  So right now it is (tokens: tuple, layers: tuple, (batch, seq, hidden): tensor)
+            #     where the first seq includes the prompt, and the rest is seq==1 for each token
+            #  We want to stack the layers to get (layers: tuple, (seq, hidden): ndarray)
+            batch_size = last_token_states[1].shape[0]
+            if batch_size != 1:
+                raise NotImplementedError("Batch size > 1 not implemented")
+            num_layers = len(hidden_states[0])
+            layers_tokens_array = [[] for _ in range(num_layers)]
+            for token in hidden_states:
+                for i, layer in enumerate(range(num_layers)):
+                    layers_tokens_array[i].append(token[layer].squeeze(0))
+            layers = [
+                torch.cat(layer, dim=0).cpu().numpy() for layer in layers_tokens_array
+            ]
+            return tuple(layers)
+        else:
+            # The last token should have everything
+            # So last token should be (layers [tuple], (batch, seq, hidden) [tensor])
+            # We want to be (layers [tuple], (seq, hidden) [ndarray])
+            layers = [layer.squeeze(0).cpu().numpy() for layer in last_token_states]
+            return tuple(layers)
+
     def _predict_maybe_cached(
         self,
         prompt: LmPrompt,
     ) -> LmPrediction | list[LmPrediction]:
         if torch.cuda.is_available():
             pre_memory = torch.cuda.memory_allocated()
```

### Comparing `lmwrapper-0.8.7.6/lmwrapper/huggingface_wrapper/wrapper.py` & `lmwrapper-0.9.0.2/lmwrapper/huggingface_wrapper/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from pathlib import Path
 from typing import Literal
 
 from packaging import version
 
 from lmwrapper.env import _MPS_ENABLED, _ONNX_RUNTIME, _QUANTIZATION_ENABLED
 from lmwrapper.huggingface_wrapper.predictor import HuggingFacePredictor
+from lmwrapper.huggingface_wrapper.utilstorch import log_cuda_mem
 from lmwrapper.prompt_trimming import PromptTrimmer
 from lmwrapper.runtime import Runtime
 from lmwrapper.structs import LmPrompt
-from lmwrapper.huggingface_wrapper.utilstorch import log_cuda_mem
 
 try:
     import torch
 
     assert version.parse(torch.__version__) >= version.parse("2.0")
 except ImportError:
     msg = "Expect to work on torch. Please see https://pytorch.org/ for install info."
@@ -367,20 +367,19 @@
         }
     elif model.startswith("Salesforce/codet5") and not model.endswith("b"):
         model_class = T5ForConditionalGeneration
 
         # T5 class does not support this arg,
         # only autoclasses do
         _kwargs.pop("trust_remote_code", None)
-    elif model.startswith("Salesforce/codet5p-") and model.endswith("b"):
-        model_class = AutoModelForSeq2SeqLM
-        _kwargs |= {
-            "low_cpu_mem_usage": True,
-        }
-    elif model == "Salesforce/instructcodet5p-16b":
+    elif (
+        model.startswith("Salesforce/codet5p-")
+        and model.endswith("b")
+        or model == "Salesforce/instructcodet5p-16b"
+    ):
         model_class = AutoModelForSeq2SeqLM
         _kwargs |= {
             "low_cpu_mem_usage": True,
         }
     elif model.startswith("codellama/CodeLlama-"):
         _kwargs |= {
             "low_cpu_mem_usage": True,
```

### Comparing `lmwrapper-0.8.7.6/lmwrapper/openai_wrapper/wrapper.py` & `lmwrapper-0.9.0.2/lmwrapper/openai_wrapper/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 import re
 import time
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
 
 import tiktoken
-
 from openai import OpenAI, RateLimitError
 from openai.types.completion_choice import Logprobs
-from openai.types.chat.chat_completion_token_logprob import TopLogprob
 
 from lmwrapper.abstract_predictor import LmPredictor
 from lmwrapper.secrets_manager import (
     SecretEnvVar,
     SecretFile,
     SecretInterface,
     assert_is_a_secret,
@@ -137,16 +135,16 @@
                 msg,
             )
 
         if isinstance(self.metad.logprobs, Logprobs):
             return self.metad.logprobs.top_logprobs
 
         top_logprobs = []
-        for p in self.metad.logprobs.content: # for each token
-            odict = dict([ (t.token,t.logprob) for t in p.top_logprobs ])
+        for p in self.metad.logprobs.content:  # for each token
+            odict = dict([(t.token, t.logprob) for t in p.top_logprobs])
             top_logprobs.append(odict)
         return top_logprobs
 
 
 class OpenAiLmChatPrediction(LmPrediction):
     pass
 
@@ -261,17 +259,14 @@
                 len(prompt.get_text_as_chat()) * 3
             )  # Extra buffer for each turn transition
             val += 2  # Extra setup tokens
         else:
             val = len(self._tokenizer.encode(prompt.get_text_as_string_default_form()))
         return val
 
-
-
-
     def _predict_maybe_cached(
         self,
         prompt: LmPrompt,
     ) -> LmPrediction | list[LmPrediction]:
         if PRINT_ON_PREDICT:
             print("RUN PREDICT ", prompt.text[: min(10, len(prompt.text))])
 
@@ -343,14 +338,15 @@
             return choice.text if not self._chat_mode else choice.message.content
 
         out = [
             OpenAiLmPrediction(
                 get_completion_text(get_text_from_choice(choice)),
                 prompt,
                 choice,
+                internals=None,
             )
             for choice in choices
         ]
         if len(choices) == 1:
             return out[0]
         return out
```

### Comparing `lmwrapper-0.8.7.6/lmwrapper/prompt_trimming.py` & `lmwrapper-0.9.0.2/lmwrapper/prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/runtime.py` & `lmwrapper-0.9.0.2/lmwrapper/runtime.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/secrets_manager.py` & `lmwrapper-0.9.0.2/lmwrapper/secrets_manager.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/structs.py` & `lmwrapper-0.9.0.2/lmwrapper/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import contextlib
 import statistics
 from dataclasses import dataclass
-from typing import Any, Union
+from typing import Any, Optional, Union
 
+from lmwrapper.interals import ModelInternalsResults
 from lmwrapper.utils import StrEnum
 
 LM_CHAT_DIALOG_COERCIBLE_TYPES = Union[
     str,
     list[Union["LmChatTurn", tuple[str, str], dict, str]],
     "LmChatDialog",
 ]  # Defines a set of types that can be converted into a LmChatDialog
@@ -90,14 +91,16 @@
     By default (None), we will add a bos token if the tokenizer does not seem to
     add one by default, and it is not a seq2seq model.
     Set to True to always add a bos token.
     Set to False to never add a bos token (but the tokenizer might still add one).
     """
     add_special_tokens: bool = True
     """Whether or not to add special tokens when encoding the prompt."""
+    model_internals_request: Optional["ModelInternalsRequest"] = None
+    """Used to attempt to get hidden states and attentions from the model."""
 
     # TODO: make a auto_reduce_max_tokens to reduce when might go over.
 
     def __post_init__(self):
         if self.max_tokens is not None and not isinstance(self.max_tokens, int):
             msg = "The max_tokens parameter should be an int."
             raise ValueError(msg)
@@ -264,14 +267,15 @@
 
 
 @dataclass
 class LmPrediction:
     completion_text: str
     prompt: LmPrompt
     metad: Any
+    internals: ModelInternalsResults | None
 
     def __post_init__(self):
         self._was_cached = False
 
     @property
     def was_cached(self) -> bool:
         return hasattr(self, "_was_cached") and self._was_cached
@@ -351,21 +355,19 @@
     @property
     def top_token_logprobs(self) -> list[dict[str, float]]:
         if self.prompt.logprobs == 1:
             # If we only have a single logprob, then we can adapt the
             #   logprob property into a list of dictionaries. This allows
             #   partial support for implementations that support only that.
             return [
-                {
-                    token: float(logprob)
-                }
+                {token: float(logprob)}
                 for token, logprob in zip(
                     self.completion_tokens,
                     self.completion_logprobs,
-                    strict=True
+                    strict=True,
                 )
             ]
         msg = "This version of prediction does not support top token logprobs"
         raise NotImplementedError(
             msg,
         )
```

### Comparing `lmwrapper-0.8.7.6/lmwrapper/togethertoy.py` & `lmwrapper-0.9.0.2/lmwrapper/togethertoy.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/utils.py` & `lmwrapper-0.9.0.2/lmwrapper/utils.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper/wrapping_config.py` & `lmwrapper-0.9.0.2/lmwrapper/wrapping_config.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/lmwrapper.egg-info/PKG-INFO` & `lmwrapper-0.9.0.2/lmwrapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lmwrapper
-Version: 0.8.7.6
+Version: 0.9.0.2
 Summary: Wrapper around language model APIs
 Author-email: David Gros <DNGros@users.noreply.github.com>, Claudio Spiess <claudiosv@users.noreply.github.com>
 Project-URL: Homepage, https://github.com/DaiseyCode/lmwrapper
 Keywords: large language models,openai
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `lmwrapper-0.8.7.6/lmwrapper.egg-info/SOURCES.txt` & `lmwrapper-0.9.0.2/lmwrapper.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.md
 pyproject.toml
 lmwrapper/_TokenStoppingCriteria.py
 lmwrapper/__init__.py
 lmwrapper/abstract_predictor.py
 lmwrapper/caching.py
 lmwrapper/env.py
+lmwrapper/interals.py
 lmwrapper/prompt_trimming.py
 lmwrapper/runtime.py
 lmwrapper/secrets_manager.py
 lmwrapper/structs.py
 lmwrapper/togethertoy.py
 lmwrapper/utils.py
 lmwrapper/wrapping_config.py
@@ -23,13 +24,14 @@
 lmwrapper/huggingface_wrapper/utilstorch.py
 lmwrapper/huggingface_wrapper/wrapper.py
 lmwrapper/openai_wrapper/__init__.py
 lmwrapper/openai_wrapper/wrapper.py
 test/test_caching.py
 test/test_docs.py
 test/test_huggingface.py
+test/test_huggingface_internals.py
 test/test_huggingface_memory.py
 test/test_models_common.py
 test/test_openai.py
 test/test_prompt_trimming.py
 test/test_structs.py
 test/test_util.py
```

### Comparing `lmwrapper-0.8.7.6/pyproject.toml` & `lmwrapper-0.9.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 [tool.setuptools.packages.find]
 where = ["."]
 include = ["lmwrapper*"]
 
 [project]
 name = "lmwrapper"
-version = "0.8.7.6"
+version = "0.9.0.2"
 authors = [
     { name = "David Gros", email = "DNGros@users.noreply.github.com" },
     { name = "Claudio Spiess", email = "claudiosv@users.noreply.github.com" },
 ]
 description = "Wrapper around language model APIs"
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `lmwrapper-0.8.7.6/test/test_caching.py` & `lmwrapper-0.9.0.2/test/test_caching.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/test/test_docs.py` & `lmwrapper-0.9.0.2/test/test_docs.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/test/test_huggingface.py` & `lmwrapper-0.9.0.2/test/test_huggingface.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     _expand_offsets_to_a_token_index_for_every_text_index,
     _get_token_offsets,
 )
 from lmwrapper.prompt_trimming import HfTokenTrimmer
 from lmwrapper.runtime import Runtime
 from lmwrapper.structs import LmPrompt
 from lmwrapper.utils import StrEnum
+import os
 
 
 class Models(StrEnum):
     CodeT5plus_220M = "Salesforce/codet5p-220m"
     CodeT5plus_6B = "Salesforce/codet5p-6b"
+    CodeGen_350M = "Salesforce/codegen-350M-mono"
     CodeGen2_1B = "Salesforce/codegen2-1B"
     CodeGen2_3_7B = "Salesforce/codegen2-3_7B"
     InstructCodeT5plus_16B = "Salesforce/instructcodet5p-16b"
     CodeLLama_7B = "codellama/CodeLlama-7b-hf"
     CodeLLama_7B_Instruct = "codellama/CodeLlama-7b-Instruct-hf"
     DistilGPT2 = "distilgpt2"
     GPT2 = "gpt2"
@@ -34,20 +36,22 @@
     SMALL_GPU = (
         CUDA_UNAVAILABLE or torch.cuda.mem_get_info()[0] < 17_179_869_184
     )  # 16GB
 except RuntimeError:
     SMALL_GPU = True
 
 SEQ2SEQ_MODELS = {Models.CodeT5plus_220M}
-CAUSAL_MODELS = {Models.DistilGPT2, Models.GPT2, Models.CodeGen2_1B}
+CAUSAL_MODELS = {Models.DistilGPT2, Models.GPT2}
 BIG_SEQ2SEQ_MODELS = {Models.CodeT5plus_6B, Models.InstructCodeT5plus_16B}
-BIG_CAUSAL_MODELS = {Models.CodeGen2_3_7B, Models.Mistral_7B}
+BIG_CAUSAL_MODELS = {Models.CodeGen2_1B, Models.CodeGen2_3_7B, Models.Mistral_7B}
 BIG_MODELS = BIG_SEQ2SEQ_MODELS | BIG_CAUSAL_MODELS
 ALL_MODELS = SEQ2SEQ_MODELS | CAUSAL_MODELS | BIG_MODELS
 
+IS_GITHUB_ACTIONS = os.getenv("GITHUB_ACTIONS") == "true"
+
 
 @pytest.mark.slow()
 @pytest.mark.parametrize("model", [Models.CodeLLama_7B])
 def test_code_llama_autoregressive(model):
     """7B and 13B *base* models can be used for text/code completion"""
     lm = get_huggingface_lm(
         model,
@@ -846,14 +850,16 @@
     print("Expected", expected_offsets)
     assert expected_offsets[:3] == [0, 1, 4]
     offsets = _get_token_offsets(tokenizer, token_ids)
     starts, ends = zip(*offsets, strict=False)
     assert list(starts) == expected_offsets
 
 
+#@pytest.mark.skipif(IS_GITHUB_ACTIONS, reason="Can't load tokenizer on GitHub Actions")
+@pytest.mark.skip(reason="Mistral seems broken with gating error")
 def test_offsets_for_mistral():
     model_name = Models.Mistral_7B
     from transformers import AutoTokenizer
 
     tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=True)
     # token_ids = [2287,  2682,   618, 2287, 2682]
     # assert ' ' + tokenizer.decode(token_ids) == '    print("    print'
@@ -862,14 +868,16 @@
     assert offsets == [
         (0, len("▁▁▁")),
         (3, 3 + len("▁print")),
         (3 + len("▁print"), 3 + len("▁print") + len('("')),
     ]
 
 
+#@pytest.mark.skipif(IS_GITHUB_ACTIONS, reason="Can't load tokenizer on GitHub Actions")
+@pytest.mark.skip(reason="Mistral seems broken with gating error")
 def test_offsets_for_mistral2():
     model_name = Models.Mistral_7B
     from transformers import AutoTokenizer
 
     tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=True)
     token_ids = [618, 2287, 2682, 618]
     offsets = _get_token_offsets(tokenizer, token_ids)
@@ -877,14 +885,16 @@
         (0, len('("')),
         (2, 2 + len("▁▁▁")),
         (5, 5 + len("▁print")),
         (11, 11 + len('("')),
     ]
 
 
+#@pytest.mark.skipif(IS_GITHUB_ACTIONS, reason="Can't load tokenizer on GitHub Actions")
+@pytest.mark.skip(reason="Mistral seems broken with gating error")
 def test_offsets_for_mistral3():
     model_name = Models.Mistral_7B
     from transformers import AutoTokenizer
 
     tokenizer = AutoTokenizer.from_pretrained(model_name, use_fast=True)
     token_ids = [2682, 618]
     offsets = _get_token_offsets(tokenizer, token_ids)
@@ -1027,12 +1037,14 @@
     )
     assert resp.completion_text in {
         "('hello world')",
         '("hello world")',
     }
 
 
+#@pytest.mark.skipif(IS_GITHUB_ACTIONS, reason="Can't load tokenizer on GitHub Actions")
+@pytest.mark.skip(reason="Mistral seems broken with gating error")
 def test_check_tokenizer_check():
     mistral_tokenizer = AutoTokenizer.from_pretrained(Models.Mistral_7B, use_fast=True)
     assert _check_tokenizer_to_see_if_adds_bos(mistral_tokenizer, True)
     gpt2_tokenizer = AutoTokenizer.from_pretrained(Models.DistilGPT2, use_fast=True)
     assert not _check_tokenizer_to_see_if_adds_bos(gpt2_tokenizer, True)
```

### Comparing `lmwrapper-0.8.7.6/test/test_huggingface_memory.py` & `lmwrapper-0.9.0.2/test/test_huggingface_memory.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/test/test_models_common.py` & `lmwrapper-0.9.0.2/test/test_models_common.py`

 * *Files 0% similar despite different names*

```diff
@@ -615,31 +615,32 @@
     )
     pred_dict = pred.dict_serialize()
     from pprint import pprint
 
     pprint(pred_dict)
 
 
-@pytest.mark.skip(reason="Huggingface does not support completion_token_offsets currently")
+@pytest.mark.skip(
+    reason="Huggingface does not support completion_token_offsets currently",
+)
 @pytest.mark.parametrize("lm", ALL_MODELS)
 def test_token_offsets(lm):
     prompt = "A B C D E F G H"
     pred = lm.predict(
         LmPrompt(
             prompt,
             max_tokens=3,
             cache=False,
             temperature=0,
         ),
     )
     assert pred.completion_text == " I J K"
     assert pred.completion_tokens == [" I", " J", " K"]
     base_len = len(prompt)
-    assert pred.completion_token_offsets == [
-        base_len + 0, base_len + 2, base_len + 4]
+    assert pred.completion_token_offsets == [base_len + 0, base_len + 2, base_len + 4]
 
 
 @pytest.mark.parametrize("lm", ALL_MODELS)
 def test_token_offsets(lm):
     prompt = "A B C D E F G H"
     pred = lm.predict(
         LmPrompt(
@@ -654,9 +655,7 @@
     assert pred.completion_tokens == [" I", " J", " K"]
     top_probs = pred.top_token_logprobs
     assert len(top_probs) == 3
     for i, expected in enumerate([" I", " J", " K"]):
         assert isinstance(top_probs[i][expected], float)
         assert top_probs[i][expected] == pred.completion_logprobs[i]
         assert top_probs[i][expected] < 0
-
-
```

### Comparing `lmwrapper-0.8.7.6/test/test_openai.py` & `lmwrapper-0.9.0.2/test/test_openai.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import pytest
 
 from lmwrapper.caching import clear_cache_dir
 from lmwrapper.openai_wrapper.wrapper import (
     OpenAiInstantiationHook,
     OpenAiModelNames,
     OpenAIPredictor,
-    get_open_ai_lm, parse_backoff_time,
+    get_open_ai_lm,
+    parse_backoff_time,
 )
 from lmwrapper.structs import LmChatDialog, LmPrompt
 
 
 def play_with_probs():
     lm = get_open_ai_lm()
     out = lm.predict(
@@ -96,31 +97,36 @@
             num_completions=1,
             temperature=0.0,
             cache=False,
         ),
     )
     assert out.completion_text.strip() == "4"
 
+
 def test_chat_nologprob_exception():
     lm = get_open_ai_lm(OpenAiModelNames.gpt_3_5_turbo)
     out = lm.predict(
         LmPrompt(
             "What is 2+2? Answer with just one number.",
             max_tokens=1,
             num_completions=1,
             temperature=0.0,
             cache=False,
             logprobs=0,
         ),
     )
-    with pytest.raises(ValueError, match="Response does not contain top_logprobs.") as exc_info:
+    with pytest.raises(
+        ValueError,
+        match="Response does not contain top_logprobs.",
+    ) as exc_info:
         out.top_token_logprobs
 
     assert type(exc_info.value) is ValueError
 
+
 def test_simple_chat_mode_multiturn():
     lm = get_open_ai_lm(OpenAiModelNames.gpt_3_5_turbo)
     prompt = [
         "What is 2+2? Answer with just one number.",
         "4",
         "What is 3+2?",
     ]
@@ -338,28 +344,40 @@
     lm = get_open_ai_lm(OpenAiModelNames.gpt_3_5_turbo)
     tokens = lm.tokenize("I like pie")
     assert tokens == ["I", " like", " pie"]
 
 
 def test_backoff_parse():
     mock_exception = MagicMock()
-    mock_exception.message = "Rate limit reached for gpt-3.5-turbo-instruct in organization on tokens per min (TPM): Limit 90000, Used 89007, Requested 2360. Please try again in 1.42s. Visit https://platform.openai.com/account/rate-limits to learn more."
+    mock_exception.message = (
+        "Rate limit reached for gpt-3.5-turbo-instruct in organization on tokens per"
+        " min (TPM): Limit 90000, Used 89007, Requested 2360. Please try again in"
+        " 1.42s. Visit https://platform.openai.com/account/rate-limits to learn more."
+    )
     backoff = parse_backoff_time(mock_exception)
     assert backoff == 2
 
 
 def test_backoff_parse2():
     mock_exception = MagicMock()
-    mock_exception.message = "Rate limit reached for gpt-3.5-turbo-instruct in organization org on tokens per min (TPM): Limit 90000, Used 89007, Requested 2360. Please try again in 1.42s. Visit https://platform.openai.com/account/rate-limits to learn more."
+    mock_exception.message = (
+        "Rate limit reached for gpt-3.5-turbo-instruct in organization org on tokens"
+        " per min (TPM): Limit 90000, Used 89007, Requested 2360. Please try again in"
+        " 1.42s. Visit https://platform.openai.com/account/rate-limits to learn more."
+    )
     backoff = parse_backoff_time(mock_exception)
     assert backoff == 2
 
 
 def test_backoff_parse3():
     mock_exception = MagicMock()
-    mock_exception.message = "Rate limit reached for gpt-3.5-turbo-instruct in organization org on tokens per min (TPM): Limit 90000, Used 89007, Requested 2360. Please try again in 5s. Visit https://platform.openai.com/account/rate-limits to learn more."
+    mock_exception.message = (
+        "Rate limit reached for gpt-3.5-turbo-instruct in organization org on tokens"
+        " per min (TPM): Limit 90000, Used 89007, Requested 2360. Please try again in"
+        " 5s. Visit https://platform.openai.com/account/rate-limits to learn more."
+    )
     backoff = parse_backoff_time(mock_exception)
     assert backoff == 5
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `lmwrapper-0.8.7.6/test/test_prompt_trimming.py` & `lmwrapper-0.9.0.2/test/test_prompt_trimming.py`

 * *Files identical despite different names*

### Comparing `lmwrapper-0.8.7.6/test/test_structs.py` & `lmwrapper-0.9.0.2/test/test_structs.py`

 * *Files identical despite different names*

