# Comparing `tmp/slipcover-1.0.8.tar.gz` & `tmp/slipcover-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slipcover-1.0.8.tar", last modified: Sat Apr 13 00:19:34 2024, max compression
+gzip compressed data, was "slipcover-1.0.9.tar", last modified: Wed Apr 24 20:33:07 2024, max compression
```

## Comparing `slipcover-1.0.8.tar` & `slipcover-1.0.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-13 00:19:15.000000 slipcover-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-13 00:19:15.000000 slipcover-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-13 00:19:34.279439 slipcover-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-13 00:19:15.000000 slipcover-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 00:19:34.283439 slipcover-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-13 00:19:15.000000 slipcover-1.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.275439 slipcover-1.0.8/src/
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/probe.cxx
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/pyptr.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/src/slipcover/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6472 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    21990 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/bytecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/fuzz.py
--rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/importer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25595 2024-04-13 00:19:15.000000 slipcover-1.0.8/src/slipcover/slipcover.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/src/slipcover.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-13 00:19:34.000000 slipcover-1.0.8/src/slipcover.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 00:19:34.279439 slipcover-1.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    15650 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_branch.py
--rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_bytecode.py
--rw-r--r--   0 runner    (1001) docker     (127)    28457 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_importer.py
--rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_instrumentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/test_isolate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme-class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme-inner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme-partial.py
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-13 00:19:15.000000 slipcover-1.0.8/tests/testme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:33:07.227299 slipcover-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-24 20:32:50.000000 slipcover-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 20:32:50.000000 slipcover-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-24 20:33:07.227299 slipcover-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8234 2024-04-24 20:32:50.000000 slipcover-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 20:33:07.227299 slipcover-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-24 20:32:50.000000 slipcover-1.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:33:07.223299 slipcover-1.0.9/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/probe.cxx
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/pyptr.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:33:07.223299 slipcover-1.0.9/src/slipcover/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6473 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21990 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      437 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/fuzz.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9302 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2171 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25769 2024-04-24 20:32:50.000000 slipcover-1.0.9/src/slipcover/slipcover.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:33:07.227299 slipcover-1.0.9/src/slipcover.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9403 2024-04-24 20:33:07.000000 slipcover-1.0.9/src/slipcover.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 20:33:07.000000 slipcover-1.0.9/src/slipcover.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 20:33:07.000000 slipcover-1.0.9/src/slipcover.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-24 20:33:07.000000 slipcover-1.0.9/src/slipcover.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 20:33:07.000000 slipcover-1.0.9/src/slipcover.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-24 20:33:07.000000 slipcover-1.0.9/src/slipcover.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 20:33:07.227299 slipcover-1.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    15650 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/test_branch.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22245 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/test_bytecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29942 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9528 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/test_importer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17508 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/test_instrumentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/test_isolate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/testme-class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/testme-inner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/testme-partial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-24 20:32:50.000000 slipcover-1.0.9/tests/testme.py
```

### Comparing `slipcover-1.0.8/LICENSE` & `slipcover-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/PKG-INFO` & `slipcover-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.8
+Version: 1.0.9
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.8/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.9/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -58,16 +58,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.9/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.9/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -87,15 +87,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.8/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.9/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.8/README.md` & `slipcover-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/setup.py` & `slipcover-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/probe.cxx` & `slipcover-1.0.9/src/probe.cxx`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/pyptr.h` & `slipcover-1.0.9/src/pyptr.h`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/slipcover/__main__.py` & `slipcover-1.0.9/src/slipcover/__main__.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/slipcover/branch.py` & `slipcover-1.0.9/src/slipcover/branch.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
             else:
                 for node in ast.walk(mark):
                     node.lineno = from_line
 
             return [mark]
 
         def visit_FunctionDef(self, node: Union[ast.AsyncFunctionDef, ast.FunctionDef]) -> ast.AST:
