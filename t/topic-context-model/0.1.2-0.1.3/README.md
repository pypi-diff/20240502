# Comparing `tmp/topic-context-model-0.1.2.tar.gz` & `tmp/topic_context_model-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "topic-context-model-0.1.2.tar", last modified: Thu Mar 21 13:44:19 2024, max compression
+gzip compressed data, was "topic_context_model-0.1.3.tar", last modified: Thu May  2 13:49:30 2024, max compression
```

## Comparing `topic-context-model-0.1.2.tar` & `topic_context_model-0.1.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:44:19.737700 topic-context-model-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-21 13:44:19.737700 topic-context-model-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5810 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 13:44:19.737700 topic-context-model-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:44:19.737700 topic-context-model-0.1.2/tcm/
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/tcm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/tcm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12478 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/tcm/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    12372 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/tcm/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/tcm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-03-21 13:43:57.000000 topic-context-model-0.1.2/tcm/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 13:44:19.737700 topic-context-model-0.1.2/topic_context_model.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-03-21 13:44:19.000000 topic-context-model-0.1.2/topic_context_model.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-03-21 13:44:19.000000 topic-context-model-0.1.2/topic_context_model.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 13:44:19.000000 topic-context-model-0.1.2/topic_context_model.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-21 13:44:19.000000 topic-context-model-0.1.2/topic_context_model.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-21 13:44:19.000000 topic-context-model-0.1.2/topic_context_model.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-21 13:44:19.000000 topic-context-model-0.1.2/topic_context_model.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:30.166454 topic_context_model-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-02 13:49:30.166454 topic_context_model-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:49:30.166454 topic_context_model-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:30.166454 topic_context_model-0.1.3/tcm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/tcm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/tcm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12919 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/tcm/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15008 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/tcm/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/tcm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-02 13:49:11.000000 topic_context_model-0.1.3/tcm/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:49:30.166454 topic_context_model-0.1.3/topic_context_model.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7073 2024-05-02 13:49:30.000000 topic_context_model-0.1.3/topic_context_model.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-02 13:49:30.000000 topic_context_model-0.1.3/topic_context_model.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:49:30.000000 topic_context_model-0.1.3/topic_context_model.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-02 13:49:30.000000 topic_context_model-0.1.3/topic_context_model.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-02 13:49:30.000000 topic_context_model-0.1.3/topic_context_model.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-02 13:49:30.000000 topic_context_model-0.1.3/topic_context_model.egg-info/top_level.txt
```

### Comparing `topic-context-model-0.1.2/LICENSE` & `topic_context_model-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `topic-context-model-0.1.2/PKG-INFO` & `topic_context_model-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-context-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: Topic Context Model (TCM).
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/tcm
 Project-URL: Bug Tracker, http://github.com/jnphilipp/tcm/issues
 Keywords: topic context model,tcm,lda,lsa
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,14 +26,15 @@
 Requires-Dist: scikit-learn~=1.4.0
 
 # Topic Context Modell (TCM)
 
 Calculates the surprisal of a word given a context.
 
 ![Tests](https://github.com/jnphilipp/tcm/actions/workflows/tests.yml/badge.svg)
+[![pypi Version](https://img.shields.io/pypi/v/topic-context-model.svg?logo=pypi&logoColor=white)](https://pypi.org/project/topic-context-model/)
 
 ## Requirements
 
 * Python >= 3.10
 * scipy
 * scikit-learn
```

