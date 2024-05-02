# Comparing `tmp/cltrier_nlp-0.1.2.tar.gz` & `tmp/cltrier_nlp-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltrier_nlp-0.1.2.tar", max compression
+gzip compressed data, was "cltrier_nlp-0.1.3.tar", max compression
```

## Comparing `cltrier_nlp-0.1.2.tar` & `cltrier_nlp-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,14 @@
--rw-r--r--   0        0        0      633 2024-04-30 12:36:28.308254 cltrier_nlp-0.1.2/README.md
--rw-r--r--   0        0        0       97 2024-04-30 13:14:03.329800 cltrier_nlp-0.1.2/cltrier_nlp/__init__.py
--rw-r--r--   0        0        0     3041 2024-04-30 13:23:21.383752 cltrier_nlp-0.1.2/cltrier_nlp/corpus/__init__.py
--rw-r--r--   0        0        0     1517 2024-04-30 13:23:21.360420 cltrier_nlp-0.1.2/cltrier_nlp/corpus/sentence.py
--rw-r--r--   0        0        0       76 2024-04-30 13:09:41.008679 cltrier_nlp-0.1.2/cltrier_nlp/encoder/__init__.py
--rw-r--r--   0        0        0     2946 2024-04-30 13:23:21.403751 cltrier_nlp-0.1.2/cltrier_nlp/encoder/transformer.py
--rw-r--r--   0        0        0     1373 2024-04-30 13:30:04.998220 cltrier_nlp-0.1.2/cltrier_nlp/util/__init__.py
--rw-r--r--   0        0        0      566 2024-04-30 13:33:55.354114 cltrier_nlp-0.1.2/cltrier_nlp/util/map.py
--rw-r--r--   0        0        0     1030 2024-04-30 13:34:55.501301 cltrier_nlp-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      633 2024-04-30 12:36:28.308254 cltrier_nlp-0.1.3/README.md
+-rw-r--r--   0        0        0      507 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/__init__.py
+-rw-r--r--   0        0        0     2856 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/corpus/__init__.py
+-rw-r--r--   0        0        0     1317 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/corpus/sentence.py
+-rw-r--r--   0        0        0     2769 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/encoder/__init__.py
+-rw-r--r--   0        0        0      747 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/encoder/batch.py
+-rw-r--r--   0        0        0     2427 2024-04-30 14:43:45.708769 cltrier_nlp-0.1.3/cltrier_nlp/encoder/pooler.py
+-rw-r--r--   0        0        0      417 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/functional/__init__.py
+-rw-r--r--   0        0        0      455 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/functional/neural.py
+-rw-r--r--   0        0        0     1369 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/functional/text.py
+-rw-r--r--   0        0        0       38 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/utility/__init__.py
+-rw-r--r--   0        0        0      566 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/utility/map.py
+-rw-r--r--   0        0        0      997 2024-05-02 06:40:20.503987 cltrier_nlp-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.3/PKG-INFO
```

### Comparing `cltrier_nlp-0.1.2/README.md` & `cltrier_nlp-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.2/cltrier_nlp/encoder/transformer.py` & `cltrier_nlp-0.1.3/cltrier_nlp/encoder/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,75 +1,73 @@
 import logging
-import os
 import typing
 
 import pydantic
-
 import torch
 import transformers
 
-from .. import util
-
+from .batch import EncodedBatch
+from .pooler import EncoderPooler
+from .. import functional
 
-os.environ["TOKENIZERS_PARALLELISM"] = "false"
+__all__ = [EncodedBatch, EncoderPooler]
 
 
-class TransformerEncoderArgs(pydantic.BaseModel):
+class EncoderArgs(pydantic.BaseModel):
     model: str = "prajjwal1/bert-tiny"
-    max_length: int = 512
     layers: typing.List[int] = [-1]
 
+    device: str = functional.neural.get_device()
+
+    tokenizer: typing.Dict[str, str | int] = dict(
+        max_length=512,
+        truncation=True,
+        return_offsets_mapping=True,
+    )
+
+
+class Encoder(torch.nn.Module):
 
-class TransformerEncoder:
+    @functional.timeit
+    def __init__(self, args: EncoderArgs = EncoderArgs()):
+        super().__init__()
 