-            # Mark BRANCH_NAME global, so that our assignment are easier to find (only STORE_NAME/STORE_GLOBAL,
+            # Mark BRANCH_NAME global, so that our assignments are easier to find (only STORE_NAME/STORE_GLOBAL,
             # but not STORE_FAST, etc.)
             has_docstring = ast.get_docstring(node, clean=False) is not None
             node.body.insert(1 if has_docstring else 0, ast.Global([BRANCH_NAME]))
             super().generic_visit(node)
             return node
 
         def visit_AsyncFunctionDef(self, node: ast.AsyncFunctionDef) -> ast.AST:
```

### Comparing `slipcover-1.0.8/src/slipcover/bytecode.py` & `slipcover-1.0.9/src/slipcover/bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/slipcover/importer.py` & `slipcover-1.0.9/src/slipcover/importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/slipcover/isolate.py` & `slipcover-1.0.9/src/slipcover/isolate.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/src/slipcover/slipcover.py` & `slipcover-1.0.9/src/slipcover/slipcover.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,35 @@
         raise RuntimeError("You probably have the wrong package; " + \
                            "SlipCover for Python <3.12 requires version-specific builds")
     from . import bytecode as bc
 
 from pathlib import Path
 from . import branch as br
 
-VERSION = "1.0.8"
+VERSION = "1.0.9"
 
 # FIXME provide __all__
 
 # Counter.total() is new in 3.10
 if sys.version_info[0:2] < (3,10):
     def counter_total(self: Counter) -> int:
         return sum([self[n] for n in self])
     setattr(Counter, 'total', counter_total)
 
 
 # Python 3.13 returns 'None' lines;
-# Python 3.11+ generates a line just for RESUME;
+# Python 3.11+ generates a line just for RESUME or RETURN_GENERATOR, POP_TOP, RESUME;
 # Python 3.11 generates a 0th line
 if sys.version_info[0:2] >= (3,11):
     _op_RESUME = dis.opmap["RESUME"]
+    _op_RETURN_GENERATOR = dis.opmap["RETURN_GENERATOR"]
 
     def findlinestarts(co: types.CodeType):
         for off, line in dis.findlinestarts(co):
-            if line and co.co_code[off] != _op_RESUME:
+            if line and co.co_code[off] not in (_op_RESUME, _op_RETURN_GENERATOR):
                 yield off, line
 
 else:
     findlinestarts = dis.findlinestarts
 
 
 class SlipcoverError(Exception):
@@ -379,31 +380,29 @@
             # handle functions-within-functions
             for i, c in enumerate(co.co_consts):
                 if isinstance(c, types.CodeType):
                     ed.set_const(i, self.instrument(c, co))
 
             probe_signal_index = ed.add_const(probe.signal)
 
-            off_list = list(dis.findlinestarts(co))
+            off_list = list(findlinestarts(co))
             if self.branch:
                 off_list.extend(list(ed.find_const_assignments(br.BRANCH_NAME)))
                 # sort line probes (2-tuples) before branch probes (3-tuples) because
                 # line probes don't overwrite bytecode like branch probes do, so if there
                 # are two being inserted at the same offset, the accumulated offset 'delta' applies
                 off_list.sort(key = lambda x: (x[0], len(x)))
 
             insert_labels = []
             probes = []
 
             delta = 0
             for off_item in off_list:
                 if len(off_item) == 2: # from findlinestarts
                     offset, lineno = off_item
-                    if lineno == 0 or co.co_code[offset] == bc.op_RESUME:
-                        continue
 
                     # Can't insert between an EXTENDED_ARG and the final opcode
                     if (offset >= 2 and co.co_code[offset-2] == bc.op_EXTENDED_ARG):
                         while (offset < len(co.co_code) and co.co_code[offset-2] == bc.op_EXTENDED_ARG):
                             offset += 2 # TODO will we overtake the next offset from findlinestarts?
 
                     insert_labels.append(lineno)
