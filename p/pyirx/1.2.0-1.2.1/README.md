# Comparing `tmp/pyirx-1.2.0.tar.gz` & `tmp/pyirx-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyirx-1.2.0.tar", max compression
+gzip compressed data, was "pyirx-1.2.1.tar", max compression
```

## Comparing `pyirx-1.2.0.tar` & `pyirx-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1498 2024-04-21 22:03:17.092317 pyirx-1.2.0/LICENSE
--rw-r--r--   0        0        0      518 2024-04-21 22:03:17.092317 pyirx-1.2.0/docs/index.md
--rw-r--r--   0        0        0     2126 2024-04-21 22:04:29.871634 pyirx-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      149 2024-04-21 22:04:29.871634 pyirx-1.2.0/src/irx/__init__.py
--rw-r--r--   0        0        0       32 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/__init__.py
--rw-r--r--   0        0        0     4793 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/base.py
--rw-r--r--   0        0        0    27549 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/llvmliteir.py
--rw-r--r--   0        0        0      739 2024-04-21 22:03:17.092317 pyirx-1.2.0/src/irx/builders/symbol_table.py
--rw-r--r--   0        0        0        0 2024-04-21 22:03:17.096317 pyirx-1.2.0/src/irx/py.typed
--rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 pyirx-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2024-05-02 02:04:29.947567 pyirx-1.2.1/LICENSE
+-rw-r--r--   0        0        0      518 2024-05-02 02:04:29.947567 pyirx-1.2.1/docs/index.md
+-rw-r--r--   0        0        0     2268 2024-05-02 02:05:48.991809 pyirx-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      149 2024-05-02 02:05:48.987809 pyirx-1.2.1/src/irx/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-02 02:04:29.955567 pyirx-1.2.1/src/irx/builders/__init__.py
+-rw-r--r--   0        0        0     4793 2024-05-02 02:04:29.955567 pyirx-1.2.1/src/irx/builders/base.py
+-rw-r--r--   0        0        0    27546 2024-05-02 02:04:29.955567 pyirx-1.2.1/src/irx/builders/llvmliteir.py
+-rw-r--r--   0        0        0      739 2024-05-02 02:04:29.955567 pyirx-1.2.1/src/irx/builders/symbol_table.py
+-rw-r--r--   0        0        0        0 2024-05-02 02:04:29.955567 pyirx-1.2.1/src/irx/py.typed
+-rw-r--r--   0        0        0     1238 1970-01-01 00:00:00.000000 pyirx-1.2.1/PKG-INFO
```

### Comparing `pyirx-1.2.0/LICENSE` & `pyirx-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyirx-1.2.0/docs/index.md` & `pyirx-1.2.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pyirx-1.2.0/pyproject.toml` & `pyirx-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyirx"
-version = "1.2.0"  # semantic-release
+version = "1.2.1"  # semantic-release
 description = "IRx"
 readme = "docs/index.md"
 authors = ["Ivan Ogasawara <ivan.ogasawara@gmail.com>"]
 license = "BSD 3 Clause"
 exclude = [
   ".git/*",
   ".env*",
@@ -13,15 +13,15 @@
   {include = "irx", from="src"},
 ]
 include = ["src/irx/py.typed"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4"
 atpublic = ">=4.0"
-astx = "0.11.*"
+astx = "0.12.2"
 typing-extensions = { version = "^4", python = "<3.9" }
 llvmlite = ">=0.41.1"
 plum-dispatch = ">=2.2.2"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.3.2"
 pytest-cov = ">=4.1.0"
@@ -36,19 +36,22 @@
 ipykernel = ">=6.0.0"
 mkdocs = ">=1.4.3"
 mkdocs-exclude = ">=1.0.2"
 mkdocs-jupyter = ">=0.24.7"
 mkdocs-literate-nav = ">=0.6.0"
 mkdocs-macros-plugin = ">=0.7.0,<1"
 mkdocs-material = ">=9.1.15"
-mkdocstrings = ">=0.21.2"
-mkdocstrings-python = ">=1.1.2"
-makim = "1.14.0"
+mkdocstrings = {version=">=0.24.3", extras=["python"]}
+makim = "1.15.1"
 pdbpp = ">=0.10.3"
 jupyterlab = ">=4.0.7"
+# 'PosixPath' object has no attribute 'endswith'
+virtualenv = "<=20.25.1"
+mkdocs-gen-files = ">=0.5.0"
+nbmake = ">=1.5.3"
 
 [tool.pytest.ini_options]
 testpaths = [
     "tests",
 ]
 
 [tool.bandit]
@@ -105,7 +108,8 @@
 check_untyped_defs = true
 strict = true
 ignore_missing_imports = true
 warn_unused_ignores = true
 warn_redundant_casts = true
 warn_unused_configs = true
 show_error_codes = true
+exclude = ["scripts/"]
```

### Comparing `pyirx-1.2.0/src/irx/builders/base.py` & `pyirx-1.2.1/src/irx/builders/base.py`

 * *Files identical despite different names*

### Comparing `pyirx-1.2.0/src/irx/builders/llvmliteir.py` & `pyirx-1.2.1/src/irx/builders/llvmliteir.py`

 * *Files 0% similar despite different names*

```diff
@@ -654,24 +654,24 @@
 
         self.visit(expr.body)
         self.result_stack.append(fn)
 
     @dispatch  # type: ignore[no-redef]
     def visit(self, expr: astx.FunctionPrototype) -> None:
         """Translate ASTx Function Prototype to LLVM-IR."""
-        args_type = [self._llvm.INT32_TYPE] * len(expr.args)
+        args_type = [self._llvm.INT32_TYPE] * len(expr.args.nodes)
         # note: it should be dynamic
         return_type = self._llvm.get_data_type("int32")
         fn_type = ir.FunctionType(return_type, args_type, False)
 
         fn = ir.Function(self._llvm.module, fn_type, expr.name)
 
         # Set names for all arguments.
         for idx, arg in enumerate(fn.args):
-            fn.args[idx].name = expr.args[idx].name
+            arg.name = expr.args[idx].name
 
         self.result_stack.append(fn)
 
     @dispatch  # type: ignore[no-redef]
     def visit(self, expr: astx.FunctionReturn) -> None:
         """Translate ASTx FunctionReturn to LLVM-IR."""
         self.visit(expr.value)
```

### Comparing `pyirx-1.2.0/src/irx/builders/symbol_table.py` & `pyirx-1.2.1/src/irx/builders/symbol_table.py`

 * *Files identical despite different names*

### Comparing `pyirx-1.2.0/PKG-INFO` & `pyirx-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pyirx
-Version: 1.2.0
+Version: 1.2.1
 Summary: IRx
 License: BSD 3 Clause
 Author: Ivan Ogasawara
 Author-email: ivan.ogasawara@gmail.com
 Requires-Python: >=3.8.1,<4
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: astx (==0.11.*)
+Requires-Dist: astx (==0.12.2)
 Requires-Dist: atpublic (>=4.0)
 Requires-Dist: llvmlite (>=0.41.1)
 Requires-Dist: plum-dispatch (>=2.2.2)
 Requires-Dist: typing-extensions (>=4,<5) ; python_version < "3.9"
 Description-Content-Type: text/markdown
 
 # IRx
```

