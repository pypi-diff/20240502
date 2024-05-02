# Comparing `tmp/llama_index_readers_docstring_walker-0.1.3.tar.gz` & `tmp/llama_index_readers_docstring_walker-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_docstring_walker-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_readers_docstring_walker-0.1.4.tar", max compression
```

## Comparing `llama_index_readers_docstring_walker-0.1.3.tar` & `llama_index_readers_docstring_walker-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     6577 2024-02-13 13:53:01.757034 llama_index_readers_docstring_walker-0.1.3/README.md
--rw-r--r--   0        0        0      118 2024-02-13 13:53:01.757537 llama_index_readers_docstring_walker-0.1.3/llama_index/readers/docstring_walker/__init__.py
--rw-r--r--   0        0        0     7431 2024-02-13 13:53:01.757603 llama_index_readers_docstring_walker-0.1.3/llama_index/readers/docstring_walker/base.py
--rw-r--r--   0        0        0     1559 2024-02-21 19:45:06.945775 llama_index_readers_docstring_walker-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     7270 1970-01-01 00:00:00.000000 llama_index_readers_docstring_walker-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     6582 2024-05-02 17:02:31.953773 llama_index_readers_docstring_walker-0.1.4/README.md
+-rw-r--r--   0        0        0      118 2024-05-02 17:02:31.953773 llama_index_readers_docstring_walker-0.1.4/llama_index/readers/docstring_walker/__init__.py
+-rw-r--r--   0        0        0     7431 2024-05-02 17:02:31.953773 llama_index_readers_docstring_walker-0.1.4/llama_index/readers/docstring_walker/base.py
+-rw-r--r--   0        0        0     1559 2024-05-02 17:02:31.953773 llama_index_readers_docstring_walker-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     7224 1970-01-01 00:00:00.000000 llama_index_readers_docstring_walker-0.1.4/PKG-INFO
```

### Comparing `llama_index_readers_docstring_walker-0.1.3/README.md` & `llama_index_readers_docstring_walker-0.1.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Very often you have a large code base, with a rich docstrings and comments, that you would like to use to produce documentation. In fact, many open-source libraries like Scikit-learn or PyTorch have docstring so rich, that they contain LaTeX equations, or detailed examples.
 
 At the same time, sometimes LLMs are used to read the full code from a repository, which can cost you many tokens, time and computational power.
 
 DocstringWalker tries to find a sweet spot between these two approaches. You can use it to:
 
 1. Parse all docstrings from modules, classes, and functions in your local code directory.
-2. Convert them do Llama Documents.
+2. Convert them do LlamaIndex Documents.
 3. Feed into LLM of your choice to produce a code-buddy chatbot or generate documentation.
    DocstringWalker utilizes only AST module, to process the code.
 
 **With this tool, you can analyze only docstrings from the code, without the need to use tokens for the code itself.**
 
 # Usage
```

### Comparing `llama_index_readers_docstring_walker-0.1.3/llama_index/readers/docstring_walker/base.py` & `llama_index_readers_docstring_walker-0.1.4/llama_index/readers/docstring_walker/base.py`

 * *Files identical despite different names*

### Comparing `llama_index_readers_docstring_walker-0.1.3/pyproject.toml` & `llama_index_readers_docstring_walker-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 description = "llama-index readers docstring_walker integration"
 exclude = ["**/BUILD"]
 keywords = ["code", "docstring", "python", "source code"]
 license = "MIT"
 maintainers = ["Filip Wojcik"]
 name = "llama-index-readers-docstring-walker"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
```

### Comparing `llama_index_readers_docstring_walker-0.1.3/PKG-INFO` & `llama_index_readers_docstring_walker-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,35 @@
 Metadata-Version: 2.1
 Name: llama-index-readers-docstring-walker
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index readers docstring_walker integration
 License: MIT
 Keywords: code,docstring,python,source code
 Author: Your Name
 Author-email: you@example.com
 Maintainer: Filip Wojcik
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Intro
 
 Very often you have a large code base, with a rich docstrings and comments, that you would like to use to produce documentation. In fact, many open-source libraries like Scikit-learn or PyTorch have docstring so rich, that they contain LaTeX equations, or detailed examples.
 
 At the same time, sometimes LLMs are used to read the full code from a repository, which can cost you many tokens, time and computational power.
 
 DocstringWalker tries to find a sweet spot between these two approaches. You can use it to:
 
 1. Parse all docstrings from modules, classes, and functions in your local code directory.
-2. Convert them do Llama Documents.
+2. Convert them do LlamaIndex Documents.
 3. Feed into LLM of your choice to produce a code-buddy chatbot or generate documentation.
    DocstringWalker utilizes only AST module, to process the code.
 
 **With this tool, you can analyze only docstrings from the code, without the need to use tokens for the code itself.**
 
 # Usage
```