@@ -427,14 +426,18 @@
                     delta += ed.insert_function_call(begin_off+delta, probe_signal_index, (branch_index,),
                                                      repl_length = end_off-begin_off)
 
             ed.add_const('__slipcover__')  # mark instrumented
             new_code = ed.finish()
 
             if self.disassemble:
+                print()
+                print(f'---- {co.co_name} before ----')
+                dis.dis(co)
+                print(f'---- {co.co_name} after ----')
                 dis.dis(new_code)
 
             if self.immediate:
                 for tr, off in zip(probes, ed.get_inserts()):
                     probe.set_immediate(tr, new_code.co_code, off)
             else:
                 index = list(zip(ed.get_inserts(), insert_labels))
```

### Comparing `slipcover-1.0.8/src/slipcover.egg-info/PKG-INFO` & `slipcover-1.0.9/src/slipcover.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slipcover
-Version: 1.0.8
+Version: 1.0.9
 Summary: Near Zero-Overhead Python Code Coverage
 Home-page: https://github.com/plasma-umass/slipcover
 Author: Juan Altmayer Pizzorno, Emery Berger
 Author-email: juan@altmayer.com, emery@cs.umass.edu
 License: Apache License 2.0
 Keywords: coverage testing
 Classifier: Programming Language :: Python :: 3.8
