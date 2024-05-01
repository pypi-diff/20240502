# Comparing `tmp/GeoAlchemy2-0.9.3.tar.gz` & `tmp/GeoAlchemy2-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/GeoAlchemy2-0.9.3.tar", last modified: Tue Jul 27 11:11:31 2021, max compression
+gzip compressed data, was "dist/GeoAlchemy2-0.9.4.tar", last modified: Wed Aug 25 16:53:27 2021, max compression
```

## Comparing `GeoAlchemy2-0.9.3.tar` & `GeoAlchemy2-0.9.4.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (116)       29 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/geoalchemy2/
--rw-r--r--   0 runner    (1001) docker     (116)     7494 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/comparator.py
--rw-r--r--   0 runner    (1001) docker     (116)     8710 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     6965 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      518 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     8285 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/elements.py
--rw-r--r--   0 runner    (1001) docker     (116)     3392 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/shape.py
--rw-r--r--   0 runner    (1001) docker     (116)    63113 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    14245 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/types.py
--rw-r--r--   0 runner    (1001) docker     (116)      240 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/geoalchemy2/exc.py
--rw-r--r--   0 runner    (1001) docker     (116)      617 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/RELEASE.rst
--rw-r--r--   0 runner    (1001) docker     (116)      546 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      833 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     5628 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (116)     1604 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      114 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1717 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/TEST.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     4019 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/.github/workflows/test_and_publish.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     2646 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_shape.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/tests/gallery/
--rw-r--r--   0 runner    (1001) docker     (116)     1902 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/test_disable_wrapping.py
--rw-r--r--   0 runner    (1001) docker     (116)     3759 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/test_raster_transform.py
--rw-r--r--   0 runner    (1001) docker     (116)     5153 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/test_type_decorator.py
--rw-r--r--   0 runner    (1001) docker     (116)     2137 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/test_length_at_insert.py
--rw-r--r--   0 runner    (1001) docker     (116)     3111 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/test_summarystatsagg.py
--rw-r--r--   0 runner    (1001) docker     (116)     5353 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/test_decipher_raster.py
--rw-r--r--   0 runner    (1001) docker     (116)       30 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/gallery/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1076 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    16937 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    11114 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_functional_spatialite.py
--rw-r--r--   0 runner    (1001) docker     (116)     5799 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_comparator.py
--rw-r--r--   0 runner    (1001) docker     (116)    12994 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (116)    34581 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (116)     8749 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/tests/test_types.py
--rw-r--r--   0 runner    (1001) docker     (116)       86 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/requirements-doc.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)       12 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1604 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)       16 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       33 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1782 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      714 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)       28 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/MANIFEST.in
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/doc/
--rw-r--r--   0 runner    (1001) docker     (116)     8176 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)    11730 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/core_tutorial.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/doc/_templates/
--rw-r--r--   0 runner    (1001) docker     (116)      119 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_templates/sidebar-about.html
--rw-r--r--   0 runner    (1001) docker     (116)      291 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_templates/sidebar-links.html
--rw-r--r--   0 runner    (1001) docker     (116)      148 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_templates/sidebar-logo.html
--rw-r--r--   0 runner    (1001) docker     (116)     3899 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/shape.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/doc/_static/
--rw-r--r--   0 runner    (1001) docker     (116)    21092 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_static/geoalchemy.png
--rw-r--r--   0 runner    (1001) docker     (116)    17361 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_static/geoalchemy_small.png
--rw-r--r--   0 runner    (1001) docker     (116)    20959 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_static/geoalchemy_small.svg
--rw-r--r--   0 runner    (1001) docker     (116)    17274 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_static/geoalchemy.svg
--rw-r--r--   0 runner    (1001) docker     (116)    13758 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/orm_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (116)      115 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/types.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4521 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/make.bat
--rw-r--r--   0 runner    (1001) docker     (116)      323 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/elements.rst
--rw-r--r--   0 runner    (1001) docker     (116)      112 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/spatial_functions.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6686 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/spatialite_tutorial.rst
--rw-r--r--   0 runner    (1001) docker     (116)     4610 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)      156 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/spatial_operators.rst
--rw-r--r--   0 runner    (1001) docker     (116)     2656 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/migrate.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/doc/_themes/
--rw-r--r--   0 runner    (1001) docker     (116)     1789 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/
--rw-r--r--   0 runner    (1001) docker     (116)      590 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/relations.html
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-07-27 11:11:31.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/static/
--rw-r--r--   0 runner    (1001) docker     (116)     6659 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/static/flasky.css_t
--rw-r--r--   0 runner    (1001) docker     (116)      976 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/static/small_flask.css
--rw-r--r--   0 runner    (1001) docker     (116)      937 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/layout.html
--rw-r--r--   0 runner    (1001) docker     (116)      178 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/flask/theme.conf
--rw-r--r--   0 runner    (1001) docker     (116)     1093 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/doc/_themes/README
--rw-r--r--   0 runner    (1001) docker     (116)     1056 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/COPYING.rst
--rw-r--r--   0 runner    (1001) docker     (116)     1271 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)       59 2021-07-27 11:11:20.000000 GeoAlchemy2-0.9.3/requirements-rtd.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (116)     1604 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     4019 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/.github/workflows/test_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/MANIFEST.in
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/geoalchemy2/
+-rw-r--r--   0 runner    (1001) docker     (116)     8285 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/elements.py
+-rw-r--r--   0 runner    (1001) docker     (116)    63113 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/_functions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8710 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/functions.py
+-rw-r--r--   0 runner    (1001) docker     (116)      240 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/exc.py
+-rw-r--r--   0 runner    (1001) docker     (116)      518 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3392 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/shape.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7375 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7494 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14245 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/geoalchemy2/types.py
+-rw-r--r--   0 runner    (1001) docker     (116)      714 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1604 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1782 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       12 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       26 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1056 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/COPYING.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5708 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/CHANGES.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/doc/
+-rw-r--r--   0 runner    (1001) docker     (116)     2656 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/migrate.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     3899 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4521 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/doc/_templates/
+-rw-r--r--   0 runner    (1001) docker     (116)      119 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_templates/sidebar-about.html
+-rw-r--r--   0 runner    (1001) docker     (116)      148 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_templates/sidebar-logo.html
+-rw-r--r--   0 runner    (1001) docker     (116)      291 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_templates/sidebar-links.html
+-rw-r--r--   0 runner    (1001) docker     (116)    13758 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/orm_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      162 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/shape.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      115 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/types.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     6686 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/spatialite_tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/doc/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)    21092 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_static/geoalchemy.png
+-rw-r--r--   0 runner    (1001) docker     (116)    17361 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_static/geoalchemy_small.png
+-rw-r--r--   0 runner    (1001) docker     (116)    17274 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_static/geoalchemy.svg
+-rw-r--r--   0 runner    (1001) docker     (116)    20959 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_static/geoalchemy_small.svg
+-rw-r--r--   0 runner    (1001) docker     (116)      323 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/elements.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/doc/_themes/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/
+-rw-r--r--   0 runner    (1001) docker     (116)      590 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/relations.html
+-rw-r--r--   0 runner    (1001) docker     (116)      178 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/theme.conf
+-rw-r--r--   0 runner    (1001) docker     (116)      937 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/static/
+-rw-r--r--   0 runner    (1001) docker     (116)     6659 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/static/flasky.css_t
+-rw-r--r--   0 runner    (1001) docker     (116)      976 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/flask/static/small_flask.css
+-rw-r--r--   0 runner    (1001) docker     (116)     1789 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)     1093 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/_themes/README
+-rw-r--r--   0 runner    (1001) docker     (116)      112 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/spatial_functions.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      156 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/spatial_operators.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     4610 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)     8176 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11730 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/doc/core_tutorial.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      114 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      617 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/RELEASE.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      546 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/requirements-rtd.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1717 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/TEST.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1291 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (116)       86 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       29 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/.flake8
+-rw-r--r--   0 runner    (1001) docker     (116)       49 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)    12994 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_elements.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/tests/gallery/
+-rw-r--r--   0 runner    (1001) docker     (116)     3111 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/test_summarystatsagg.py
+-rw-r--r--   0 runner    (1001) docker     (116)       30 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5153 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/test_type_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5353 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/test_decipher_raster.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3759 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/test_raster_transform.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1902 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/test_disable_wrapping.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2137 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/gallery/test_length_at_insert.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11114 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_functional_spatialite.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1076 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2646 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_shape.py
+-rw-r--r--   0 runner    (1001) docker     (116)    16937 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_functions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8749 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_types.py
+-rw-r--r--   0 runner    (1001) docker     (116)    34581 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5799 2021-08-25 16:53:16.000000 GeoAlchemy2-0.9.4/tests/test_comparator.py
+-rw-r--r--   0 runner    (1001) docker     (116)      833 2021-08-25 16:53:27.000000 GeoAlchemy2-0.9.4/setup.cfg
```

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/comparator.py` & `GeoAlchemy2-0.9.4/geoalchemy2/comparator.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/functions.py` & `GeoAlchemy2-0.9.4/geoalchemy2/functions.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/__init__.py` & `GeoAlchemy2-0.9.4/geoalchemy2/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,29 @@
     )
 
 from .exc import ArgumentError
 
 from . import functions  # NOQA
 from . import types  # NOQA
 
+import sqlalchemy
 from sqlalchemy import Table, event
 from sqlalchemy.sql import select, func, expression, text
 
+from packaging import version
+
+_SQLALCHEMY_VERSION_BEFORE_14 = version.parse(sqlalchemy.__version__) < version.parse("1.4")
+
+
+def _format_select_args(*args):
+    if _SQLALCHEMY_VERSION_BEFORE_14:
+        return [args]
+    else:
+        return args
+
 
 def _setup_ddl_event_listeners():
     @event.listens_for(Table, "before_create")
     def before_create(target, connection, **kw):
         dispatch("before-create", target, connection)
 
     @event.listens_for(Table, "after_create")
@@ -65,15 +77,15 @@
                     elif bind.dialect.name == 'postgresql':
                         drop_func = 'DropGeometryColumn'
                     else:
                         raise ArgumentError('dialect {} is not supported'.format(bind.dialect.name))
                     args = [table.schema] if table.schema else []
                     args.extend([table.name, c.name])
 
-                    stmt = select([getattr(func, drop_func)(*args)])
+                    stmt = select(*_format_select_args(getattr(func, drop_func)(*args)))
                     stmt = stmt.execution_options(autocommit=True)
                     bind.execute(stmt)
 
         elif event == 'after-create':
             # Restore original column list including managed Geometry columns
             table.columns = table.info.pop('_saved_columns')
 
@@ -89,23 +101,24 @@
                         c.type.dimension
                     ])
                     if c.type.use_typmod is not None:
                         args.append(c.type.use_typmod)
                     if bind.dialect.name == 'sqlite':
                         args.append(not c.type.nullable)
 
-                    stmt = select([func.AddGeometryColumn(*args)])
+                    stmt = select(*_format_select_args(func.AddGeometryColumn(*args)))
                     stmt = stmt.execution_options(autocommit=True)
                     bind.execute(stmt)
 
                 # Add spatial indices for the Geometry and Geography columns
                 if isinstance(c.type, (Geometry, Geography)) and \
                         c.type.spatial_index is True:
                     if bind.dialect.name == 'sqlite':
-                        stmt = select([func.CreateSpatialIndex(table.name, c.name)])
+                        stmt = select(*_format_select_args(func.CreateSpatialIndex(table.name,
+                                                                                   c.name)))
                         stmt = stmt.execution_options(autocommit=True)
                         bind.execute(stmt)
                     elif bind.dialect.name == 'postgresql':
 
                         index_name = '"idx_{}_{}"'.format(table.name, c.name)
 
                         if c.type.use_N_D_index:
```

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/compat.py` & `GeoAlchemy2-0.9.4/geoalchemy2/compat.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/elements.py` & `GeoAlchemy2-0.9.4/geoalchemy2/elements.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/shape.py` & `GeoAlchemy2-0.9.4/geoalchemy2/shape.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/_functions.py` & `GeoAlchemy2-0.9.4/geoalchemy2/_functions.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/geoalchemy2/types.py` & `GeoAlchemy2-0.9.4/geoalchemy2/types.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/RELEASE.rst` & `GeoAlchemy2-0.9.4/RELEASE.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/.gitignore` & `GeoAlchemy2-0.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/setup.cfg` & `GeoAlchemy2-0.9.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/CHANGES.txt` & `GeoAlchemy2-0.9.4/CHANGES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 GeoAlchemy 2 Changelog
 ======================
 
