# Comparing `tmp/cltrier_nlp-0.1.3.tar.gz` & `tmp/cltrier_nlp-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cltrier_nlp-0.1.3.tar", max compression
+gzip compressed data, was "cltrier_nlp-0.1.4.tar", max compression
```

## Comparing `cltrier_nlp-0.1.3.tar` & `cltrier_nlp-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      633 2024-04-30 12:36:28.308254 cltrier_nlp-0.1.3/README.md
--rw-r--r--   0        0        0      507 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/__init__.py
--rw-r--r--   0        0        0     2856 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/corpus/__init__.py
--rw-r--r--   0        0        0     1317 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/corpus/sentence.py
--rw-r--r--   0        0        0     2769 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/encoder/__init__.py
--rw-r--r--   0        0        0      747 2024-05-02 06:39:38.562780 cltrier_nlp-0.1.3/cltrier_nlp/encoder/batch.py
--rw-r--r--   0        0        0     2427 2024-04-30 14:43:45.708769 cltrier_nlp-0.1.3/cltrier_nlp/encoder/pooler.py
--rw-r--r--   0        0        0      417 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/functional/__init__.py
--rw-r--r--   0        0        0      455 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/functional/neural.py
--rw-r--r--   0        0        0     1369 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/functional/text.py
--rw-r--r--   0        0        0       38 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/utility/__init__.py
--rw-r--r--   0        0        0      566 2024-05-02 06:39:38.566113 cltrier_nlp-0.1.3/cltrier_nlp/utility/map.py
--rw-r--r--   0        0        0      997 2024-05-02 06:40:20.503987 cltrier_nlp-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      633 2024-04-30 12:36:28.308254 cltrier_nlp-0.1.4/README.md
+-rw-r--r--   0        0        0      513 2024-05-02 13:39:38.069285 cltrier_nlp-0.1.4/cltrier_nlp/__init__.py
+-rw-r--r--   0        0        0     3357 2024-05-02 13:49:31.124909 cltrier_nlp-0.1.4/cltrier_nlp/corpus/__init__.py
+-rw-r--r--   0        0        0     1601 2024-05-02 13:49:44.304304 cltrier_nlp-0.1.4/cltrier_nlp/corpus/sentence.py
+-rw-r--r--   0        0        0     3041 2024-05-02 13:39:16.910298 cltrier_nlp-0.1.4/cltrier_nlp/encoder/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-02 13:20:39.672728 cltrier_nlp-0.1.4/cltrier_nlp/encoder/batch.py
+-rw-r--r--   0        0        0     2556 2024-05-02 13:44:28.872227 cltrier_nlp-0.1.4/cltrier_nlp/encoder/pooler.py
+-rw-r--r--   0        0        0      454 2024-05-02 13:42:32.691002 cltrier_nlp-0.1.4/cltrier_nlp/functional/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-02 13:21:35.690210 cltrier_nlp-0.1.4/cltrier_nlp/functional/neural.py
+-rw-r--r--   0        0        0     1454 2024-05-02 13:21:45.699761 cltrier_nlp-0.1.4/cltrier_nlp/functional/text.py
+-rw-r--r--   0        0        0       49 2024-05-02 13:38:50.221580 cltrier_nlp-0.1.4/cltrier_nlp/utility/__init__.py
+-rw-r--r--   0        0        0      683 2024-05-02 13:22:04.985564 cltrier_nlp-0.1.4/cltrier_nlp/utility/map.py
+-rw-r--r--   0        0        0     1250 2024-05-02 13:53:34.547101 cltrier_nlp-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1563 1970-01-01 00:00:00.000000 cltrier_nlp-0.1.4/PKG-INFO
```

### Comparing `cltrier_nlp-0.1.3/README.md` & `cltrier_nlp-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cltrier_nlp-0.1.3/cltrier_nlp/corpus/sentence.py` & `cltrier_nlp-0.1.4/cltrier_nlp/corpus/sentence.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,47 +3,70 @@
 import pandas
 import pydantic
 
 from .. import functional
 
 
 class Sentence(pydantic.BaseModel):
+    """
+
+    """
     raw: str
 
-    language: str = None
+    language: str = 'unknown'
     tokens: typing.List[str] = pydantic.Field(default_factory=lambda: [])
 
     def model_post_init(self, __context) -> None:
+        """
 
+        """
         self.raw = self.raw.replace("\n", " ").strip()
 
         if not self.language:
             self.language = functional.text.detect_language(self.raw)
 
         if not self.tokens:
             self.tokens = functional.text.tokenize(self.raw)
 
-    @pydantic.computed_field
+    @pydantic.computed_field  # type: ignore[misc]
     @property
     def bigrams(self) -> typing.List[typing.Tuple[str, ...]]:
+        """
+
+        """
         return functional.text.ngrams(self.tokens, 2)
 
-    @pydantic.computed_field
+    @pydantic.computed_field  # type: ignore[misc]
     @property
     def trigrams(self) -> typing.List[typing.Tuple[str, ...]]:
+        """
+
+        """
         return functional.text.ngrams(self.tokens, 3)
 
-    @pydantic.computed_field
+    @pydantic.computed_field  # type: ignore[misc]
     @property
     def tetragram(self) -> typing.List[typing.Tuple[str, ...]]:
+        """
+
+        """
         return functional.text.ngrams(self.tokens, 4)
 
-    @pydantic.computed_field
+    @pydantic.computed_field  # type: ignore[misc]
     @property
     def pentagram(self) -> typing.List[typing.Tuple[str, ...]]:
+        """
+
+        """
         return functional.text.ngrams(self.tokens, 5)
 
     def to_row(self) -> pandas.Series:
+        """
+
+        """
         return pandas.Series(self.model_dump())
 
     def __len__(self) -> int:
+        """
+
+        """
         return len(self.tokens)
```

### Comparing `cltrier_nlp-0.1.3/cltrier_nlp/encoder/__init__.py` & `cltrier_nlp-0.1.4/cltrier_nlp/encoder/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,65 @@
+"""
+
+"""
 import logging
 import typing
 
 import pydantic
 import torch
 import transformers
 
 from .batch import EncodedBatch
 from .pooler import EncoderPooler
 from .. import functional
 
-__all__ = [EncodedBatch, EncoderPooler]
+__all__ = ["EncodedBatch", "EncoderPooler"]
 
 
 class EncoderArgs(pydantic.BaseModel):
+    """
+
+    """
     model: str = "prajjwal1/bert-tiny"
     layers: typing.List[int] = [-1]
 
     device: str = functional.neural.get_device()
 
     tokenizer: typing.Dict[str, str | int] = dict(
         max_length=512,
         truncation=True,
         return_offsets_mapping=True,
     )
 
 
 class Encoder(torch.nn.Module):
+    """
+
+    """
 
     @functional.timeit
     def __init__(self, args: EncoderArgs = EncoderArgs()):
+        """
+
+        """
         super().__init__()
 
         self.args = args
 
         self.tokenizer = transformers.AutoTokenizer.from_pretrained(args.model)
         self.model = transformers.AutoModel.from_pretrained(
             args.model, output_hidden_states=True
         ).to(self.args.device)
 
         logging.info(self)
 
     def __call__(self, batch: typing.List[str], unpad: bool = True) -> EncodedBatch:
+        """
+
+        """
         encoding, token = self.tokenize(batch)
         embeds: torch.Tensor = self.forward(
             torch.tensor(encoding["input_ids"], device=self.args.device).long(),
             torch.tensor(encoding["attention_mask"], device=self.args.device).short(),
         )
 
         return EncodedBatch(
@@ -55,39 +70,60 @@
             }
             | encoding
         )
 
     def tokenize(
         self, batch: typing.List[str], padding: bool = True
     ) -> typing.Tuple[typing.Dict, typing.List[typing.List[str]]]:
+        """
+
+        """
         return (
             encoding := self.tokenizer(batch, padding=padding, **self.args.tokenizer),
             [self.ids_to_tokens(ids) for ids in encoding["input_ids"]],
         )
 
     def forward(self, ids: torch.Tensor, masks: torch.Tensor) -> torch.Tensor:
+        """
+
+        """
         return (
             torch.stack(
                 [self.model.forward(ids, masks).hidden_states[i] for i in self.args.layers]
             )
             .sum(0)
             .squeeze()
         )
 
     def ids_to_tokens(self, ids: torch.Tensor) -> typing.List[str]:
+        """
+
+        """
         return self.tokenizer.convert_ids_to_tokens(ids)
 
     def ids_to_sent(self, ids: torch.Tensor) -> str:
+        """
+
+        """
         return self.tokenizer.decode(ids, skip_special_tokens=True)
 
     @property
     def dim(self) -> int:
+        """
+
+        """
         return self.model.config.to_dict()["hidden_size"]
 
     def __len__(self) -> int:
+        """
+
+        """
         return self.model.config.to_dict()["vocab_size"]
 
     def __repr__(self) -> str:
+        """
+
+        """
         return (
             f'> Encoder Name: {self.model.config.__dict__["_name_or_path"]}\n'
             f"  Memory Usage: {functional.neural.calculate_model_memory_usage(self.model)}"
         )
```

### Comparing `cltrier_nlp-0.1.3/cltrier_nlp/encoder/batch.py` & `cltrier_nlp-0.1.4/cltrier_nlp/encoder/batch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import typing
 
 import pydantic
 import torch
 
 
 class EncodedBatch(pydantic.BaseModel):
+    """
+
+    """
     embeds: typing.List[torch.Tensor]
     token: typing.List[typing.List[str]]
 
     input_ids: typing.List[typing.List[int]]
     token_type_ids: typing.List[typing.List[int]]
 
     attention_mask: typing.List[typing.List[int]]
```

### Comparing `cltrier_nlp-0.1.3/cltrier_nlp/encoder/pooler.py` & `cltrier_nlp-0.1.4/cltrier_nlp/encoder/pooler.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import pydantic
 import torch
 
 from .batch import EncodedBatch
 
 
 class EncoderPoolerArgs(pydantic.BaseModel):
+    """
+
+    """
     fns: typing.Dict[str, typing.Callable] = {
         # sentence based
         "sent_cls": lambda x: x[0],
         "sent_mean": lambda x: torch.mean(x[1:-1], dim=0),
         # word based, positional extraction
         "subword_first": lambda x: x[0],
         "subword_last": lambda x: x[-1],
@@ -28,21 +31,27 @@
         "subword_mean",
         "subword_min",
         "subword_max",
     ] = "sent_cls"
 
 
 class EncoderPooler:
+    """
+
+    """
 
     def __call__(
         self,
         encodes: EncodedBatch,
-        extract_spans: typing.List[typing.Tuple[int, int]] = None,
+        extract_spans: typing.Union[typing.List[typing.Tuple[int, int]], None] = None,
         form=EncoderPoolerArgs().types,
     ) -> typing.List[torch.Tensor]:
+        """
+
+        """
 
         if form not in ["sent_cls", "sent_mean"] and not extract_spans:
             raise ValueError("Please provide a list of span values to extract.")
 
         return [
             EncoderPoolerArgs().fns[form](embed)
             for embed in (
@@ -50,24 +59,30 @@
                 if form in ["sent_cls", "sent_mean"]
                 else EncoderPooler._extract_embed_spans(encodes, extract_spans)
             )
         ]
 
     @staticmethod
     def _extract_embed_spans(encodes: EncodedBatch, extract_spans) -> typing.Generator:
+        """
+
+        """
         for span, mapping, embeds in zip(extract_spans, encodes.offset_mapping, encodes.embeds):
             emb_span_idx = EncoderPooler._get_token_idx(
                 mapping[1 : embeds.size(dim=0) - 1], span
             )
             yield embeds[emb_span_idx[0] : emb_span_idx[1] + 1]
 
     @staticmethod
     def _get_token_idx(
         mapping: typing.List[typing.Tuple[int, int]], c_span: typing.Tuple[int, int]
     ) -> typing.Tuple[int, int]:
+        """
+
+        """
         def prep_map(pos):
             return list(enumerate(list(zip(*mapping))[pos]))
 
         span: typing.Tuple[int, int] = (
             next(eid for eid, cid in reversed(prep_map(0)) if cid <= c_span[0]),
             next(eid for eid, cid in prep_map(1) if cid >= c_span[1]),
         )
```

### Comparing `cltrier_nlp-0.1.3/cltrier_nlp/functional/text.py` & `cltrier_nlp-0.1.4/cltrier_nlp/functional/text.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,42 +3,57 @@
 
 import langcodes
 import langdetect
 import nltk
 
 
 def load_stopwords(languages: typing.List[str]) -> typing.List[str]:
+    """
+
+    """
     return list(
         set().union(
             *[
                 nltk.corpus.stopwords.words(lang)
                 for lang in languages
                 if lang in nltk.corpus.stopwords.fileids()
             ]
         )
     )
 
 
 def sentenize(text: str) -> typing.List[str]:
+    """
+
+    """
     return nltk.tokenize.sent_tokenize(text, language=detect_language(text))
 
 
 def tokenize(text: str) -> typing.List[str]:
+    """
+
+    """
     try:
         return nltk.tokenize.word_tokenize(text.lower(), language=detect_language(text))
 
     except LookupError:
         return nltk.tokenize.word_tokenize(text.lower())
 
 
 def ngrams(tokens: typing.List[str], n: int) -> typing.List[typing.Tuple[str, ...]]:
+    """
+
+    """
     return [tuple(tokens[i : i + n]) for i in range(len(tokens) - n + 1)]
 
 
 def detect_language(content: str) -> str:
+    """
+
+    """
     # Ignore langcodes dependent language data warning
     # DeprecationWarning: pkg_resources is deprecated as an API.
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", category=DeprecationWarning)
 
         try:
             return langcodes.Language.get(langdetect.detect(content)).display_name().lower()
```

### Comparing `cltrier_nlp-0.1.3/cltrier_nlp/utility/map.py` & `cltrier_nlp-0.1.4/cltrier_nlp/utility/map.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,32 @@
 import typing
 
 
 class Map:
+    """
+
+    """
 
     def __init__(self, keys: typing.Set[str]) -> None:
+        """
+
+        """
         self.keys2ids: typing.Dict[str, int] = {key: idx for idx, key in enumerate(keys)}
         self.ids2keys: typing.Dict[int, str] = {idx: key for key, idx in self.keys2ids.items()}
 
     def get_ids(self, keys: typing.List[str]) -> typing.List[int]:
+        """
+
+        """
         return [self.keys2ids[key] for key in keys]
 
     def get_keys(self, ids: typing.List[int]) -> typing.List[str]:
+        """
+
+        """
         return [self.ids2keys[idx] for idx in ids]
 
     def __len__(self):
+        """
+
+        """
         return len(self.keys2ids)
```

### Comparing `cltrier_nlp-0.1.3/pyproject.toml` & `cltrier_nlp-0.1.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "cltrier_nlp"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Simon Münker <muenker@uni-trier.de>"]
 readme = "README.md"
 license = "Apache-2.0"
 repository = "https://github.com/simon-muenker/cltrier_nlp"
 classifiers = [
     "Development Status :: 3 - Alpha",
@@ -20,31 +20,40 @@
 [tool.poetry.dependencies]
 python = "^3.11"
 nltk = "^3.8.1"
 pydantic = "^2.7.1"
 langdetect = "^1.0.9"
 langcodes = "^3.4.0"
 transformers = "^4.40.1"
-torch = "^2.3.0"
+torch = "^2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.1.1"
+pre-commit = "^3.7.0"
+ruff = "^0.4.2"
+mypy = "^1.10.0"
+
+[tool.poetry.group.docs.dependencies]
+mkdocs = "^1.6.0"
+mkdocstrings = { version = "^0.25.0", extras = ["python"] }
+mkdocs-literate-nav = "^0.6.1"
+mkdocs-gen-files = "^0.5.0"
+mkdocs-section-index = "^0.3.9"
+
+[tool.poetry.group.examples.dependencies]
 jupyter = "^1.0.0"
 pandas = "^2.2.2"
 matplotlib = "^3.8.4"
 seaborn = "^0.13.2"
-pre-commit = "^3.7.0"
-black = "^24.4.2"
-ruff = "^0.4.2"
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "DEBUG"
 testpaths = [
     "tests",
 ]
 
-[tool.black]
-line-length = 96
-
 [tool.ruff]
 line-length = 96
+
+[tool.mypy]
+files = "cltrier_nlp"
```

### Comparing `cltrier_nlp-0.1.3/PKG-INFO` & `cltrier_nlp-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cltrier_nlp
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Home-page: https://github.com/simon-muenker/cltrier_nlp
 License: Apache-2.0
 Author: Simon Münker
 Author-email: muenker@uni-trier.de
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Text Processing
 Requires-Dist: langcodes (>=3.4.0,<4.0.0)
 Requires-Dist: langdetect (>=1.0.9,<2.0.0)
 Requires-Dist: nltk (>=3.8.1,<4.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
-Requires-Dist: torch (>=2.3.0,<3.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: transformers (>=4.40.1,<5.0.0)
 Project-URL: Repository, https://github.com/simon-muenker/cltrier_nlp
 Description-Content-Type: text/markdown
 
 # Project Repository: NLP Course (M.Sc. NLP, University Trier)
 
 ## Usage
```

