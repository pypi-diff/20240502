# Comparing `tmp/gptify-0.3.2.tar.gz` & `tmp/gptify-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gptify-0.3.2.tar", max compression
+gzip compressed data, was "gptify-0.3.3.tar", max compression
```

## Comparing `gptify-0.3.2.tar` & `gptify-0.3.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1234 2024-04-19 05:50:39.571396 gptify-0.3.2/README.md
--rw-r--r--   0        0        0      316 2024-04-19 05:50:39.571396 gptify-0.3.2/gptify/.gptignore
--rw-r--r--   0        0        0        0 2024-04-19 05:50:39.571396 gptify-0.3.2/gptify/__init__.py
--rw-r--r--   0        0        0      201 2024-04-19 05:50:39.571396 gptify-0.3.2/gptify/cli.py
--rw-r--r--   0        0        0     4665 2024-04-19 05:50:39.571396 gptify-0.3.2/gptify/gpt_repository_loader.py
--rw-r--r--   0        0        0      465 2024-04-19 05:50:39.571396 gptify-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1234 2024-05-02 05:16:24.293395 gptify-0.3.3/README.md
+-rw-r--r--   0        0        0      319 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/.gptignore
+-rw-r--r--   0        0        0        0 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/__init__.py
+-rw-r--r--   0        0        0      201 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/cli.py
+-rw-r--r--   0        0        0     4665 2024-05-02 05:16:24.293395 gptify-0.3.3/gptify/gpt_repository_loader.py
+-rw-r--r--   0        0        0      465 2024-05-02 05:16:24.293395 gptify-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     1760 1970-01-01 00:00:00.000000 gptify-0.3.3/PKG-INFO
```

### Comparing `gptify-0.3.2/README.md` & `gptify-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `gptify-0.3.2/gptify/gpt_repository_loader.py` & `gptify-0.3.3/gptify/gpt_repository_loader.py`

 * *Files identical despite different names*

### Comparing `gptify-0.3.2/PKG-INFO` & `gptify-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptify
-Version: 0.3.2
+Version: 0.3.3
 Summary: Convert code repos into an LLM prompt-friendly format. Forked from https://github.com/zackees/gptrepo
 Author: Wilder Lopes
 Author-email: wilder@ogre.run
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

