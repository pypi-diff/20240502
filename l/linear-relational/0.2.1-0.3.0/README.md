# Comparing `tmp/linear_relational-0.2.1.tar.gz` & `tmp/linear_relational-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "linear_relational-0.2.1.tar", max compression
+gzip compressed data, was "linear_relational-0.3.0.tar", max compression
```

## Comparing `linear_relational-0.2.1.tar` & `linear_relational-0.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1069 2024-02-16 14:44:48.999285 linear_relational-0.2.1/LICENSE
--rw-r--r--   0        0        0     9160 2024-02-16 14:44:48.999285 linear_relational-0.2.1/README.md
--rw-r--r--   0        0        0    10932 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/CausalEditor.py
--rw-r--r--   0        0        0     1027 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/Concept.py
--rw-r--r--   0        0        0     4715 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/ConceptMatcher.py
--rw-r--r--   0        0        0     7196 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/Lre.py
--rw-r--r--   0        0        0      559 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/Prompt.py
--rw-r--r--   0        0        0     3460 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/PromptValidator.py
--rw-r--r--   0        0        0      930 2024-02-16 14:44:49.835281 linear_relational-0.2.1/linear_relational/__init__.py
--rw-r--r--   0        0        0     4784 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/TraceLayer.py
--rw-r--r--   0        0        0     2988 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/TraceLayerDict.py
--rw-r--r--   0        0        0     1893 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/balance_grouped_items.py
--rw-r--r--   0        0        0      174 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/constants.py
--rw-r--r--   0        0        0     4242 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/extract_token_activations.py
--rw-r--r--   0        0        0     3523 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/layer_matching.py
--rw-r--r--   0        0        0      270 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/logger.py
--rw-r--r--   0        0        0     9877 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/token_utils.py
--rw-r--r--   0        0        0     2133 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/torch_utils.py
--rw-r--r--   0        0        0     3015 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/util.py
--rw-r--r--   0        0        0     2550 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/lib/verify_answers_match_expected.py
--rw-r--r--   0        0        0        0 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/py.typed
--rw-r--r--   0        0        0    11650 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/training/Trainer.py
--rw-r--r--   0        0        0     6551 2024-02-16 14:44:49.003285 linear_relational-0.2.1/linear_relational/training/train_lre.py
--rw-r--r--   0        0        0      925 2024-02-16 14:44:49.835281 linear_relational-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     9799 1970-01-01 00:00:00.000000 linear_relational-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-02 21:45:01.756913 linear_relational-0.3.0/LICENSE
+-rw-r--r--   0        0        0     9433 2024-05-02 21:45:01.756913 linear_relational-0.3.0/README.md
+-rw-r--r--   0        0        0    10932 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/CausalEditor.py
+-rw-r--r--   0        0        0     1027 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/Concept.py
+-rw-r--r--   0        0        0     4715 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/ConceptMatcher.py
+-rw-r--r--   0        0        0     7196 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/Lre.py
+-rw-r--r--   0        0        0      559 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/Prompt.py
+-rw-r--r--   0        0        0     3460 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/PromptValidator.py
+-rw-r--r--   0        0        0      930 2024-05-02 21:45:02.568920 linear_relational-0.3.0/linear_relational/__init__.py
+-rw-r--r--   0        0        0     4784 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/TraceLayer.py
+-rw-r--r--   0        0        0     2988 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/TraceLayerDict.py
+-rw-r--r--   0        0        0     1893 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/balance_grouped_items.py
+-rw-r--r--   0        0        0       92 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/constants.py
+-rw-r--r--   0        0        0     4242 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/extract_token_activations.py
+-rw-r--r--   0        0        0     3523 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/layer_matching.py
+-rw-r--r--   0        0        0      270 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/logger.py
+-rw-r--r--   0        0        0     9877 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/token_utils.py
+-rw-r--r--   0        0        0     2133 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/torch_utils.py
+-rw-r--r--   0        0        0     3015 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/util.py
+-rw-r--r--   0        0        0     2550 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/lib/verify_answers_match_expected.py
+-rw-r--r--   0        0        0        0 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/py.typed
+-rw-r--r--   0        0        0    11936 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/training/Trainer.py
+-rw-r--r--   0        0        0     6551 2024-05-02 21:45:01.756913 linear_relational-0.3.0/linear_relational/training/train_lre.py
+-rw-r--r--   0        0        0      947 2024-05-02 21:45:02.568920 linear_relational-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    10072 1970-01-01 00:00:00.000000 linear_relational-0.3.0/PKG-INFO
```

### Comparing `linear_relational-0.2.1/LICENSE` & `linear_relational-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/README.md` & `linear_relational-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # Linear-Relational
 
 [![ci](https://img.shields.io/github/actions/workflow/status/chanind/linear-relational/ci.yaml?branch=main)](https://github.com/chanind/linear-relational)
+[![Codecov](https://img.shields.io/codecov/c/github/chanind/linear-relational/main)](https://codecov.io/gh/chanind/linear-relational)
 [![PyPI](https://img.shields.io/pypi/v/linear-relational?color=blue)](https://pypi.org/project/linear-relational/)
 
 Linear Relational Embeddings (LREs) and Linear Relational Concepts (LRCs) for LLMs using PyTorch and Huggingface Transformers.
 
 Full docs: [https://chanind.github.io/linear-relational](https://chanind.github.io/linear-relational)
 
 ## About
@@ -25,15 +26,18 @@
 
 Linear Relational Concepts (LRCs) represent a concept $(r, o)$ as a direction vector $v$ on subject tokens, and can act like a simple linear classifier. For instance, while a LRE can represent the relation "located in country", we could learn a LRC for "located in the country: France", "located in country: Germany", "located in country: China", etc... This is just the result from passing in an object activation into the inverse LRE equation above.
 
 $$
 v_{o} = W^{\dagger}(o - b)
 $$
 
-For more information on LREs and LRCs, check out [these](https://arxiv.org/abs/2308.09124) [papers](https://arxiv.org/abs/2311.08968).
+For more information on LREs and LRCs, check out the following papers:
+
+- [Identifying Linear Relational Concepts in Large Language Models](https://arxiv.org/abs/2311.08968)
+- [Linearity of Relation Decoding in Transformer Language Models](https://arxiv.org/abs/2308.09124)
 
 ## Installation
 
 ```
 pip install linear-relational
 ```
```

### Comparing `linear_relational-0.2.1/linear_relational/CausalEditor.py` & `linear_relational-0.3.0/linear_relational/CausalEditor.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/Concept.py` & `linear_relational-0.3.0/linear_relational/Concept.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/ConceptMatcher.py` & `linear_relational-0.3.0/linear_relational/ConceptMatcher.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/Lre.py` & `linear_relational-0.3.0/linear_relational/Lre.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/Prompt.py` & `linear_relational-0.3.0/linear_relational/Prompt.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/PromptValidator.py` & `linear_relational-0.3.0/linear_relational/PromptValidator.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/__init__.py` & `linear_relational-0.3.0/linear_relational/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 
 from .CausalEditor import (
     CausalEditor,
     ConceptSwapAndPredictGreedyRequest,
     ConceptSwapRequest,
 )
 from .Concept import Concept
```

### Comparing `linear_relational-0.2.1/linear_relational/lib/TraceLayer.py` & `linear_relational-0.3.0/linear_relational/lib/TraceLayer.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/TraceLayerDict.py` & `linear_relational-0.3.0/linear_relational/lib/TraceLayerDict.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/balance_grouped_items.py` & `linear_relational-0.3.0/linear_relational/lib/balance_grouped_items.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/extract_token_activations.py` & `linear_relational-0.3.0/linear_relational/lib/extract_token_activations.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/layer_matching.py` & `linear_relational-0.3.0/linear_relational/lib/layer_matching.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/token_utils.py` & `linear_relational-0.3.0/linear_relational/lib/token_utils.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/torch_utils.py` & `linear_relational-0.3.0/linear_relational/lib/torch_utils.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/util.py` & `linear_relational-0.3.0/linear_relational/lib/util.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/lib/verify_answers_match_expected.py` & `linear_relational-0.3.0/linear_relational/lib/verify_answers_match_expected.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/linear_relational/training/Trainer.py` & `linear_relational-0.3.0/linear_relational/training/Trainer.py`

 * *Files 5% similar despite different names*

```diff
@@ -48,35 +48,43 @@
 
     def train_lre(
         self,
         relation: str,
         subject_layer: int,
         object_layer: int,
         prompts: list[Prompt],
+        max_lre_training_samples: int | None = None,
         object_aggregation: ObjectAggregation = "mean",
         validate_prompts: bool = True,
         validate_prompts_batch_size: int = 4,
         move_to_cpu: bool = False,
         verbose: bool = True,
+        seed: int | str | float = 42,
     ) -> Lre:
         processed_prompts = self._process_relation_prompts(
             relation=relation,
             prompts=prompts,
             validate_prompts=validate_prompts,
             validate_prompts_batch_size=validate_prompts_batch_size,
             verbose=verbose,
         )
+        prompts_by_object = group_items(processed_prompts, lambda p: p.object_name)
+        lre_train_prompts = balance_grouped_items(
+            items_by_group=prompts_by_object,
+            max_total=max_lre_training_samples,
+            seed=seed,
+        )
         return train_lre(
             model=self.model,
             tokenizer=self.tokenizer,
             layer_matcher=self.layer_matcher,
             relation=relation,
             subject_layer=subject_layer,
             object_layer=object_layer,
-            prompts=processed_prompts,
+            prompts=lre_train_prompts,
             object_aggregation=object_aggregation,
             move_to_cpu=move_to_cpu,
         )
 
     def train_relation_concepts(
         self,
         relation: str,
@@ -106,23 +114,23 @@
                 f"Only one valid object found for {relation}. Results may be poor."
             )
         lre_train_prompts = balance_grouped_items(
             items_by_group=prompts_by_object,
             max_total=max_lre_training_samples,
             seed=seed,
         )
-        inv_lre = self.train_lre(
+        inv_lre = train_lre(
+            model=self.model,
+            tokenizer=self.tokenizer,
+            layer_matcher=self.layer_matcher,
             relation=relation,
             subject_layer=subject_layer,
             object_layer=object_layer,
             prompts=lre_train_prompts,
             object_aggregation=object_aggregation,
-            validate_prompts=False,  # we already validated the prompts above
-            validate_prompts_batch_size=validate_prompts_batch_size,
-            verbose=verbose,
         ).invert(inv_lre_rank)
 
         return self.train_relation_concepts_from_inv_lre(
             relation=relation,
             inv_lre=inv_lre,
             prompts=processed_prompts,
             vector_aggregation=vector_aggregation,
```

### Comparing `linear_relational-0.2.1/linear_relational/training/train_lre.py` & `linear_relational-0.3.0/linear_relational/training/train_lre.py`

 * *Files identical despite different names*

### Comparing `linear_relational-0.2.1/pyproject.toml` & `linear_relational-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "linear-relational"
-version = "0.2.1"
+version = "0.3.0"
 description = "A Python library for working with Linear Relational Embeddings (LREs) and Linear Relational Concepts (LRCs) for LLMs"
 authors = ["David Chanin <chanindav@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 transformers = "^4.35.2"
@@ -19,14 +19,15 @@
 isort = "^5.12.0"
 pytest = "^7.4.3"
 torch = "^2.1.1"
 sentencepiece = "^0.1.99"
 protobuf = "^4.25.1"
 furo = "^2023.9.10"
 pygments = "^2.17.2"
+pytest-cov = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
```

### Comparing `linear_relational-0.2.1/PKG-INFO` & `linear_relational-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: linear-relational
-Version: 0.2.1
+Version: 0.3.0
 Summary: A Python library for working with Linear Relational Embeddings (LREs) and Linear Relational Concepts (LRCs) for LLMs
 Author: David Chanin
 Author-email: chanindav@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -13,14 +13,15 @@
 Requires-Dist: tqdm (>=4.0.0)
 Requires-Dist: transformers (>=4.35.2,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Linear-Relational
 
 [![ci](https://img.shields.io/github/actions/workflow/status/chanind/linear-relational/ci.yaml?branch=main)](https://github.com/chanind/linear-relational)
+[![Codecov](https://img.shields.io/codecov/c/github/chanind/linear-relational/main)](https://codecov.io/gh/chanind/linear-relational)
 [![PyPI](https://img.shields.io/pypi/v/linear-relational?color=blue)](https://pypi.org/project/linear-relational/)
 
 Linear Relational Embeddings (LREs) and Linear Relational Concepts (LRCs) for LLMs using PyTorch and Huggingface Transformers.
 
 Full docs: [https://chanind.github.io/linear-relational](https://chanind.github.io/linear-relational)
 
 ## About
@@ -41,15 +42,18 @@
 
 Linear Relational Concepts (LRCs) represent a concept $(r, o)$ as a direction vector $v$ on subject tokens, and can act like a simple linear classifier. For instance, while a LRE can represent the relation "located in country", we could learn a LRC for "located in the country: France", "located in country: Germany", "located in country: China", etc... This is just the result from passing in an object activation into the inverse LRE equation above.
 
 $$
 v_{o} = W^{\dagger}(o - b)
 $$
 
-For more information on LREs and LRCs, check out [these](https://arxiv.org/abs/2308.09124) [papers](https://arxiv.org/abs/2311.08968).
+For more information on LREs and LRCs, check out the following papers:
+
+- [Identifying Linear Relational Concepts in Large Language Models](https://arxiv.org/abs/2311.08968)
+- [Linearity of Relation Decoding in Transformer Language Models](https://arxiv.org/abs/2308.09124)
 
 ## Installation
 
 ```
 pip install linear-relational
 ```
```

