# Comparing `tmp/robotcode_debugger-0.79.0.tar.gz` & `tmp/robotcode_debugger-0.80.0.tar.gz`

## Comparing `robotcode_debugger-0.79.0.tar` & `robotcode_debugger-0.80.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/__version__.py
--rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/cli.py
--rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/dap_types.py
--rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/debugger.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/hooks.py
--rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/listeners.py
--rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/protocol.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/py.typed
--rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/run.py
--rw-r--r--   0        0        0    15859 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/__init__.py
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/cli.py
--rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/client.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/run.py
--rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/server.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/LICENSE.txt
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/README.md
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/pyproject.toml
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 robotcode_debugger-0.79.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/__version__.py
+-rw-r--r--   0        0        0     5895 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/cli.py
+-rw-r--r--   0        0        0    25783 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/dap_types.py
+-rw-r--r--   0        0        0    69967 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/debugger.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/hooks.py
+-rw-r--r--   0        0        0    12904 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/listeners.py
+-rw-r--r--   0        0        0    12802 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/protocol.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/py.typed
+-rw-r--r--   0        0        0     8485 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/run.py
+-rw-r--r--   0        0        0    15859 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/__init__.py
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/cli.py
+-rw-r--r--   0        0        0     3654 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/client.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/run.py
+-rw-r--r--   0        0        0    13913 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/server.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/LICENSE.txt
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/README.md
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/pyproject.toml
+-rw-r--r--   0        0        0     2224 2020-02-02 00:00:00.000000 robotcode_debugger-0.80.0/PKG-INFO
```

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/cli.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/dap_types.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/dap_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/debugger.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/debugger.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/listeners.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/listeners.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/protocol.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/run.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/server.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/cli.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/client.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/client.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/run.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/run.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/src/robotcode/debugger/launcher/server.py` & `robotcode_debugger-0.80.0/src/robotcode/debugger/launcher/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/.gitignore` & `robotcode_debugger-0.80.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/LICENSE.txt` & `robotcode_debugger-0.80.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_debugger-0.79.0/README.md` & `robotcode_debugger-0.80.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # robotcode-debugger
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-debugger.svg)](https://pypi.org/project/robotcode-debugger)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-debugger.svg)](https://pypi.org/project/robotcode-debugger)
-[![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
+[![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
 
 -----
 
 ## Introduction
 
 The [RobotCode](https://robotcode.io) Debugger for Robot Framework.
```

### Comparing `robotcode_debugger-0.79.0/pyproject.toml` & `robotcode_debugger-0.80.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -24,31 +24,31 @@
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
 dynamic = ["version"]
 dependencies = [
   "robotframework>=4.1.0",
-  "robotcode-jsonrpc2==0.79.0",
-  "robotcode-runner==0.79.0",
+  "robotcode-jsonrpc2==0.80.0",
+  "robotcode-runner==0.80.0",
 ]
 
 [project.optional-dependencies]
 debugpy = ["debugpy"]
 
 [project.entry-points.robotcode]
 debugger = "robotcode.debugger.hooks"
 
 [project.urls]
 Homepage = "https://robotcode.io"
 Donate = "https://github.com/sponsors/d-biehl"
-Documentation = "https://github.com/d-biehl/robotcode#readme"
-Changelog = "https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md"
-Issues = "https://github.com/d-biehl/robotcode/issues"
-Source = "https://github.com/d-biehl/robotcode"
+Documentation = "https://github.com/robotcodedev/robotcode#readme"
+Changelog = "https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md"
+Issues = "https://github.com/robotcodedev/robotcode/issues"
+Source = "https://github.com/robotcodedev/robotcode"
 
 [tool.hatch.version]
 path = "src/robotcode/debugger/__version__.py"
 
 [tool.hatch.build]
 dev-mode-dirs = ["src"]
```

### Comparing `robotcode_debugger-0.79.0/PKG-INFO` & `robotcode_debugger-0.80.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.3
 Name: robotcode-debugger
-Version: 0.79.0
+Version: 0.80.0
 Summary: RobotCode Debugger for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
-Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
-Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
-Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
-Project-URL: Source, https://github.com/d-biehl/robotcode
+Project-URL: Documentation, https://github.com/robotcodedev/robotcode#readme
+Project-URL: Changelog, https://github.com/robotcodedev/robotcode/blob/main/CHANGELOG.md
+Project-URL: Issues, https://github.com/robotcodedev/robotcode/issues
+Project-URL: Source, https://github.com/robotcodedev/robotcode
 Author-email: Daniel Biehl <dbiehl@live.de>
 License: Apache-2.0
 License-File: LICENSE.txt
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Robot Framework
 Classifier: Framework :: Robot Framework :: Tool
 Classifier: Operating System :: OS Independent
@@ -21,26 +21,26 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.79.0
-Requires-Dist: robotcode-runner==0.79.0
+Requires-Dist: robotcode-jsonrpc2==0.80.0
+Requires-Dist: robotcode-runner==0.80.0
 Requires-Dist: robotframework>=4.1.0
 Provides-Extra: debugpy
 Requires-Dist: debugpy; extra == 'debugpy'
 Description-Content-Type: text/markdown
 
 # robotcode-debugger
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-debugger.svg)](https://pypi.org/project/robotcode-debugger)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-debugger.svg)](https://pypi.org/project/robotcode-debugger)
-[![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
+[![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
 
 -----
 
 ## Introduction
 
 The [RobotCode](https://robotcode.io) Debugger for Robot Framework.
```

