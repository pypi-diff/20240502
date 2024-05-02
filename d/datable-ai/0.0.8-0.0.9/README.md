# Comparing `tmp/datable_ai-0.0.8.tar.gz` & `tmp/datable_ai-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datable_ai-0.0.8.tar", max compression
+gzip compressed data, was "datable_ai-0.0.9.tar", max compression
```

## Comparing `datable_ai-0.0.8.tar` & `datable_ai-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     1068 2024-05-01 08:28:04.000079 datable_ai-0.0.8/LICENSE
--rw-r--r--   0        0        0      426 2024-05-01 08:28:04.000079 datable_ai-0.0.8/README.md
--rw-r--r--   0        0        0      175 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/core/__init__.py
--rw-r--r--   0        0        0     3643 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/core/llm.py
--rw-r--r--   0        0        0      169 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/helper.py
--rw-r--r--   0        0        0     3131 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/ocr.py
--rw-r--r--   0        0        0     5680 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/output.py
--rw-r--r--   0        0        0     2526 2024-05-01 08:28:04.000079 datable_ai-0.0.8/datable_ai/structured_output.py
--rw-r--r--   0        0        0      665 2024-05-01 08:28:04.004079 datable_ai-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 datable_ai-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 05:23:16.204812 datable_ai-0.0.9/LICENSE
+-rw-r--r--   0        0        0      426 2024-05-02 05:23:16.204812 datable_ai-0.0.9/README.md
+-rw-r--r--   0        0        0      175 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/core/__init__.py
+-rw-r--r--   0        0        0     3643 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/core/llm.py
+-rw-r--r--   0        0        0      169 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/helper.py
+-rw-r--r--   0        0        0     3131 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/ocr.py
+-rw-r--r--   0        0        0     5680 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/output.py
+-rw-r--r--   0        0        0     2526 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/structured_output.py
+-rw-r--r--   0        0        0     1846 2024-05-02 05:23:16.204812 datable_ai-0.0.9/datable_ai/transcription.py
+-rw-r--r--   0        0        0      707 2024-05-02 05:23:16.208812 datable_ai-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1344 1970-01-01 00:00:00.000000 datable_ai-0.0.9/PKG-INFO
```

### Comparing `datable_ai-0.0.8/LICENSE` & `datable_ai-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.8/datable_ai/core/llm.py` & `datable_ai-0.0.9/datable_ai/core/llm.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.8/datable_ai/ocr.py` & `datable_ai-0.0.9/datable_ai/ocr.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.8/datable_ai/output.py` & `datable_ai-0.0.9/datable_ai/output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.8/datable_ai/structured_output.py` & `datable_ai-0.0.9/datable_ai/structured_output.py`

 * *Files identical despite different names*

### Comparing `datable_ai-0.0.8/PKG-INFO` & `datable_ai-0.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: datable-ai
-Version: 0.0.8
+Version: 0.0.9
 Summary: datable-ai
 License: MIT
 Author: datable
 Author-email: dev@datable.jp
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: deepgram-sdk (>=3.2.7,<4.0.0)
 Requires-Dist: langchain (>=0.1.16,<0.2.0)
 Requires-Dist: langchain-anthropic (>=0.1.11,<0.2.0)
 Requires-Dist: langchain-openai (>=0.1.3,<0.2.0)
 Requires-Dist: openai (>=1.23.1,<2.0.0)
 Requires-Dist: pillow (>=10.3.0,<11.0.0)
+Requires-Dist: pydub (>=0.25.1,<0.26.0)
 Requires-Dist: pytest (>=8.1.1,<9.0.0)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Project-URL: Repository, https://github.com/datable-inc/datable-ai
 Description-Content-Type: text/markdown
 
 <div align="center">
 <h1>datable-ai</h1>
```