### Comparing `topic-context-model-0.1.2/README.md` & `topic_context_model-0.1.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Topic Context Modell (TCM)
 
 Calculates the surprisal of a word given a context.
 
 ![Tests](https://github.com/jnphilipp/tcm/actions/workflows/tests.yml/badge.svg)
+[![pypi Version](https://img.shields.io/pypi/v/topic-context-model.svg?logo=pypi&logoColor=white)](https://pypi.org/project/topic-context-model/)
 
 ## Requirements
 
 * Python >= 3.10
 * scipy
 * scikit-learn
```

### Comparing `topic-context-model-0.1.2/pyproject.toml` & `topic_context_model-0.1.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "topic-context-model"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
     {name = "J. Nathanael Philipp", email = "nathanael@philipp.land"}
 ]
 description="Topic Context Model (TCM)."
 readme = "README.md"
 license = {text = "GPLv3+"}
 requires-python = ">=3.10"
```

### Comparing `topic-context-model-0.1.2/tcm/__init__.py` & `topic_context_model-0.1.3/tcm/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 __all__ = ["TopicContextModel"]
 
 __app_name__ = "tcm"
 __author__ = "J. Nathanael Philipp"
 __email__ = "nathanael@philipp.land"
 __copyright__ = "Copyright 2023-2024 J. Nathanael Philipp (jnphilipp)"
 __license__ = "GPLv3"
-__version_info__ = (0, 1, 2)
+__version_info__ = (0, 1, 3)
 __version__ = ".".join(str(e) for e in __version_info__)
 __github__ = "https://github.com/jnphilipp/tcm"
 VERSION = (
     f"%(prog)s v{__version__}\n{__copyright__}\n"
     + "License GPLv3+: GNU GPL version 3 or later <https://gnu.org/licenses/gpl.html>."
     + "\nThis is free software: you are free to change and redistribute it.\n"
     + "There is NO WARRANTY, to the extent permitted by law.\n\n"
```

### Comparing `topic-context-model-0.1.2/tcm/__main__.py` & `topic_context_model-0.1.3/tcm/__main__.py`

 * *Files identical despite different names*

### Comparing `topic-context-model-0.1.2/tcm/app.py` & `topic_context_model-0.1.3/tcm/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     ArgumentDefaultsHelpFormatter,
     ArgumentParser,
     RawTextHelpFormatter,
 )
 from pathlib import Path
 
 from . import __app_name__, VERSION
-from .data import data_load, surprisal_save
+from .data import load, save
 from .model import TopicContextModel
 from .tokenizer import default_tokenizer
 
 
 class ArgFormatter(ArgumentDefaultsHelpFormatter, RawTextHelpFormatter):
     """Combination of ArgumentDefaultsHelpFormatter and RawTextHelpFormatter."""
 
@@ -97,14 +97,26 @@
     )
     parser.add_argument(
         "--surprisal-file-name-part",
         type=str,
         default="-surprisal",
         help="added to the name of input file to when saving surprisal data.",
     )
+    parser.add_argument(
+        "--exclude-pos-tags",
+        nargs="+",
+        default=[],
+        help="exclude words with these PoS-tags.",
+    )
+    parser.add_argument(
+        "--conllu-keyname",
+        type=str,
+        default="surprisal",
+        help="key name to use when saving to CoNLL-U, in misc.",
+    )
 
     # lda
     subparsers = parser.add_subparsers(
         title="models", help="which model to use.", dest="model"
     )
     lda_parser = subparsers.add_parser("lda", help="use LDA as model for TCM.")
     lda_parser.add_argument(
@@ -330,22 +342,23 @@
     logging.basicConfig(
         format=args.log_format,
         level=logging.DEBUG,
         handlers=handlers,
     )
 
     tcm = TopicContextModel.load(args.model_file) if args.model_file.exists() else None
-    data, words, out_of_vocab = data_load(
+    data, words, out_of_vocab = load(
         args.data,
         args.fields,
         None if tcm is None else tcm.words,
         default_tokenizer if args.tokenize else None,
         args.file_as_text,
         args.batch_size,
-        verbose=verbosity,
+        args.exclude_pos_tags,
+        verbosity,
     )
 
     if tcm is None and args.model == "lda":
         tcm = TopicContextModel.LatentDirichletAllocation(
             words,
             args.n_components,
             args.doc_topic_prior,
@@ -386,17 +399,20 @@
         else:
             x = data.copy()
             x.resize((data.shape[0], len(words)))
         tcm.fit(x)
         tcm.save(args.model_file)
     if "surprisal" in args.action:
         surprisal_data = tcm.surprisal(data)
-        surprisal_save(
+        save(
             args.data,
             args.fields,
             surprisal_data,
             words,
             out_of_vocab,
             args.surprisal_file_name_part,
             args.file_as_text,
+            default_tokenizer if args.tokenize else None,
+            args.exclude_pos_tags,
+            args.conllu_keyname,
         )
     return None
```

### Comparing `topic-context-model-0.1.2/tcm/data.py` & `topic_context_model-0.1.3/tcm/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,55 +19,71 @@
 import gzip
 import joblib
 import logging
 import numpy as np
 import re
 
 from collections import Counter
+from conllu import parse_incr, TokenList
 from csv import DictReader, DictWriter, Sniffer
 from joblib import Parallel, delayed
 from scipy.sparse import csr_matrix
 from pathlib import Path
 from typing import Callable
 
 
-def data_load(
+def load(
     paths: str | Path | list[str | Path],
     fields: str | list[str] | None,
     words: list[str] | None = None,
     tokenizer: Callable[[str], list[str]] | None = None,
     file_as_text: bool = False,
     batch_size: int = 128,
+    exclude_pos_tags: list[str] = [],
     verbose: int = 10,
 ) -> tuple[csr_matrix, list[str], dict[int, str]]:
-    """Load texts from text or csv files.
+    """Load texts from text, csv or CoNLL-U files.
 
     Text files need to have a text per line, for csv files fields names need to be
     given. The text needs to betokenized with `;` for senteces and `,` for words.
 
+    For CoNLL-U files the lemma will be used, optionally a list of PoS-tags can be given
+    that will be exclude, the fields for UPOS and XPOS will be checked.
+
     paths: path or list of paths to load texts from
     fields: if files are in csv format, which field to use
+    words: optional list of words (vocab). If given words not in this list will be
+           excluded.
     """
 
-    def convert_line(*texts: str) -> tuple[list[int], list[int]]:
+    def convert(*texts: str | TokenList) -> tuple[list[int], list[int]]:
         data = []
         indices = []
         counter: Counter = Counter()
         for text in texts:
-            if re.fullmatch(r"[^\s]+\t+[^\t]+", text.strip()):
-                idx, text = re.split(r"\t+", text.strip())
-            if tokenizer is not None:
-                counter.update(tokenizer(text.strip()))
-            elif ";" in text and "," in text:
-                for s in text.strip().split(";"):
-                    counter.update(s.split(","))
-            elif "," in text:
-                counter.update(text.strip().split(","))
-            else:
-                raise RuntimeError(f"Unrecognized format for line {text}.")
+            if isinstance(text, str):
+                if re.fullmatch(r"[^\s]+\t+[^\t]+", text.strip()):
+                    idx, text = re.split(r"\t+", text.strip())
+                if tokenizer is not None:
+                    counter.update(tokenizer(text.strip()))
+                elif ";" in text and "," in text:
+                    for s in text.strip().split(";"):
+                        counter.update(s.split(","))
+                elif "," in text:
+                    counter.update(text.strip().split(","))
+                else:
+                    raise RuntimeError(f"Unrecognized format for line {text}.")
+            elif isinstance(text, TokenList):
+                for token in text:
+                    if (
+                        token["upos"] in exclude_pos_tags
+                        or token["xpos"] in exclude_pos_tags
+                    ):
+                        continue
+                    counter.update([token["lemma"]])
         for k, v in counter.items():
             if words is None:
                 idx = vocab.setdefault(k, len(vocab))
             elif k not in vocab:
                 idx = out_of_vocab.setdefault(k, len(vocab) + len(out_of_vocab))
             else:
                 idx = vocab[k]
@@ -89,48 +105,61 @@
     out_of_vocab: dict[str, int] = {}
     for c, path in enumerate(paths):
         if isinstance(path, str):
             path = Path(path)
         logging.info(f"Load data from {path}.")
         if path.name.endswith(".gz"):
             fopen = gzip.open
-        elif path.name.endswith((".txt", ".csv")):
+        elif path.name.endswith((".txt", ".csv", ".conllu")):
             fopen = open
         else:
             raise RuntimeError("Unsopported file type.")
         with fopen(path, "rt", encoding="utf8") as f:
-            if path.name.endswith((".csv", ".csv.gz")):
+            if path.name.endswith((".conllu", ".conllu.gz")):
+                with Parallel(
+                    n_jobs=joblib.cpu_count(),
+                    verbose=verbose,
+                    require="sharedmem",
+                    batch_size=batch_size,
+                ) as parallel:
+                    for i, j in parallel(
+                        [delayed(convert)(tokenlist) for tokenlist in parse_incr(f)]
+                    ):
+                        data += i
+                        indices += j
+                        indptr.append(len(indices))
+            elif path.name.endswith((".csv", ".csv.gz")):
                 assert fields is not None
                 dialect = Sniffer().sniff(f.readline() + f.readline())
                 f.seek(0)
                 reader = DictReader(f, dialect=dialect)
                 with Parallel(
                     n_jobs=joblib.cpu_count(),
                     verbose=verbose,
                     require="sharedmem",
                     batch_size=batch_size,
                 ) as parallel:
                     for i, j in parallel(
                         [
-                            delayed(convert_line)(*(row[field] for field in fields))
+                            delayed(convert)(*(row[field] for field in fields))
                             for row in reader
                         ]
                     ):
                         data += i
                         indices += j
                         indptr.append(len(indices))
             elif path.name.endswith((".txt", ".txt.gz")):
                 with Parallel(
                     n_jobs=joblib.cpu_count(),
                     verbose=verbose,
                     require="sharedmem",
                     batch_size=batch_size,
                 ) as parallel:
                     for i, j in parallel(
-                        [delayed(convert_line)(line.strip()) for line in f]
+                        [delayed(convert)(line.strip()) for line in f]
                     ):
                         data += i
                         indices += j
                         indptr.append(len(indices))
             else:
                 raise RuntimeError("Unsopported file type.")
         if file_as_text:
@@ -150,67 +179,93 @@
             if words is None
             else words
         ),
         {v: k for k, v in sorted(out_of_vocab.items(), key=lambda x: x[1])},
     )
 
 
-def surprisal_save(
+def save(
     paths: str | Path | list[str | Path],
     fields: str | list[str] | None,
     surprisal_data: csr_matrix,
     words: list[str],
     out_of_vocab: dict[int, str],
     surprisal_file_name_part: str = "-surprisal",
     file_as_text: bool = False,
     tokenizer: Callable[[str], list[str]] | None = None,
+    exclude_pos_tags: list[str] = [],
+    conllu_keyname: str = "surprisal",
 ) -> None:
     """Save surprisal values.
 
     Args:
      * paths:
      * fields:
      * surprisal_data:
      * words:
+     * out_of_vocab:
      * surprisal_file_name_part:
      * file_as_text:
      * tokenizer:
+     * exclude_pos_tags:
+     * conllu_keyname:
     """
     if isinstance(paths, str) or isinstance(paths, Path):
         paths = [paths]
 
     rwords = {w: i for i, w in enumerate(words)}
     for k, v in out_of_vocab.items():
         rwords[v] = k
 
     fopen: Callable
     idx = 0
     for path in paths:
         if isinstance(path, str):
             path = Path(path)
         out_path = path.parent / re.sub(
-            r"(.+?)(\.(txt|.csv)(\.gz)?)$",
+            r"(.+?)(\.(txt|csv|conllu)(\.gz)?)$",
             rf"\g<1>{surprisal_file_name_part}\g<2>",
             path.name,
         )
 
         if path.name.endswith(".gz"):
             fopen = gzip.open
-        elif path.name.endswith((".txt", ".csv")):
+        elif path.name.endswith((".txt", ".csv", ".conllu")):
             fopen = open
         else:
             raise RuntimeError("Unsopported file type.")
         with fopen(path, "rt", encoding="utf8") as fr:
             if file_as_text:
                 doc = surprisal_data.getrow(idx).toarray().squeeze()
                 idx += 1
 
             with fopen(out_path, "wt", encoding="utf8") as fw:
                 logging.info(f"Save surprisal data for {path} in {out_path}.")
-                if path.name.endswith((".csv", ".csv.gz")):
+                if path.name.endswith((".conllu", ".conllu.gz")):
+                    for tokenlist in parse_incr(fr):
+                        if not file_as_text:
+                            doc = surprisal_data.getrow(idx).toarray().squeeze()
+                            idx += 1
+                        for token in tokenlist:
+                            if (
+                                token["upos"] in exclude_pos_tags
+                                or token["xpos"] in exclude_pos_tags
+                            ):
+                                continue
+                            if token["lemma"] in rwords:
+                                if "misc" in token and token["misc"]:
+                                    token["misc"][conllu_keyname] = doc[
+                                        rwords[token["lemma"]]
+                                    ]
+                                else:
+                                    token["misc"] = {
+                                        conllu_keyname: doc[rwords[token["lemma"]]]
+                                    }
+                        fw.write(tokenlist.serialize())
+                elif path.name.endswith((".csv", ".csv.gz")):
                     assert fields is not None
                     dialect = Sniffer().sniff(fr.readline() + fr.readline())
                     fr.seek(0)
                     reader = DictReader(fr, dialect=dialect)
                     writer = DictWriter(
                         fw,
                         fr.fieldnames + [f"{field}-surprisal" for field in fields],
```

### Comparing `topic-context-model-0.1.2/tcm/model.py` & `topic_context_model-0.1.3/tcm/model.py`

 * *Files identical despite different names*

### Comparing `topic-context-model-0.1.2/tcm/tokenizer.py` & `topic_context_model-0.1.3/tcm/tokenizer.py`

 * *Files identical despite different names*

### Comparing `topic-context-model-0.1.2/topic_context_model.egg-info/PKG-INFO` & `topic_context_model-0.1.3/topic_context_model.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: topic-context-model
-Version: 0.1.2
+Version: 0.1.3
 Summary: Topic Context Model (TCM).
 Author-email: "J. Nathanael Philipp" <nathanael@philipp.land>
 License: GPLv3+
 Project-URL: Homepage, https://github.com/jnphilipp/tcm
 Project-URL: Bug Tracker, http://github.com/jnphilipp/tcm/issues
 Keywords: topic context model,tcm,lda,lsa
 Classifier: Development Status :: 5 - Production/Stable
@@ -26,14 +26,15 @@
 Requires-Dist: scikit-learn~=1.4.0
 
 # Topic Context Modell (TCM)
 
 Calculates the surprisal of a word given a context.
 
 ![Tests](https://github.com/jnphilipp/tcm/actions/workflows/tests.yml/badge.svg)
+[![pypi Version](https://img.shields.io/pypi/v/topic-context-model.svg?logo=pypi&logoColor=white)](https://pypi.org/project/topic-context-model/)
 
 ## Requirements
 
 * Python >= 3.10
 * scipy
 * scikit-learn
```