-    @util.timeit
-    def __init__(self, args: TransformerEncoderArgs = TransformerEncoderArgs()):
-        transformers.logging.set_verbosity_error()
         self.args = args
 
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(args.model)
         self.model = transformers.AutoModel.from_pretrained(
             args.model, output_hidden_states=True
-        ).to(util.get_device())
+        ).to(self.args.device)
 
         logging.info(self)
 
-    def __call__(self, batch: typing.List[str], return_unpad: bool = True) -> typing.Dict:
-        token, encoding = self.tokenize(batch)
+    def __call__(self, batch: typing.List[str], unpad: bool = True) -> EncodedBatch:
+        encoding, token = self.tokenize(batch)
         embeds: torch.Tensor = self.forward(
-            torch.tensor(encoding['input_ids'], device=util.get_device()).long(),
-            torch.tensor(encoding['attention_mask'], device=util.get_device()).short(),
+            torch.tensor(encoding["input_ids"], device=self.args.device).long(),
+            torch.tensor(encoding["attention_mask"], device=self.args.device).short(),
         )
 
-        def unpad_output(output: torch.tensor, mask: torch.tensor) -> torch.tensor:
-            return (
-                [v[:n] for v, n in zip(output, torch.tensor(mask).sum(1))]
-                if return_unpad
-                else output
-            )
-
-        return {
-            'embeds': unpad_output(embeds, encoding['attention_mask']),
-            'token': unpad_output(token, encoding['attention_mask']),
-            **encoding,
-        }
+        return EncodedBatch(
+            **{
+                "embeds": embeds,
+                "token": token,
+                "unpad": unpad,
+            }
+            | encoding
+        )
 
     def tokenize(
         self, batch: typing.List[str], padding: bool = True
-    ) -> typing.Tuple[typing.List[typing.List[str]], dict]:
-        encoding = self.tokenizer(
-            batch,
-            padding=padding,
-            max_length=self.args.max_length,
-            truncation=True,
-            return_offsets_mapping=True,
+    ) -> typing.Tuple[typing.Dict, typing.List[typing.List[str]]]:
+        return (
+            encoding := self.tokenizer(batch, padding=padding, **self.args.tokenizer),
+            [self.ids_to_tokens(ids) for ids in encoding["input_ids"]],
         )
 
-        return [self.ids_to_tokens(ids) for ids in encoding['input_ids']], encoding
-
     def forward(self, ids: torch.Tensor, masks: torch.Tensor) -> torch.Tensor:
         return (
             torch.stack(
                 [self.model.forward(ids, masks).hidden_states[i] for i in self.args.layers]
             )
             .sum(0)
             .squeeze()
@@ -79,17 +77,17 @@
         return self.tokenizer.convert_ids_to_tokens(ids)
 
     def ids_to_sent(self, ids: torch.Tensor) -> str:
         return self.tokenizer.decode(ids, skip_special_tokens=True)
 
     @property
     def dim(self) -> int:
-        return self.model.config.to_dict()['hidden_size']
+        return self.model.config.to_dict()["hidden_size"]
 
     def __len__(self) -> int:
-        return self.model.config.to_dict()['vocab_size']
+        return self.model.config.to_dict()["vocab_size"]
 
     def __repr__(self) -> str:
         return (
             f'> Encoder Name: {self.model.config.__dict__["_name_or_path"]}\n'
-            f'  Memory Usage: {util.calculate_model_memory_usage(self.model)}'
+            f"  Memory Usage: {functional.neural.calculate_model_memory_usage(self.model)}"
         )
```

### Comparing `cltrier_nlp-0.1.2/cltrier_nlp/util/map.py` & `cltrier_nlp-0.1.3/cltrier_nlp/utility/map.py`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.2/pyproject.toml` & `cltrier_nlp-0.1.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cltrier_nlp"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Simon Münker <muenker@uni-trier.de>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/simon-muenker/cltrier_nlp"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -40,12 +40,11 @@
 log_cli = true
 log_cli_level = "DEBUG"
 testpaths = [
     "tests",
 ]
 
 [tool.black]
-skip-string-normalization = true
 line-length = 96
 
 [tool.ruff]
 line-length = 96
```

### Comparing `cltrier_nlp-0.1.2/PKG-INFO` & `cltrier_nlp-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltrier_nlp
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Home-page: https://github.com/simon-muenker/cltrier_nlp
 License: Apache-2.0
 Author: Simon Münker
 Author-email: muenker@uni-trier.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
```

