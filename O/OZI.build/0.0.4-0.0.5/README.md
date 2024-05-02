# Comparing `tmp/OZI.build-0.0.4.tar.gz` & `tmp/OZI.build-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI.build-0.0.4.tar", last modified: Wed May  1 14:51:38 2024, max compression
+gzip compressed data, was "OZI.build-0.0.5.tar", last modified: Wed May  1 16:25:37 2024, max compression
```

## Comparing `OZI.build-0.0.4.tar` & `OZI.build-0.0.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 14:51:38.911227 OZI.build-0.0.4/
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 14:49:25.000000 OZI.build-0.0.4/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 14:49:25.000000 OZI.build-0.0.4/.gitlab-ci.yml
--rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 14:49:25.000000 OZI.build-0.0.4/COPYING
--rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 14:49:25.000000 OZI.build-0.0.4/README.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 14:49:25.000000 OZI.build-0.0.4/__init__.py
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 14:51:38.907226 OZI.build-0.0.4/doc/
--rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/generate_doc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/index.md
--rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/pyproject-gen.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/pyproject.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/pyproject.md.in
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 14:49:25.000000 OZI.build-0.0.4/doc/sitemap.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 14:49:25.000000 OZI.build-0.0.4/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 14:51:38.911227 OZI.build-0.0.4/ozi_build/
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)    14745 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/buildapi.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/pep425tags.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 14:49:25.000000 OZI.build-0.0.4/ozi_build/schema.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1132 2024-05-01 14:49:25.000000 OZI.build-0.0.4/pyproject.toml
--rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 14:49:25.000000 OZI.build-0.0.4/release
--rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 14:51:38.915227 OZI.build-0.0.4/PKG-INFO
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 16:25:37.755326 OZI.build-0.0.5/
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 16:24:59.000000 OZI.build-0.0.5/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 16:24:59.000000 OZI.build-0.0.5/.gitlab-ci.yml
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 16:24:59.000000 OZI.build-0.0.5/COPYING
+-rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 16:24:59.000000 OZI.build-0.0.5/README.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 16:24:59.000000 OZI.build-0.0.5/__init__.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 16:25:37.751326 OZI.build-0.0.5/doc/
+-rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/generate_doc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/index.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/pyproject-gen.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/pyproject.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/pyproject.md.in
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/sitemap.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 16:24:59.000000 OZI.build-0.0.5/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 16:25:37.755326 OZI.build-0.0.5/ozi_build/
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)    14741 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/buildapi.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/pep425tags.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/schema.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1070 2024-05-01 16:24:59.000000 OZI.build-0.0.5/pyproject.toml
+-rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 16:24:59.000000 OZI.build-0.0.5/release
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 16:25:37.763326 OZI.build-0.0.5/PKG-INFO
```

### Comparing `OZI.build-0.0.4/COPYING` & `OZI.build-0.0.5/COPYING`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/doc/generate_doc.py` & `OZI.build-0.0.5/doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/doc/index.md` & `OZI.build-0.0.5/doc/index.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/doc/meson.build` & `OZI.build-0.0.5/doc/meson.build`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/doc/pyproject-gen.md` & `OZI.build-0.0.5/doc/pyproject-gen.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/doc/pyproject.md` & `OZI.build-0.0.5/doc/pyproject.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/doc/pyproject.md.in` & `OZI.build-0.0.5/doc/pyproject.md.in`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/ozi_build/buildapi.py` & `OZI.build-0.0.5/ozi_build/buildapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -374,15 +374,15 @@
         if not option_build:
             log.warning(
                 "meson-python-option-name not specified in the "
                 + "[tool.ozi-build.metadata] section, assuming `python3`"
             )
         else:
             for opt in config.options:
-                if opt['name'] == 'python_version':
+                if opt['name'] == option_build:
                     python = opt['value']
                     break
         if not is_pure:
             abi = get_abi(python)
         else:
             abi = '{}-none'.format(
                 config.get('requires-python', get_abi(python))
```

### Comparing `OZI.build-0.0.4/ozi_build/pep425tags.py` & `OZI.build-0.0.5/ozi_build/pep425tags.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/ozi_build/schema.py` & `OZI.build-0.0.5/ozi_build/schema.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.4/pyproject.toml` & `OZI.build-0.0.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     'tomli>=2.0.0;python_version<"3.11"',
     "setuptools>=64",
 ]
 backend-path = [".", "ozi_build"]
 build-backend = "ozi_build.buildapi"
 
 [tool.ozi-build.metadata]
-meson-python-option-name=true
+meson-python-option-name="python_version"
 author="Thibault Saunier"
 author-email="tsaunier@gnome.org"
 maintainer="Eden Rose Duff MSc"
 maintainer-email="help@oziproject.dev"
 summary="Create pep517 compliant packages from the meson build system, OZI-maintained fork."
 home-page="https://github.com/OZI-Project/OZI.build"
 description-file="README.rst"
@@ -24,12 +24,8 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 requires-python="py3"
 requires = ["wheel>0.33", "meson[ninja]>1.1.0", 'tomli>=2.0.0;python_version<"3.11"', "setuptools"]
 project-urls= [
     "Source, https://github.com/OZI-Project/OZI.build",
     "Documentation, https://thiblahute.gitlab.io/mesonpep517/",
-]
-
-[tool.setuptools.packages.find]
-where = ["ozi_build"]
-namespaces = false
+]
```

### Comparing `OZI.build-0.0.4/PKG-INFO` & `OZI.build-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OZI.build
-Version: 0.0.4
+Version: 0.0.5
 Summary: Create pep517 compliant packages from the meson build system, OZI-maintained fork.
 Home-page: https://github.com/OZI-Project/OZI.build
 Author: Thibault Saunier
 Author-email: tsaunier@gnome.org
 Maintainer: Eden Rose Duff MSc
 Maintainer-email: help@oziproject.dev
 Requires-Dist: wheel>0.33
```

