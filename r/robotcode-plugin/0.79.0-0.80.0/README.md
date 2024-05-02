# Comparing `tmp/robotcode_plugin-0.79.0.tar.gz` & `tmp/robotcode_plugin-0.80.0.tar.gz`

## Comparing `robotcode_plugin-0.79.0.tar` & `robotcode_plugin-0.80.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/__init__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/__version__.py
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/manager.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/py.typed
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/specs.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/click_helper/aliases.py
--rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/click_helper/options.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/src/robotcode/plugin/click_helper/types.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/LICENSE.txt
--rw-r--r--   0        0        0      712 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/README.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/pyproject.toml
--rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 robotcode_plugin-0.79.0/PKG-INFO
+-rw-r--r--   0        0        0     8693 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/__init__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/__version__.py
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/manager.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/py.typed
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/specs.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/click_helper/aliases.py
+-rw-r--r--   0        0        0    11430 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/click_helper/options.py
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/src/robotcode/plugin/click_helper/types.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/LICENSE.txt
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/README.md
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/pyproject.toml
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 robotcode_plugin-0.80.0/PKG-INFO
```

### Comparing `robotcode_plugin-0.79.0/src/robotcode/plugin/__init__.py` & `robotcode_plugin-0.80.0/src/robotcode/plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/src/robotcode/plugin/manager.py` & `robotcode_plugin-0.80.0/src/robotcode/plugin/manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/src/robotcode/plugin/specs.py` & `robotcode_plugin-0.80.0/src/robotcode/plugin/specs.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/src/robotcode/plugin/click_helper/aliases.py` & `robotcode_plugin-0.80.0/src/robotcode/plugin/click_helper/aliases.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/src/robotcode/plugin/click_helper/options.py` & `robotcode_plugin-0.80.0/src/robotcode/plugin/click_helper/options.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/src/robotcode/plugin/click_helper/types.py` & `robotcode_plugin-0.80.0/src/robotcode/plugin/click_helper/types.py`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/.gitignore` & `robotcode_plugin-0.80.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/LICENSE.txt` & `robotcode_plugin-0.80.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_plugin-0.79.0/README.md` & `robotcode_plugin-0.80.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # robotcode-plugin
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-plugin.svg)](https://pypi.org/project/robotcode-plugin)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-plugin.svg)](https://pypi.org/project/robotcode-plugin)
-[![License](https://img.shields.io/github/license/d-biehl/robotcode?style=flat&logo=apache)](https://github.com/d-biehl/robotcode/blob/master/LICENSE.txt)
+[![License](https://img.shields.io/github/license/robotcodedev/robotcode?style=flat&logo=apache)](https://github.com/robotcodedev/robotcode/blob/master/LICENSE.txt)
 
 -----
 
 ## Introduction
 
 Some classes for [RobotCode](https://robotcode.io) plugin management
```

### Comparing `robotcode_plugin-0.79.0/pyproject.toml` & `robotcode_plugin-0.80.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -26,18 +26,18 @@
   "Framework :: Robot Framework :: Tool",
 ]
 dependencies = ["click>=8.0.0", "pluggy>=1.0.0", "tomli_w>=1.0.0"]
 dynamic = ["version"]
 
 [project.urls]
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
 path = "src/robotcode/plugin/__version__.py"
 
 [tool.hatch.build]
 dev-mode-dirs = ["src"]
```

