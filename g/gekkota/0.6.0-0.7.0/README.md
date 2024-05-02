# Comparing `tmp/gekkota-0.6.0.tar.gz` & `tmp/gekkota-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gekkota-0.6.0.tar", max compression
+gzip compressed data, was "gekkota-0.7.0.tar", max compression
```

## Comparing `gekkota-0.6.0.tar` & `gekkota-0.7.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1073 2024-01-29 11:49:10.645192 gekkota-0.6.0/LICENSE
--rw-r--r--   0        0        0    24280 2024-01-29 11:49:10.645192 gekkota-0.6.0/README.md
--rw-r--r--   0        0        0     3323 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/__init__.py
--rw-r--r--   0        0        0     2456 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/annotations.py
--rw-r--r--   0        0        0     2277 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/args.py
--rw-r--r--   0        0        0     1926 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/assignment.py
--rw-r--r--   0        0        0     2588 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/block.py
--rw-r--r--   0        0        0     1036 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/classes.py
--rw-r--r--   0        0        0     1220 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/constants.py
--rw-r--r--   0        0        0     3161 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/control_flow.py
--rw-r--r--   0        0        0     1018 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/core.py
--rw-r--r--   0        0        0     1858 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/exceptions.py
--rw-r--r--   0        0        0     5765 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/expression.py
--rw-r--r--   0        0        0     2140 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/functions.py
--rw-r--r--   0        0        0     1781 2024-01-29 11:49:10.645192 gekkota-0.6.0/gekkota/generator_expr.py
--rw-r--r--   0        0        0     1907 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/imports.py
--rw-r--r--   0        0        0     1337 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/operator_expr.py
--rw-r--r--   0        0        0     6397 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/pattern_matching.py
--rw-r--r--   0        0        0        0 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/py.typed
--rw-r--r--   0        0        0     4508 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/sequences.py
--rw-r--r--   0        0        0     1260 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/small_stmt.py
--rw-r--r--   0        0        0     1530 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/to_expression.py
--rw-r--r--   0        0        0     2156 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/utils.py
--rw-r--r--   0        0        0     5189 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/values.py
--rw-r--r--   0        0        0     1921 2024-01-29 11:49:10.649192 gekkota-0.6.0/gekkota/wscomp.py
--rw-r--r--   0        0        0     1002 2024-01-29 11:49:10.649192 gekkota-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    25091 1970-01-01 00:00:00.000000 gekkota-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-02 08:57:54.418855 gekkota-0.7.0/LICENSE
+-rw-r--r--   0        0        0    24280 2024-05-02 08:57:54.422855 gekkota-0.7.0/README.md
+-rw-r--r--   0        0        0     3365 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/__init__.py
+-rw-r--r--   0        0        0     2456 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/annotations.py
+-rw-r--r--   0        0        0     2277 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/args.py
+-rw-r--r--   0        0        0     1926 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/assignment.py
+-rw-r--r--   0        0        0     2588 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/block.py
+-rw-r--r--   0        0        0     1036 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/classes.py
+-rw-r--r--   0        0        0     1398 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/comments.py
+-rw-r--r--   0        0        0     1220 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/constants.py
+-rw-r--r--   0        0        0     3161 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/control_flow.py
+-rw-r--r--   0        0        0     1018 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/core.py
+-rw-r--r--   0        0        0     1858 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/exceptions.py
+-rw-r--r--   0        0        0     5765 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/expression.py
+-rw-r--r--   0        0        0     2140 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/functions.py
+-rw-r--r--   0        0        0     1781 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/generator_expr.py
+-rw-r--r--   0        0        0     1907 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/imports.py
+-rw-r--r--   0        0        0     1337 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/operator_expr.py
+-rw-r--r--   0        0        0     6397 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/pattern_matching.py
+-rw-r--r--   0        0        0        0 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/py.typed
+-rw-r--r--   0        0        0     4508 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/sequences.py
+-rw-r--r--   0        0        0     1260 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/small_stmt.py
+-rw-r--r--   0        0        0     1530 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/to_expression.py
+-rw-r--r--   0        0        0     2186 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/utils.py
+-rw-r--r--   0        0        0     5189 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/values.py
+-rw-r--r--   0        0        0     1921 2024-05-02 08:57:54.422855 gekkota-0.7.0/gekkota/wscomp.py
+-rw-r--r--   0        0        0     1002 2024-05-02 08:57:54.422855 gekkota-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    25091 1970-01-01 00:00:00.000000 gekkota-0.7.0/PKG-INFO
```

### Comparing `gekkota-0.6.0/LICENSE` & `gekkota-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/README.md` & `gekkota-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/__init__.py` & `gekkota-0.7.0/gekkota/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from .constants import StrGen as StrGen, Config as Config
 
