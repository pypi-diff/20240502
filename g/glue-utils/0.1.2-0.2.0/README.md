# Comparing `tmp/glue_utils-0.1.2.tar.gz` & `tmp/glue_utils-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glue_utils-0.1.2.tar", max compression
+gzip compressed data, was "glue_utils-0.2.0.tar", max compression
```

## Comparing `glue_utils-0.1.2.tar` & `glue_utils-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,9 @@
--rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.1.2/LICENSE
--rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.1.2/README.md
--rw-r--r--   0        0        0     3129 2024-03-11 04:22:30.247987 glue_utils-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      110 2024-03-11 04:22:30.248520 glue_utils-0.1.2/src/glue_utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-03-11 03:53:51.532849 glue_utils-0.1.2/src/glue_utils/context.py
--rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 glue_utils-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-03-06 15:16:48.910706 glue_utils-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1138 2024-03-07 09:36:58.526889 glue_utils-0.2.0/README.md
+-rw-r--r--   0        0        0     3312 2024-05-02 06:54:14.343575 glue_utils-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0       96 2024-05-02 06:55:10.579843 glue_utils-0.2.0/src/glue_utils/__init__.py
+-rw-r--r--   0        0        0       68 2024-05-02 06:53:45.157325 glue_utils-0.2.0/src/glue_utils/glueetl/__init__.py
+-rw-r--r--   0        0        0     2135 2024-05-02 06:53:45.157808 glue_utils-0.2.0/src/glue_utils/glueetl/job.py
+-rw-r--r--   0        0        0      982 2024-05-02 06:53:45.158192 glue_utils-0.2.0/src/glue_utils/options.py
+-rw-r--r--   0        0        0        0 2024-05-02 06:53:45.158255 glue_utils-0.2.0/src/glue_utils/py.typed
+-rw-r--r--   0        0        0     2201 1970-01-01 00:00:00.000000 glue_utils-0.2.0/PKG-INFO
```

### Comparing `glue_utils-0.1.2/LICENSE` & `glue_utils-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `glue_utils-0.1.2/README.md` & `glue_utils-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `glue_utils-0.1.2/pyproject.toml` & `glue_utils-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [tool.poetry]
 name = "glue-utils"
-version = "0.1.2"
-package-mode = true
+version = "0.2.0"
+# Uncomment this when dependabot has finally been updated to it is 
+# supported by dependabot.
+# package-mode = true
 description = "Reusable utilities for working with Glue PySpark jobs"
 authors = ["Noel Llevares <dashmug@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/dashmug/glue-utils"
 repository = "https://github.com/dashmug/glue-utils/issues"
 documentation = "https://github.com/dashmug/glue-utils/wiki"
@@ -28,19 +30,18 @@
 ]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 
 [tool.poetry.group.dev.dependencies]
 pytest-randomly = "^3.15.0"
-pytest-cov = "^4.1.0"
-pip-audit = "^2.7.2"
-mypy = "^1.9.0"
-ruff = "^0.3.2"
-pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+ruff = "^0.4.2"
+mypy = "^1.10.0"
+pytest = "^8.2.0"
 
 [tool.poetry.group.local.dependencies]
 # The "local" dependency group refers to dependencies that already 
 # exist in AWS Glue's runtime. We don't need to install these in the
 # container. We only need them for local (non-container) development to 
 # aid the IDE in providing code completion and type checking.
 # 
@@ -64,24 +65,28 @@
 select = ["ALL"]
 ignore = [
     "D203",
     "D213",
     # Conflicts with ruff format
     "COM812",
     "ISC001",
+    # missing-type-self
+    "ANN101",
+    # missing-type-cls
+    "ANN102",
 ]
 exclude = ["snapshots", ".venv"]
 # # Allow unused variables when underscore-prefixed.
 dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
 
 [tool.ruff.lint.mccabe]
 max-complexity = 5
 
 [tool.ruff.lint.per-file-ignores]
-"test/**" = ["S101", "ANN", "PT", "PD", "D"]
+"test/**" = ["S101", "ANN", "ARG001", "ARG002", "PLR2004", "PT", "PD", "D"]
 
 [tool.mypy]
 files = "**/*.py"
 python_version = "3.10"
 show_error_codes = true
 pretty = true
 strict = true
```

### Comparing `glue_utils-0.1.2/PKG-INFO` & `glue_utils-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glue-utils
-Version: 0.1.2
+Version: 0.2.0
 Summary: Reusable utilities for working with Glue PySpark jobs
 Home-page: https://github.com/dashmug/glue-utils
 License: MIT
 Keywords: aws,glue,pyspark,spark,etl,data,data-engineering
 Author: Noel Llevares
 Author-email: dashmug@gmail.com
 Requires-Python: >=3.10,<4.0
```

