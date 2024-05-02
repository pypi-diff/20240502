# Comparing `tmp/caustic.parser-2.2.6.post1.tar.gz` & `tmp/caustic.parser-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "caustic.parser-2.2.6.post1.tar", last modified: Sun Apr 28 22:32:53 2024, max compression
+gzip compressed data, was "caustic.parser-3.0.0.tar", last modified: Thu May  2 18:56:01 2024, max compression
```

## Comparing `caustic.parser-2.2.6.post1.tar` & `caustic.parser-3.0.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/
--rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-2.2.6.post1/LICENSE
--rw-r--r--   0 shae      (1000) shae      (1000)     1890 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      985 2024-04-24 20:59:46.000000 caustic.parser-2.2.6.post1/README.md
--rw-r--r--   0 shae      (1000) shae      (1000)     1013 2024-04-28 22:32:30.000000 caustic.parser-2.2.6.post1/pyproject.toml
--rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/setup.cfg
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.089672 caustic.parser-2.2.6.post1/src/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.089672 caustic.parser-2.2.6.post1/src/caustic/
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/src/caustic/parser/
--rw-r--r--   0 shae      (1000) shae      (1000)     2157 2024-04-24 21:00:34.000000 caustic.parser-2.2.6.post1/src/caustic/parser/__init__.py
--rw-r--r--   0 shae      (1000) shae      (1000)     5643 2024-04-25 22:54:55.000000 caustic.parser-2.2.6.post1/src/caustic/parser/cli.py
--rw-r--r--   0 shae      (1000) shae      (1000)     3688 2024-04-25 22:16:48.000000 caustic.parser-2.2.6.post1/src/caustic/parser/error.py
-drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-04-28 22:32:53.093005 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/
--rw-r--r--   0 shae      (1000) shae      (1000)     1890 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/PKG-INFO
--rw-r--r--   0 shae      (1000) shae      (1000)      371 2024-04-28 22:32:53.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/SOURCES.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/dependency_links.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/entry_points.txt
--rw-r--r--   0 shae      (1000) shae      (1000)       22 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/requires.txt
--rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-04-28 22:32:52.000000 caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/top_level.txt
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-02 18:56:01.339516 caustic.parser-3.0.0/
+-rw-r--r--   0 shae      (1000) shae      (1000)    11337 2024-04-08 15:09:28.000000 caustic.parser-3.0.0/LICENSE
+-rw-r--r--   0 shae      (1000) shae      (1000)     2381 2024-05-02 18:56:01.339516 caustic.parser-3.0.0/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)     1419 2024-05-02 18:52:22.000000 caustic.parser-3.0.0/README.md
+-rw-r--r--   0 shae      (1000) shae      (1000)     1033 2024-05-02 18:54:22.000000 caustic.parser-3.0.0/pyproject.toml
+-rw-r--r--   0 shae      (1000) shae      (1000)       38 2024-05-02 18:56:01.339516 caustic.parser-3.0.0/setup.cfg
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-02 18:56:01.326183 caustic.parser-3.0.0/src/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-02 18:56:01.326183 caustic.parser-3.0.0/src/caustic/
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-02 18:56:01.336183 caustic.parser-3.0.0/src/caustic/parser/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2228 2024-05-02 18:37:28.000000 caustic.parser-3.0.0/src/caustic/parser/__init__.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     1738 2024-05-01 18:04:36.000000 caustic.parser-3.0.0/src/caustic/parser/actions.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     6392 2024-05-02 18:35:27.000000 caustic.parser-3.0.0/src/caustic/parser/cli.py
+-rw-r--r--   0 shae      (1000) shae      (1000)     3688 2024-04-25 22:16:48.000000 caustic.parser-3.0.0/src/caustic/parser/error.py
+drwxr-xr-x   0 shae      (1000) shae      (1000)        0 2024-05-02 18:56:01.336183 caustic.parser-3.0.0/src/caustic.parser.egg-info/
+-rw-r--r--   0 shae      (1000) shae      (1000)     2381 2024-05-02 18:56:01.000000 caustic.parser-3.0.0/src/caustic.parser.egg-info/PKG-INFO
+-rw-r--r--   0 shae      (1000) shae      (1000)      401 2024-05-02 18:56:01.000000 caustic.parser-3.0.0/src/caustic.parser.egg-info/SOURCES.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        1 2024-05-02 18:56:01.000000 caustic.parser-3.0.0/src/caustic.parser.egg-info/dependency_links.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       47 2024-05-02 18:56:01.000000 caustic.parser-3.0.0/src/caustic.parser.egg-info/entry_points.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)       41 2024-05-02 18:56:01.000000 caustic.parser-3.0.0/src/caustic.parser.egg-info/requires.txt
+-rw-r--r--   0 shae      (1000) shae      (1000)        8 2024-05-02 18:56:01.000000 caustic.parser-3.0.0/src/caustic.parser.egg-info/top_level.txt
```

### Comparing `caustic.parser-2.2.6.post1/LICENSE` & `caustic.parser-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6.post1/PKG-INFO` & `caustic.parser-3.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.6.post1
+Version: 3.0.0
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: parglare
+Provides-Extra: cst
+Requires-Dist: caustic.cst; extra == "cst"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 Caustic's Parser -- uses grammar specification to compile Caustic source code
 into a [CST (Caustic AST)](https://codeberg.org/Caustic/CausticAST)
 
 Uses [ParGlare](https://github.com/igordejanovic/parglare) for parsing,
@@ -31,28 +33,36 @@
 
 
 # CLI usage
 
 See `cap --help`
 
 
-# Example module usage
+# Module usage
 
 ```python3
 import sys
 import parglare
+from pprint import pprint
 from pathlib import Path
 
-from caustic.parser import CausticParser
-from caustic.parser.error import format_exc
+from caustic import parser
 
-# CausticParser.from_file() loads the grammar using ParGlare,
-# then invokes CausticParser.from_grammar(), which creates a ParGlare
-# parser instance and uses that to finally create the parser
-p = CausticParser.from_file(Path('<your-grammar-file>'))
+grammar = parglare.Grammar.from_file(parser.builtin_grammar('canonical/canonical.pg'))
+#                                           ^ builtin_grammar fetches the builtin grammar path from caustic.grammar,
+#                                             optionally adding a subdirectory and checking if it exists
+
+
+parser_ = parglare.GLRParser(grammar, lexical_disambiguation=True,
+                             actions=parser.actions.action.all)
+#                                           ^ the actions module supplies some generally useful actions,
+#                                             as well as actions specifically for creating CST nodes
 
 try:
-    print(p.parse(input()))
+    forest = parser_.parse(input())
 except parglare.ParseError as e:
-    # custom error formatting (optional)
-    print(format_exc(e), file=sys.stderr)
+    # custom error formatting
+    print(parser.errors.format_exc(e), file=sys.stderr)
+
+cst = parser_.call_actions(forest.get_first_tree())
+pprint(cst)
 ```
```

### Comparing `caustic.parser-2.2.6.post1/README.md` & `caustic.parser-3.0.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -7,28 +7,36 @@
 
 
 # CLI usage
 
 See `cap --help`
 
 
-# Example module usage
+# Module usage
 
 ```python3
 import sys
 import parglare
+from pprint import pprint
 from pathlib import Path
 
-from caustic.parser import CausticParser
-from caustic.parser.error import format_exc
+from caustic import parser
 
-# CausticParser.from_file() loads the grammar using ParGlare,
-# then invokes CausticParser.from_grammar(), which creates a ParGlare
-# parser instance and uses that to finally create the parser
-p = CausticParser.from_file(Path('<your-grammar-file>'))
+grammar = parglare.Grammar.from_file(parser.builtin_grammar('canonical/canonical.pg'))
+#                                           ^ builtin_grammar fetches the builtin grammar path from caustic.grammar,
+#                                             optionally adding a subdirectory and checking if it exists
+
+
+parser_ = parglare.GLRParser(grammar, lexical_disambiguation=True,
+                             actions=parser.actions.action.all)
+#                                           ^ the actions module supplies some generally useful actions,
+#                                             as well as actions specifically for creating CST nodes
 
 try:
-    print(p.parse(input()))
+    forest = parser_.parse(input())
 except parglare.ParseError as e:
-    # custom error formatting (optional)
-    print(format_exc(e), file=sys.stderr)
+    # custom error formatting
+    print(parser.errors.format_exc(e), file=sys.stderr)
+
+cst = parser_.call_actions(forest.get_first_tree())
+pprint(cst)
 ```
```

### Comparing `caustic.parser-2.2.6.post1/pyproject.toml` & `caustic.parser-3.0.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "caustic.parser"
-version = "2.2.6-1"
+version = "3.0.0"
 dependencies = ['parglare']
 requires-python = ">=3.9"
 authors = [{name="Shae.c32"}]
 maintainers = []
 description = "Caustic's parsing framework"
 readme = "README.md"
 keywords = ['caustic', 'language', 'parser', 'syntax', 'grammar']
@@ -21,15 +21,16 @@
 ]
 
 [project.urls]
 Homepage = "https://codeberg.org/Caustic/CausticParser"
 Issues = "https://codeberg.org/Caustic/CausticParser/issues"
 
 [project.optional-dependencies]
+cst = ["caustic.cst"]
 cli = ["click"]
 
 [project.scripts]
-cap = "caustic.parser.cli:cli"
+cap = "caustic.parser.cli:cap"
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
```

### Comparing `caustic.parser-2.2.6.post1/src/caustic/parser/error.py` & `caustic.parser-3.0.0/src/caustic/parser/error.py`

 * *Files identical despite different names*

### Comparing `caustic.parser-2.2.6.post1/src/caustic.parser.egg-info/PKG-INFO` & `caustic.parser-3.0.0/src/caustic.parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: caustic.parser
-Version: 2.2.6.post1
+Version: 3.0.0
 Summary: Caustic's parsing framework
 Author: Shae.c32
 Project-URL: Homepage, https://codeberg.org/Caustic/CausticParser
 Project-URL: Issues, https://codeberg.org/Caustic/CausticParser/issues
 Keywords: caustic,language,parser,syntax,grammar
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -15,14 +15,16 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Compilers
 Classifier: Topic :: Software Development :: Interpreters
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: parglare
+Provides-Extra: cst
+Requires-Dist: caustic.cst; extra == "cst"
 Provides-Extra: cli
 Requires-Dist: click; extra == "cli"
 
 Caustic's Parser -- uses grammar specification to compile Caustic source code
 into a [CST (Caustic AST)](https://codeberg.org/Caustic/CausticAST)
 
 Uses [ParGlare](https://github.com/igordejanovic/parglare) for parsing,
@@ -31,28 +33,36 @@
 
 
 # CLI usage
 
 See `cap --help`
 
 
-# Example module usage
+# Module usage
 
 ```python3
 import sys
 import parglare
+from pprint import pprint
 from pathlib import Path
 
-from caustic.parser import CausticParser
-from caustic.parser.error import format_exc
+from caustic import parser
 
-# CausticParser.from_file() loads the grammar using ParGlare,
-# then invokes CausticParser.from_grammar(), which creates a ParGlare
-# parser instance and uses that to finally create the parser
-p = CausticParser.from_file(Path('<your-grammar-file>'))
+grammar = parglare.Grammar.from_file(parser.builtin_grammar('canonical/canonical.pg'))
+#                                           ^ builtin_grammar fetches the builtin grammar path from caustic.grammar,
+#                                             optionally adding a subdirectory and checking if it exists
+
+
+parser_ = parglare.GLRParser(grammar, lexical_disambiguation=True,
+                             actions=parser.actions.action.all)
+#                                           ^ the actions module supplies some generally useful actions,
+#                                             as well as actions specifically for creating CST nodes
 
 try:
-    print(p.parse(input()))
+    forest = parser_.parse(input())
 except parglare.ParseError as e:
-    # custom error formatting (optional)
-    print(format_exc(e), file=sys.stderr)
+    # custom error formatting
+    print(parser.errors.format_exc(e), file=sys.stderr)
+
+cst = parser_.call_actions(forest.get_first_tree())
+pprint(cst)
 ```
```