+from .comments import Comment as Comment
+
 from .core import Renderable as Renderable, Statement as Statement
 
 from .expression import Expression as Expression, Parens as Parens
 
 from .args import (
     CallArg as CallArg,
     FuncArg as FuncArg,
```

### Comparing `gekkota-0.6.0/gekkota/annotations.py` & `gekkota-0.7.0/gekkota/annotations.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/args.py` & `gekkota-0.7.0/gekkota/args.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/assignment.py` & `gekkota-0.7.0/gekkota/assignment.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/block.py` & `gekkota-0.7.0/gekkota/block.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/classes.py` & `gekkota-0.7.0/gekkota/classes.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/constants.py` & `gekkota-0.7.0/gekkota/constants.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/control_flow.py` & `gekkota-0.7.0/gekkota/control_flow.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/core.py` & `gekkota-0.7.0/gekkota/core.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/exceptions.py` & `gekkota-0.7.0/gekkota/exceptions.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/expression.py` & `gekkota-0.7.0/gekkota/expression.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/functions.py` & `gekkota-0.7.0/gekkota/functions.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/generator_expr.py` & `gekkota-0.7.0/gekkota/generator_expr.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/imports.py` & `gekkota-0.7.0/gekkota/imports.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/operator_expr.py` & `gekkota-0.7.0/gekkota/operator_expr.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/pattern_matching.py` & `gekkota-0.7.0/gekkota/pattern_matching.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/sequences.py` & `gekkota-0.7.0/gekkota/sequences.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/small_stmt.py` & `gekkota-0.7.0/gekkota/small_stmt.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/to_expression.py` & `gekkota-0.7.0/gekkota/to_expression.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/utils.py` & `gekkota-0.7.0/gekkota/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Sequence
+from typing import Sequence, Iterable
 
 
 class Utils:
     @staticmethod
     def add_tab(generator: StrGen, config: Config) -> StrGen:
         tab_size: int = config.get("tab_size", 4)
         tab_char: str = config.get("tab_char", " ")
@@ -14,36 +14,46 @@
         for part in generator:
             yield part
             if part == "\n":
                 yield tab
 
     @staticmethod
     def separated(
-        separator: Sequence[str], renderables: Sequence[Renderable], config: Config
+        separator: Iterable[str], renderables: Iterable[Renderable], config: Config
     ) -> StrGen:
-        if not len(renderables):
-            yield ""
-            return
-        yield from renderables[0].render(config)
-        for renderable in renderables[1:]:
-            yield from separator
+        counter = 0
+
+        for renderable in renderables:
+            if counter:
+                yield from separator
+
             yield from renderable.render(config)
 
-    @staticmethod
-    def separated_str(separator: Sequence[str], strings: Sequence[str], config: Config):
-        if not len(strings):
+            counter += 1
+
+        if not counter:
             yield ""
-            return
-        yield strings[0]
-        for renderable in strings[1:]:
-            yield from separator
+
+    @staticmethod
+    def separated_str(separator: Iterable[str], strings: Iterable[str], config: Config):
+        counter = 0
+
+        for renderable in strings:
+            if counter:
+                yield from separator
+
             yield renderable
 
+            counter += 1
+
+        if not counter:
+            yield ""
+
     @staticmethod
-    def comma_separated(renderables: Sequence[Renderable], config: Config) -> StrGen:
+    def comma_separated(renderables: Iterable[Renderable], config: Config) -> StrGen:
         yield from Utils.separated(", ", renderables, config)
 
     @staticmethod
     def make_compact(generator: StrGen, config: Config) -> StrGen:
         is_tab = False
         last_token_isalpha = False
         for token in generator:
```

### Comparing `gekkota-0.6.0/gekkota/values.py` & `gekkota-0.7.0/gekkota/values.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/gekkota/wscomp.py` & `gekkota-0.7.0/gekkota/wscomp.py`

 * *Files identical despite different names*

### Comparing `gekkota-0.6.0/pyproject.toml` & `gekkota-0.7.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gekkota"
-version = "0.6.0"
+version = "0.7.0"
 description = "Python code-generation for Python"
 authors = ["Dmitry Gritsenko <k01419q45@ya.ru>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/courage-tci/gekkota"
 homepage = "https://github.com/courage-tci/gekkota"
 keywords = ["codegen"]
```

### Comparing `gekkota-0.6.0/PKG-INFO` & `gekkota-0.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gekkota
-Version: 0.6.0
+Version: 0.7.0
 Summary: Python code-generation for Python
 Home-page: https://github.com/courage-tci/gekkota
 License: MIT
 Keywords: codegen
 Author: Dmitry Gritsenko
 Author-email: k01419q45@ya.ru
 Requires-Python: >=3.8,<4.0
```