@@ -24,15 +24,15 @@
 
 ![slipcover](https://github.com/plasma-umass/slipcover/raw/main/docs/slipcover-logo.png)
 
 # SlipCover: Near Zero-Overhead Python Code Coverage
 by [Juan Altmayer Pizzorno](https://jaltmayerpizzorno.github.io) and [Emery Berger](https://emeryberger.com)
 at UMass Amherst's [PLASMA lab](https://plasma-umass.org/).
 
-[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.8/LICENSE)
+[![license](https://img.shields.io/github/license/plasma-umass/slipcover?color=blue)](https://github.com/plasma-umass/slipcover/blob/v1.0.9/LICENSE)
 [![pypi](https://img.shields.io/pypi/v/slipcover?color=blue)](https://pypi.org/project/slipcover/)
 [![Downloads](https://static.pepy.tech/badge/slipcover)](https://pepy.tech/project/slipcover)
 ![pyversions](https://img.shields.io/pypi/pyversions/slipcover)
 ![tests](https://github.com/jaltmayerpizzorno/slipcover/workflows/tests/badge.svg)
 
 ## About Slipcover
 SlipCover is a fast [code coverage](https://en.wikipedia.org/wiki/Code_coverage) tool.
@@ -58,16 +58,16 @@
 Care is taken throughout SlipCover to keep things as efficient as possible.
 On Python 3.12, rather than rewrite bytecode, SlipCover uses the new
 [`sys.monitoring`](https://docs.python.org/3.12/library/sys.monitoring.html) API
 to collect coverage information.
 
 
 ### Performance
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
-<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.8/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.9/benchmarks/cpython.png?raw=True" align="right" width="65%"/>
+<img src="https://github.com/plasma-umass/slipcover/blob/v1.0.9/benchmarks/pypy.png?raw=True" align="right" width="65%"/>
 
 [//]: # (CPython-range)
 The first image on the right shows SlipCover's [speedup](https://en.wikipedia.org/wiki/Speedup),
 ranging from 1.1x to 3.4x, in relation to [Coverage.py](https://github.com/nedbat/coveragepy), running on
 [CPython 3.10.5](https://github.com/python/cpython).
 
 The first two benchmarks are the test suites for [scikit-learn](https://scikit-learn.org/stable/)
@@ -87,15 +87,15 @@
 Since it is so high for some of the benchmarks, we plot it on a logarithmic scale (see the second image on the right).
 
 In a proof-of-concept integration with a property-based testing package,
 SlipCover sped up coverage-based testing 22x.
 
 ### Accuracy
 We verified SlipCover's accuracy against [Coverage.py](https://github.com/nedbat/coveragepy)
-and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.8/tools/oracle.py) of our own that collects coverage using Python tracing.
+and against a [simple script](https://github.com/plasma-umass/slipcover/blob/v1.0.9/tools/oracle.py) of our own that collects coverage using Python tracing.
 We found SlipCover's results to be accurate, in fact, in certain cases [more accurate](https://github.com/nedbat/coveragepy/issues/1358).
 
 ## Getting started
 SlipCover is available from [PyPI](https://pypi.org/project/slipcover).
 You can install it like any other Python module with
 ```console
 pip3 install slipcover
```

### Comparing `slipcover-1.0.8/src/slipcover.egg-info/SOURCES.txt` & `slipcover-1.0.9/src/slipcover.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/test_branch.py` & `slipcover-1.0.9/tests/test_branch.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/test_bytecode.py` & `slipcover-1.0.9/tests/test_bytecode.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/test_coverage.py` & `slipcover-1.0.9/tests/test_coverage.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,14 +156,77 @@
     assert {simple_current_file()} == cov['files'].keys()
 
     cov = cov['files'][simple_current_file()]
     assert [3, 4, 5, 6] == [l-base_line for l in cov['executed_lines']]
     assert [] == cov['missing_lines']
 
 
+def test_async_inline():
+    sci = sc.Slipcover()
+    result = None
+
+    base_line = current_line()
+    async def foo(n):
+        nonlocal result
+        x = 0
+        for i in range(n):
+            x += (i+1)
+        result = x
+
+    sci.instrument(foo)
+
+    import asyncio
+    asyncio.run(foo(3))
+
+    assert 6 == result
+
+    cov = sci.get_coverage()
+    assert {simple_current_file()} == cov['files'].keys()
+
+    cov = cov['files'][simple_current_file()]
+    assert [3, 4, 5, 6] == [l-base_line for l in cov['executed_lines']]
+    assert [] == cov['missing_lines']
+
+
+@pytest.mark.parametrize("do_branch", [True, False])
+def test_async_file(tmp_path, do_branch):
+    code = tmp_path / "t.py"
+    out = tmp_path / "out.json"
+
+    code.write_text("""\
+import asyncio
+
+async def foo(n):
+    x = 0
+    for i in range(n):
+        x += (i+1)
+    result = x
+
+asyncio.run(foo(3))
+""")
+
+    subprocess.run([sys.executable, '-m', 'slipcover'] + (['--branch'] if do_branch else []) +\
+                   ['--json', '--out', out, code])
+    with out.open("r") as f:
+        cov = json.load(f)
+
+    assert {str(code)} == cov['files'].keys()
+
+    cov = cov['files'][str(code)]
+    assert [1, 3, 4, 5, 6, 7, 9] == cov['executed_lines']
+    assert [] == cov['missing_lines']
+
+    if do_branch:
+        assert [[5,6], [5,7]] == cov['executed_branches']
+        assert [] == cov['missing_branches']
+    else:
+        assert 'executed_branches' not in cov
+        assert 'missing_branches' not in cov
+
+
 def test_branches():
     t = ast_parse("""
         def foo(x):
             if x >= 0:
                 if x > 1:
                     if x > 2:
                         return 2
```

### Comparing `slipcover-1.0.8/tests/test_importer.py` & `slipcover-1.0.9/tests/test_importer.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/test_instrumentation.py` & `slipcover-1.0.9/tests/test_instrumentation.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/test_isolate.py` & `slipcover-1.0.9/tests/test_isolate.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/testme-class.py` & `slipcover-1.0.9/tests/testme-class.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/testme-inner.py` & `slipcover-1.0.9/tests/testme-inner.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/testme-partial.py` & `slipcover-1.0.9/tests/testme-partial.py`

 * *Files identical despite different names*

### Comparing `slipcover-1.0.8/tests/testme.py` & `slipcover-1.0.9/tests/testme.py`

 * *Files identical despite different names*

