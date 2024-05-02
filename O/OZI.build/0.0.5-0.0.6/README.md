# Comparing `tmp/OZI.build-0.0.5.tar.gz` & `tmp/OZI.build-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OZI.build-0.0.5.tar", last modified: Wed May  1 16:25:37 2024, max compression
+gzip compressed data, was "OZI.build-0.0.6.tar", last modified: Thu May  2 00:17:27 2024, max compression
```

## Comparing `OZI.build-0.0.5.tar` & `OZI.build-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 16:25:37.755326 OZI.build-0.0.5/
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 16:24:59.000000 OZI.build-0.0.5/.gitignore
--rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 16:24:59.000000 OZI.build-0.0.5/.gitlab-ci.yml
--rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 16:24:59.000000 OZI.build-0.0.5/COPYING
--rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 16:24:59.000000 OZI.build-0.0.5/README.rst
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 16:24:59.000000 OZI.build-0.0.5/__init__.py
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 16:25:37.751326 OZI.build-0.0.5/doc/
--rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/generate_doc.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/index.md
--rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/pyproject-gen.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/pyproject.md
--rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/pyproject.md.in
--rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 16:24:59.000000 OZI.build-0.0.5/doc/sitemap.txt
--rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 16:24:59.000000 OZI.build-0.0.5/meson.build
-drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-01 16:25:37.755326 OZI.build-0.0.5/ozi_build/
--rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/__init__.py
--rw-rw-r--   0 ross      (1000) ross      (1000)    14741 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/buildapi.py
--rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/meson.build
--rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/pep425tags.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 16:24:59.000000 OZI.build-0.0.5/ozi_build/schema.py
--rw-rw-r--   0 ross      (1000) ross      (1000)     1070 2024-05-01 16:24:59.000000 OZI.build-0.0.5/pyproject.toml
--rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 16:24:59.000000 OZI.build-0.0.5/release
--rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-01 16:25:37.763326 OZI.build-0.0.5/PKG-INFO
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-02 00:17:27.001459 OZI.build-0.0.6/
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 23:15:58.000000 OZI.build-0.0.6/.gitignore
+-rw-rw-r--   0 ross      (1000) ross      (1000)      422 2024-05-01 23:15:58.000000 OZI.build-0.0.6/.gitlab-ci.yml
+-rw-rw-r--   0 ross      (1000) ross      (1000)    11359 2024-05-01 23:15:58.000000 OZI.build-0.0.6/COPYING
+-rw-rw-r--   0 ross      (1000) ross      (1000)      482 2024-05-01 23:15:58.000000 OZI.build-0.0.6/README.rst
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 23:15:58.000000 OZI.build-0.0.6/__init__.py
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-02 00:17:27.001459 OZI.build-0.0.6/doc/
+-rwxrwxr-x   0 ross      (1000) ross      (1000)      651 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/generate_doc.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1105 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/index.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)      623 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3388 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/pyproject-gen.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4171 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/pyproject.md
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1339 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/pyproject.md.in
+-rw-rw-r--   0 ross      (1000) ross      (1000)       29 2024-05-01 23:15:58.000000 OZI.build-0.0.6/doc/sitemap.txt
+-rw-rw-r--   0 ross      (1000) ross      (1000)      164 2024-05-01 23:15:58.000000 OZI.build-0.0.6/meson.build
+drwxrwxr-x   0 ross      (1000) ross      (1000)        0 2024-05-02 00:17:27.001459 OZI.build-0.0.6/ozi_build/
+-rw-rw-r--   0 ross      (1000) ross      (1000)        0 2024-05-01 23:15:58.000000 OZI.build-0.0.6/ozi_build/__init__.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)    14755 2024-05-01 23:15:58.000000 OZI.build-0.0.6/ozi_build/buildapi.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)      230 2024-05-01 23:15:58.000000 OZI.build-0.0.6/ozi_build/meson.build
+-rw-rw-r--   0 ross      (1000) ross      (1000)     4297 2024-05-01 23:15:58.000000 OZI.build-0.0.6/ozi_build/pep425tags.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     3509 2024-05-01 23:15:58.000000 OZI.build-0.0.6/ozi_build/schema.py
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1070 2024-05-01 23:15:58.000000 OZI.build-0.0.6/pyproject.toml
+-rwxrwxr-x   0 ross      (1000) ross      (1000)       73 2024-05-01 23:15:58.000000 OZI.build-0.0.6/release
+-rw-rw-r--   0 ross      (1000) ross      (1000)     1353 2024-05-02 00:17:27.009460 OZI.build-0.0.6/PKG-INFO
```

### Comparing `OZI.build-0.0.5/COPYING` & `OZI.build-0.0.6/COPYING`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/doc/generate_doc.py` & `OZI.build-0.0.6/doc/generate_doc.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/doc/index.md` & `OZI.build-0.0.6/doc/index.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/doc/meson.build` & `OZI.build-0.0.6/doc/meson.build`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/doc/pyproject-gen.md` & `OZI.build-0.0.6/doc/pyproject-gen.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/doc/pyproject.md` & `OZI.build-0.0.6/doc/pyproject.md`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/doc/pyproject.md.in` & `OZI.build-0.0.6/doc/pyproject.md.in`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/ozi_build/buildapi.py` & `OZI.build-0.0.6/ozi_build/buildapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -442,15 +442,15 @@
                 '--prefix',
                 installdir,
                 config_settings=config_settings,
                 builddir=builddir,
             )
 
             config = Config(builddir)
-            meson('dist', '-C', builddir)
+            meson('dist', '--no-tests', '-C', builddir)
 
             tf_dir = '{}-{}'.format(config['module'], config['version'])
             mesondistfilename = '%s.tar.xz' % tf_dir
             mesondisttar = tarfile.open(
                 Path(builddir) / 'meson-dist' / mesondistfilename
             )
             for entry in mesondisttar:
```

### Comparing `OZI.build-0.0.5/ozi_build/pep425tags.py` & `OZI.build-0.0.6/ozi_build/pep425tags.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/ozi_build/schema.py` & `OZI.build-0.0.6/ozi_build/schema.py`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/pyproject.toml` & `OZI.build-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `OZI.build-0.0.5/PKG-INFO` & `OZI.build-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OZI.build
-Version: 0.0.5
+Version: 0.0.6
 Summary: Create pep517 compliant packages from the meson build system, OZI-maintained fork.
 Home-page: https://github.com/OZI-Project/OZI.build
 Author: Thibault Saunier
 Author-email: tsaunier@gnome.org
 Maintainer: Eden Rose Duff MSc
 Maintainer-email: help@oziproject.dev
 Requires-Dist: wheel>0.33
```

