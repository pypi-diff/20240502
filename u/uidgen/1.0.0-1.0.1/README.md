# Comparing `tmp/uidgen-1.0.0.tar.gz` & `tmp/uidgen-1.0.1.tar.gz`

## Comparing `uidgen-1.0.0.tar` & `uidgen-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 uidgen-1.0.0/uidgen/__init__.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 uidgen-1.0.0/uidgen/__main__.py
--rw-r--r--   0        0        0    41037 2020-02-02 00:00:00.000000 uidgen-1.0.0/uidgen/data.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 uidgen-1.0.0/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 uidgen-1.0.0/LICENSE
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 uidgen-1.0.0/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 uidgen-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 uidgen-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 uidgen-1.0.1/uidgen/__init__.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 uidgen-1.0.1/uidgen/__main__.py
+-rw-r--r--   0        0        0    41037 2020-02-02 00:00:00.000000 uidgen-1.0.1/uidgen/data.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 uidgen-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 uidgen-1.0.1/LICENSE
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 uidgen-1.0.1/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 uidgen-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     3831 2020-02-02 00:00:00.000000 uidgen-1.0.1/PKG-INFO
```

### Comparing `uidgen-1.0.0/uidgen/data.py` & `uidgen-1.0.1/uidgen/data.py`

 * *Files identical despite different names*

### Comparing `uidgen-1.0.0/LICENSE` & `uidgen-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uidgen-1.0.0/pyproject.toml` & `uidgen-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "uidgen"
-version = "1.0.0"
+version = "1.0.1"
 authors = [{ name = "Jay Mody", email = "jaykmody@gmail.com" }]
 description = "An adjective-noun-number identifier generator."
 license = { file = "LICENSE" }
 readme = "README.md"
 keywords = ["names", "random", "rng"]
 classifiers = [
     "Natural Language :: English",
```

