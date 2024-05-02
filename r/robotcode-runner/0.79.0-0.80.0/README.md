# Comparing `tmp/robotcode_runner-0.79.0.tar.gz` & `tmp/robotcode_runner-0.80.0.tar.gz`

## Comparing `robotcode_runner-0.79.0.tar` & `robotcode_runner-0.80.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/__version__.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/hooks.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/py.typed
--rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/__init__.py
--rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/libdoc.py
--rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/rebot.py
--rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/robot.py
--rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/testdoc.py
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/discover/__init__.py
--rw-r--r--   0        0        0    29976 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/src/robotcode/runner/cli/discover/discover.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/README.md
--rw-r--r--   0        0        0     1835 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/pyproject.toml
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 robotcode_runner-0.79.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/__version__.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/hooks.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/py.typed
+-rw-r--r--   0        0        0      200 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/__init__.py
+-rw-r--r--   0        0        0     3358 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/libdoc.py
+-rw-r--r--   0        0        0     3436 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/rebot.py
+-rw-r--r--   0        0        0     6193 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/robot.py
+-rw-r--r--   0        0        0     3370 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/testdoc.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/discover/__init__.py
+-rw-r--r--   0        0        0    29976 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/src/robotcode/runner/cli/discover/discover.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/LICENSE.txt
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/README.md
+-rw-r--r--   0        0        0     1855 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/pyproject.toml
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 robotcode_runner-0.80.0/PKG-INFO
```

### Comparing `robotcode_runner-0.79.0/src/robotcode/runner/cli/libdoc.py` & `robotcode_runner-0.80.0/src/robotcode/runner/cli/libdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/src/robotcode/runner/cli/rebot.py` & `robotcode_runner-0.80.0/src/robotcode/runner/cli/rebot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/src/robotcode/runner/cli/robot.py` & `robotcode_runner-0.80.0/src/robotcode/runner/cli/robot.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/src/robotcode/runner/cli/testdoc.py` & `robotcode_runner-0.80.0/src/robotcode/runner/cli/testdoc.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/src/robotcode/runner/cli/discover/discover.py` & `robotcode_runner-0.80.0/src/robotcode/runner/cli/discover/discover.py`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/.gitignore` & `robotcode_runner-0.80.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/LICENSE.txt` & `robotcode_runner-0.80.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_runner-0.79.0/README.md` & `robotcode_runner-0.80.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
-[![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
+[![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
 
 -----
 
 ## Introduction
 
 Some classes for [RobotCode](https://robotcode.io) plugin management
```

### Comparing `robotcode_runner-0.79.0/PKG-INFO` & `robotcode_runner-0.80.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.3
 Name: robotcode-runner
-Version: 0.79.0
+Version: 0.80.0
 Summary: RobotCode runner plugin for Robot Framework
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
-Requires-Dist: robotcode-modifiers==0.79.0
-Requires-Dist: robotcode-plugin==0.79.0
-Requires-Dist: robotcode-robot==0.79.0
-Requires-Dist: robotcode==0.79.0
+Requires-Dist: robotcode-modifiers==0.80.0
+Requires-Dist: robotcode-plugin==0.80.0
+Requires-Dist: robotcode-robot==0.80.0
+Requires-Dist: robotcode==0.80.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-runner
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-runner.svg)](https://pypi.org/project/robotcode-runner)
-[![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
+[![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
 
 -----
 
 ## Introduction
 
 Some classes for [RobotCode](https://robotcode.io) plugin management
```