+0.9.4
+-----
+
+* Fix warnings in preparation for SQLAlchemy v2.0 @robintw (#331)
+
 0.9.3
 -----
 
 * Add support for not nullable column for SQLite @adrien-berchet (#327)
 
 0.9.2
 -----
```

### Comparing `GeoAlchemy2-0.9.3/PKG-INFO` & `GeoAlchemy2-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoAlchemy2
-Version: 0.9.3
+Version: 0.9.4
 Summary: Using SQLAlchemy with Spatial Databases
 Home-page: https://geoalchemy-2.readthedocs.io/en/latest/
 Author: Eric Lemoine
 Author-email: eric.lemoine@gmail.com
 License: MIT
 Keywords: geo gis sqlalchemy orm
 Platform: UNKNOWN
```

### Comparing `GeoAlchemy2-0.9.3/TEST.rst` & `GeoAlchemy2-0.9.4/TEST.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/.github/workflows/test_and_publish.yml` & `GeoAlchemy2-0.9.4/.github/workflows/test_and_publish.yml`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_shape.py` & `GeoAlchemy2-0.9.4/tests/test_shape.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/gallery/test_disable_wrapping.py` & `GeoAlchemy2-0.9.4/tests/gallery/test_disable_wrapping.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/gallery/test_raster_transform.py` & `GeoAlchemy2-0.9.4/tests/gallery/test_raster_transform.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/gallery/test_type_decorator.py` & `GeoAlchemy2-0.9.4/tests/gallery/test_type_decorator.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/gallery/test_length_at_insert.py` & `GeoAlchemy2-0.9.4/tests/gallery/test_length_at_insert.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/gallery/test_summarystatsagg.py` & `GeoAlchemy2-0.9.4/tests/gallery/test_summarystatsagg.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/gallery/test_decipher_raster.py` & `GeoAlchemy2-0.9.4/tests/gallery/test_decipher_raster.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/__init__.py` & `GeoAlchemy2-0.9.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_functions.py` & `GeoAlchemy2-0.9.4/tests/test_functions.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_functional_spatialite.py` & `GeoAlchemy2-0.9.4/tests/test_functional_spatialite.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_comparator.py` & `GeoAlchemy2-0.9.4/tests/test_comparator.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_elements.py` & `GeoAlchemy2-0.9.4/tests/test_elements.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_functional.py` & `GeoAlchemy2-0.9.4/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/tests/test_types.py` & `GeoAlchemy2-0.9.4/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/PKG-INFO` & `GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GeoAlchemy2
-Version: 0.9.3
+Version: 0.9.4
 Summary: Using SQLAlchemy with Spatial Databases
 Home-page: https://geoalchemy-2.readthedocs.io/en/latest/
 Author: Eric Lemoine
 Author-email: eric.lemoine@gmail.com
 License: MIT
 Keywords: geo gis sqlalchemy orm
 Platform: UNKNOWN
```

### Comparing `GeoAlchemy2-0.9.3/GeoAlchemy2.egg-info/SOURCES.txt` & `GeoAlchemy2-0.9.4/GeoAlchemy2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/README.rst` & `GeoAlchemy2-0.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/conf.py` & `GeoAlchemy2-0.9.4/doc/conf.py`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/core_tutorial.rst` & `GeoAlchemy2-0.9.4/doc/core_tutorial.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/index.rst` & `GeoAlchemy2-0.9.4/doc/index.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_static/geoalchemy.png` & `GeoAlchemy2-0.9.4/doc/_static/geoalchemy.png`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_static/geoalchemy_small.png` & `GeoAlchemy2-0.9.4/doc/_static/geoalchemy_small.png`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_static/geoalchemy_small.svg` & `GeoAlchemy2-0.9.4/doc/_static/geoalchemy_small.svg`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_static/geoalchemy.svg` & `GeoAlchemy2-0.9.4/doc/_static/geoalchemy.svg`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/orm_tutorial.rst` & `GeoAlchemy2-0.9.4/doc/orm_tutorial.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/make.bat` & `GeoAlchemy2-0.9.4/doc/make.bat`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/spatialite_tutorial.rst` & `GeoAlchemy2-0.9.4/doc/spatialite_tutorial.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/Makefile` & `GeoAlchemy2-0.9.4/doc/Makefile`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/migrate.rst` & `GeoAlchemy2-0.9.4/doc/migrate.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_themes/LICENSE` & `GeoAlchemy2-0.9.4/doc/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_themes/flask/relations.html` & `GeoAlchemy2-0.9.4/doc/_themes/flask/relations.html`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_themes/flask/static/flasky.css_t` & `GeoAlchemy2-0.9.4/doc/_themes/flask/static/flasky.css_t`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_themes/flask/static/small_flask.css` & `GeoAlchemy2-0.9.4/doc/_themes/flask/static/small_flask.css`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_themes/flask/layout.html` & `GeoAlchemy2-0.9.4/doc/_themes/flask/layout.html`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/doc/_themes/README` & `GeoAlchemy2-0.9.4/doc/_themes/README`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/COPYING.rst` & `GeoAlchemy2-0.9.4/COPYING.rst`

 * *Files identical despite different names*

### Comparing `GeoAlchemy2-0.9.3/setup.py` & `GeoAlchemy2-0.9.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,12 +27,13 @@
     license='MIT',
     packages=find_packages(exclude=['ez_setup', 'examples', 'tests', 'doc']),
     include_package_data=True,
     zip_safe=False,
     setup_requires=["setuptools_scm"],
     install_requires=[
         'SQLAlchemy>=1.1',
+        'packaging'
     ],
     entry_points="""
     # -*- Entry points: -*-
     """,
 )
```

