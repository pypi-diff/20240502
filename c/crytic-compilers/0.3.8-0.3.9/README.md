# Comparing `tmp/crytic-compilers-0.3.8.tar.gz` & `tmp/crytic-compilers-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/crytic-compilers-0.3.8.tar", last modified: Wed May  1 22:34:45 2024, max compression
+gzip compressed data, was "dist/crytic-compilers-0.3.9.tar", last modified: Wed May  1 22:37:38 2024, max compression
```

## Comparing `crytic-compilers-0.3.8.tar` & `crytic-compilers-0.3.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 dali      (1000) dali      (1000)        0 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/
-drwxrwxr-x   0 dali      (1000) dali      (1000)        0 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/
--rw-rw-r--   0 dali      (1000) dali      (1000)        1 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/top_level.txt
--rw-rw-r--   0 dali      (1000) dali      (1000)      329 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/PKG-INFO
--rw-rw-r--   0 dali      (1000) dali      (1000)      273 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/SOURCES.txt
--rw-rw-r--   0 dali      (1000) dali      (1000)       46 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/requires.txt
--rw-rw-r--   0 dali      (1000) dali      (1000)        1 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/dependency_links.txt
--rw-rw-r--   0 dali      (1000) dali      (1000)       20 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/crytic_compilers.egg-info/entry_points.txt
--rw-rw-r--   0 dali      (1000) dali      (1000)      329 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/PKG-INFO
--rw-rw-r--   0 dali      (1000) dali      (1000)      855 2024-05-01 22:34:15.000000 crytic-compilers-0.3.8/setup.py
--rw-rw-r--   0 dali      (1000) dali      (1000)       38 2024-05-01 22:34:45.000000 crytic-compilers-0.3.8/setup.cfg
--rw-rw-r--   0 dali      (1000) dali      (1000)      645 2024-05-01 20:37:59.000000 crytic-compilers-0.3.8/pyproject.toml
--rw-rw-r--   0 dali      (1000) dali      (1000)    34523 2024-05-01 20:37:59.000000 crytic-compilers-0.3.8/LICENSE
+drwxrwxr-x   0 dali      (1000) dali      (1000)        0 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/
+drwxrwxr-x   0 dali      (1000) dali      (1000)        0 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/
+-rw-rw-r--   0 dali      (1000) dali      (1000)        1 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/top_level.txt
+-rw-rw-r--   0 dali      (1000) dali      (1000)      329 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/PKG-INFO
+-rw-rw-r--   0 dali      (1000) dali      (1000)      273 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/SOURCES.txt
+-rw-rw-r--   0 dali      (1000) dali      (1000)       46 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/requires.txt
+-rw-rw-r--   0 dali      (1000) dali      (1000)        1 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/dependency_links.txt
+-rw-rw-r--   0 dali      (1000) dali      (1000)       20 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/crytic_compilers.egg-info/entry_points.txt
+-rw-rw-r--   0 dali      (1000) dali      (1000)      329 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/PKG-INFO
+-rw-rw-r--   0 dali      (1000) dali      (1000)      804 2024-05-01 22:37:28.000000 crytic-compilers-0.3.9/setup.py
+-rw-rw-r--   0 dali      (1000) dali      (1000)       38 2024-05-01 22:37:38.000000 crytic-compilers-0.3.9/setup.cfg
+-rw-rw-r--   0 dali      (1000) dali      (1000)      645 2024-05-01 20:37:59.000000 crytic-compilers-0.3.9/pyproject.toml
+-rw-rw-r--   0 dali      (1000) dali      (1000)    34523 2024-05-01 20:37:59.000000 crytic-compilers-0.3.9/LICENSE
```

### Comparing `crytic-compilers-0.3.8/setup.py` & `crytic-compilers-0.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,19 +8,18 @@
 
 install.start()
 setup(
     name="crytic-compilers",
     description="Util to facilitate smart contracts compilation.",
     url="https://github.com/crytic/crytic-compile",
     author="Trail of Boats",
-    version="0.3.8",
+    version="0.3.9",
     packages=find_packages(),
     # Python 3.12.0 on Windows suffers from https://github.com/python/cpython/issues/109590
     # breaking some of our integrations. The issue is fixed in 3.12.1
     python_requires=">=3.8,!=3.13.0",
     install_requires=["pycryptodome>=3.4.6", "cbor2", "solc-select>=v1.0.4"],
     license="AGPL-3.0",
     long_description='test',
     long_description_content_type="text/markdown",
-    package_data={"crytic_compile": ["py.typed"]},
     entry_points={"console_scripts": [""]},
 )
```

### Comparing `crytic-compilers-0.3.8/pyproject.toml` & `crytic-compilers-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crytic-compilers-0.3.8/LICENSE` & `crytic-compilers-0.3.9/LICENSE`

 * *Files identical despite different names*

