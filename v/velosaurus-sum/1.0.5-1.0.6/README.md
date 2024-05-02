# Comparing `tmp/velosaurus_sum-1.0.5.tar.gz` & `tmp/velosaurus_sum-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "velosaurus_sum-1.0.5.tar", last modified: Wed May  1 16:23:44 2024, max compression
+gzip compressed data, was "velosaurus_sum-1.0.6.tar", last modified: Wed May  1 16:59:00 2024, max compression
```

## Comparing `velosaurus_sum-1.0.5.tar` & `velosaurus_sum-1.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:44.968478 velosaurus_sum-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 16:23:44.964478 velosaurus_sum-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-01 16:23:39.000000 velosaurus_sum-1.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-01 16:23:39.000000 velosaurus_sum-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:23:44.968478 velosaurus_sum-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-01 16:23:39.000000 velosaurus_sum-1.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:44.964478 velosaurus_sum-1.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:44.964478 velosaurus_sum-1.0.5/src/velosaurus_sum/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-01 16:23:39.000000 velosaurus_sum-1.0.5/src/velosaurus_sum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-01 16:23:39.000000 velosaurus_sum-1.0.5/src/velosaurus_sum/calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:23:44.964478 velosaurus_sum-1.0.5/src/velosaurus_sum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-05-01 16:23:44.000000 velosaurus_sum-1.0.5/src/velosaurus_sum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 16:23:44.000000 velosaurus_sum-1.0.5/src/velosaurus_sum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:23:44.000000 velosaurus_sum-1.0.5/src/velosaurus_sum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 16:23:44.000000 velosaurus_sum-1.0.5/src/velosaurus_sum.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:00.501283 velosaurus_sum-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-01 16:59:00.501283 velosaurus_sum-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-01 16:58:53.000000 velosaurus_sum-1.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1741 2024-05-01 16:58:53.000000 velosaurus_sum-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 16:59:00.501283 velosaurus_sum-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-05-01 16:58:53.000000 velosaurus_sum-1.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:00.497282 velosaurus_sum-1.0.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:00.501283 velosaurus_sum-1.0.6/src/velosaurus_sum/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-01 16:58:53.000000 velosaurus_sum-1.0.6/src/velosaurus_sum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 16:58:53.000000 velosaurus_sum-1.0.6/src/velosaurus_sum/calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 16:59:00.501283 velosaurus_sum-1.0.6/src/velosaurus_sum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-01 16:59:00.000000 velosaurus_sum-1.0.6/src/velosaurus_sum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 16:59:00.000000 velosaurus_sum-1.0.6/src/velosaurus_sum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 16:59:00.000000 velosaurus_sum-1.0.6/src/velosaurus_sum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-01 16:59:00.000000 velosaurus_sum-1.0.6/src/velosaurus_sum.egg-info/top_level.txt
```

### Comparing `velosaurus_sum-1.0.5/pyproject.toml` & `velosaurus_sum-1.0.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.mypy]
 ignore_missing_imports = true
 exclude = [
     "build/",
 ]
+disallow_untyped_defs = true
 
 
 [tool.ruff]
 # Exclude a variety of commonly ignored directories.
 exclude = [
     ".bzr",
     ".direnv",
@@ -72,9 +73,9 @@
 # Like Black, automatically detect the appropriate line ending.
 line-ending = "auto"
 
 
 
 # --------------------------------------------------------------------------------------------------
 # Specific ruff isort rules
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 force-single-line = true
```

### Comparing `velosaurus_sum-1.0.5/setup.py` & `velosaurus_sum-1.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from setuptools import find_packages
 from setuptools import setup
 
+with open("PYPI_README.md") as f:
+    long_description = f.read()
+
 setup(
     name="velosaurus_sum",
-    version="1.0.5",
+    version="1.0.6",
     description="Just a dummy project for some pipeline and package deployment testing",
-    long_description="Just a dummy project for some pipeline and package deployment testing",
+    long_description=long_description,
+    long_description_content_type="text/markdown",
     author="Oliver Zott",
     author_email="zott_oliver@web.de",
     url="https://github.com/OliverZott/python-devops-example",
     # packages=find_packages(),
     packages=find_packages(where="src"),
     package_dir={"": "src"},
     install_requires=[
```

