# Comparing `tmp/marxs-1.2.tar.gz` & `tmp/marxs-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/marxs-1.2.tar", last modified: Fri Nov  6 18:53:45 2020, max compression
+gzip compressed data, was "marxs-2.0.tar", last modified: Thu May  2 13:35:13 2024, max compression
```

## Comparing `marxs-1.2.tar` & `marxs-2.0.tar`

### file list

```diff
@@ -1,246 +1,295 @@
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/
--rw-r--r--   0 hamogu     (501) staff       (20)     6794 2020-11-06 18:53:06.000000 marxs-1.2/CHANGES.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      309 2020-11-06 18:53:45.000000 marxs-1.2/PKG-INFO
--rw-r--r--   0 hamogu     (501) staff       (20)      867 2018-05-04 15:36:35.000000 marxs-1.2/README.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    37276 2019-07-15 10:56:35.000000 marxs-1.2/ah_bootstrap.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/
--rw-r--r--   0 hamogu     (501) staff       (20)    21843 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/CHANGES.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     1491 2016-05-21 09:00:23.000000 marxs-1.2/astropy_helpers/LICENSE.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     1459 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/README.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    37276 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/ah_bootstrap.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/astropy_helpers/
--rw-r--r--   0 hamogu     (501) staff       (20)     1738 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/__init__.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2016-05-21 09:00:23.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2738 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/_dummy.py
--rw-r--r--   0 hamogu     (501) staff       (20)     8674 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/build_ext.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9215 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/build_sphinx.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/src/
--rw-r--r--   0 hamogu     (501) staff       (20)     2720 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/src/compiler.c
--rw-r--r--   0 hamogu     (501) staff       (20)     1466 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/commands/test.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1930 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/conftest.py
--rw-r--r--   0 hamogu     (501) staff       (20)     8100 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/distutils_helpers.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6495 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/git_helpers.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9591 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/openmp_helpers.py
--rw-r--r--   0 hamogu     (501) staff       (20)    29074 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/setup_helpers.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/astropy_helpers/sphinx/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/sphinx/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)      156 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/sphinx/conf.py
--rw-r--r--   0 hamogu     (501) staff       (20)     8641 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/utils.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6974 2016-05-21 09:00:24.000000 marxs-1.2/astropy_helpers/astropy_helpers/version.py
--rw-r--r--   0 hamogu     (501) staff       (20)    12767 2019-06-25 11:02:28.000000 marxs-1.2/astropy_helpers/astropy_helpers/version_helpers.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/
--rw-r--r--   0 hamogu     (501) staff       (20)     2980 2016-05-21 09:00:25.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/PKG-INFO
--rw-r--r--   0 hamogu     (501) staff       (20)     3631 2016-05-21 09:00:25.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 hamogu     (501) staff       (20)        1 2016-05-21 09:00:25.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 hamogu     (501) staff       (20)        1 2016-05-21 09:00:25.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/not-zip-safe
--rw-r--r--   0 hamogu     (501) staff       (20)       47 2016-05-21 09:00:25.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/pbr.json
--rw-r--r--   0 hamogu     (501) staff       (20)       16 2016-05-21 09:00:25.000000 marxs-1.2/astropy_helpers/astropy_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/astropy_helpers/licenses/
--rw-r--r--   0 hamogu     (501) staff       (20)     1644 2017-11-02 20:35:08.000000 marxs-1.2/astropy_helpers/licenses/LICENSE_ASTROSCRAPPY.rst
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/
--rw-r--r--   0 hamogu     (501) staff       (20)     6758 2015-09-03 10:21:29.000000 marxs-1.2/docs/Makefile
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/_static/
--rw-r--r--   0 hamogu     (501) staff       (20)   204451 2018-05-04 15:36:35.000000 marxs-1.2/docs/_static/ex_pol.x3d
--rw-r--r--   0 hamogu     (501) staff       (20)      160 2015-09-03 10:21:29.000000 marxs-1.2/docs/_static/notes.txt
--rw-r--r--   0 hamogu     (501) staff       (20)   665045 2018-05-04 15:36:35.000000 marxs-1.2/docs/_static/subaperturing.x3d
--rw-r--r--   0 hamogu     (501) staff       (20)     6217 2018-05-04 15:36:35.000000 marxs-1.2/docs/_static/x3dom.css
--rw-r--r--   0 hamogu     (501) staff       (20)   972069 2018-05-04 15:36:35.000000 marxs-1.2/docs/_static/x3dom.js
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/_templates/
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/_templates/autosummary/
--rw-r--r--   0 hamogu     (501) staff       (20)      250 2018-05-04 15:36:35.000000 marxs-1.2/docs/_templates/autosummary/base.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      251 2018-05-04 15:36:35.000000 marxs-1.2/docs/_templates/autosummary/class.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      252 2018-05-04 15:36:35.000000 marxs-1.2/docs/_templates/autosummary/module.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      220 2018-05-04 15:36:35.000000 marxs-1.2/docs/_templates/layout.html
--rw-r--r--   0 hamogu     (501) staff       (20)       90 2018-05-04 15:36:35.000000 marxs-1.2/docs/changelog.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     5697 2019-07-15 11:22:04.000000 marxs-1.2/docs/conf.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2248 2018-05-04 15:36:35.000000 marxs-1.2/docs/contributing.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     7069 2018-05-04 15:36:35.000000 marxs-1.2/docs/conventions.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      199 2018-05-04 15:36:35.000000 marxs-1.2/docs/credits.rst
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/design/
--rw-r--r--   0 hamogu     (501) staff       (20)     5370 2020-08-11 00:17:58.000000 marxs-1.2/docs/design/rowland.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    15384 2019-02-17 20:31:34.000000 marxs-1.2/docs/design/tolerancing.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      357 2019-02-17 20:31:34.000000 marxs-1.2/docs/design/uncertainties.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      783 2019-02-17 20:31:34.000000 marxs-1.2/docs/design.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     6353 2020-09-03 10:44:25.000000 marxs-1.2/docs/examples.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     1568 2019-02-23 02:40:46.000000 marxs-1.2/docs/index.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     3544 2019-07-15 11:26:06.000000 marxs-1.2/docs/install.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      306 2018-05-04 15:36:35.000000 marxs-1.2/docs/licenses.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      863 2019-02-23 02:40:46.000000 marxs-1.2/docs/missions.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     6498 2020-09-03 10:44:25.000000 marxs-1.2/docs/newopticalelements.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    11412 2019-02-23 02:40:46.000000 marxs-1.2/docs/optics.rst
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/plots/
--rw-r--r--   0 hamogu     (501) staff       (20)      795 2015-09-03 10:21:29.000000 marxs-1.2/docs/plots/sketch_coords.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/docs/pyplots/
--rw-r--r--   0 hamogu     (501) staff       (20)      548 2019-02-17 20:31:34.000000 marxs-1.2/docs/pyplots/chandra_tolerancing.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1097 2020-09-03 10:44:25.000000 marxs-1.2/docs/pyplots/runexample.py
--rw-r--r--   0 hamogu     (501) staff       (20)      594 2020-09-03 10:44:25.000000 marxs-1.2/docs/pyplots/sourcespectrum.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2590 2020-09-03 10:44:25.000000 marxs-1.2/docs/pyplots/vis_pol.py
--rw-r--r--   0 hamogu     (501) staff       (20)     4591 2020-09-03 10:44:25.000000 marxs-1.2/docs/pyplots/vis_subaperturing.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5034 2020-09-03 10:44:25.000000 marxs-1.2/docs/results.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     6218 2020-09-03 10:44:25.000000 marxs-1.2/docs/runexample.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    10068 2020-09-03 10:44:25.000000 marxs-1.2/docs/source.rst
--rw-r--r--   0 hamogu     (501) staff       (20)     1541 2019-02-17 20:31:34.000000 marxs-1.2/docs/support.rst
--rw-r--r--   0 hamogu     (501) staff       (20)      429 2019-02-23 02:40:46.000000 marxs-1.2/docs/utils.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    11955 2020-09-03 10:44:25.000000 marxs-1.2/docs/visualization.rst
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/licenses/
--rw-r--r--   0 hamogu     (501) staff       (20)     1478 2018-05-04 15:36:35.000000 marxs-1.2/licenses/BSD_LICENSE.rst
--rw-r--r--   0 hamogu     (501) staff       (20)    35366 2018-05-04 15:36:35.000000 marxs-1.2/licenses/LICENSE.rst
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/
--rw-r--r--   0 hamogu     (501) staff       (20)      536 2018-05-04 15:36:35.000000 marxs-1.2/marxs/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5273 2018-05-04 15:36:35.000000 marxs-1.2/marxs/_astropy_init.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/analysis/
--rw-r--r--   0 hamogu     (501) staff       (20)      304 2018-05-04 15:36:35.000000 marxs-1.2/marxs/analysis/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     4008 2019-02-17 20:31:34.000000 marxs-1.2/marxs/analysis/analysis.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1623 2019-02-17 20:31:34.000000 marxs-1.2/marxs/analysis/coords.py
--rw-r--r--   0 hamogu     (501) staff       (20)    10143 2019-02-17 20:31:34.000000 marxs-1.2/marxs/analysis/gratings.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/analysis/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/analysis/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2300 2019-02-17 20:31:34.000000 marxs-1.2/marxs/analysis/tests/test_analysis.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1815 2019-02-17 20:31:34.000000 marxs-1.2/marxs/analysis/tests/test_grating.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/base/
--rw-r--r--   0 hamogu     (501) staff       (20)      232 2018-05-04 15:36:35.000000 marxs-1.2/marxs/base/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     8715 2020-08-11 10:23:45.000000 marxs-1.2/marxs/base/base.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2247 2019-02-23 02:40:46.000000 marxs-1.2/marxs/conftest.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/design/
--rw-r--r--   0 hamogu     (501) staff       (20)      278 2018-05-04 15:36:35.000000 marxs-1.2/marxs/design/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)    36897 2019-02-17 20:31:34.000000 marxs-1.2/marxs/design/rowland.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/design/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/design/tests/__init__.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/design/tests/data/
--rw-r--r--   0 hamogu     (501) staff       (20)    23040 2019-02-17 20:31:34.000000 marxs-1.2/marxs/design/tests/data/wiggle_global.fits
--rw-r--r--   0 hamogu     (501) staff       (20)      120 2019-02-17 20:31:34.000000 marxs-1.2/marxs/design/tests/setup_package.py
--rw-r--r--   0 hamogu     (501) staff       (20)    18575 2020-09-03 10:44:25.000000 marxs-1.2/marxs/design/tests/test_design.py
--rw-r--r--   0 hamogu     (501) staff       (20)    14068 2020-09-03 10:44:25.000000 marxs-1.2/marxs/design/tests/test_tolerancing.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2014 2018-05-04 15:36:35.000000 marxs-1.2/marxs/design/tests/test_uncertainties.py
--rw-r--r--   0 hamogu     (501) staff       (20)    26213 2020-09-18 21:29:09.000000 marxs-1.2/marxs/design/tolerancing.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1432 2019-02-17 20:31:34.000000 marxs-1.2/marxs/design/uncertainties.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/math/
--rw-r--r--   0 hamogu     (501) staff       (20)      451 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)    23851 2019-02-23 02:40:46.000000 marxs-1.2/marxs/math/geometry.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6124 2019-02-17 20:31:34.000000 marxs-1.2/marxs/math/pluecker.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6679 2019-02-17 20:31:34.000000 marxs-1.2/marxs/math/polarization.py
--rw-r--r--   0 hamogu     (501) staff       (20)     4116 2019-02-17 20:31:34.000000 marxs-1.2/marxs/math/random.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3094 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/rotations.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/math/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)    10807 2019-02-17 20:31:34.000000 marxs-1.2/marxs/math/tests/test_geometry.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2858 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/tests/test_math.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2457 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/tests/test_polarization.py
--rw-r--r--   0 hamogu     (501) staff       (20)      780 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/tests/test_random.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1537 2018-05-04 15:36:35.000000 marxs-1.2/marxs/math/tests/test_rotation.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1961 2019-02-17 20:31:34.000000 marxs-1.2/marxs/math/tests/test_utils.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5338 2019-02-17 20:31:34.000000 marxs-1.2/marxs/math/utils.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/missions/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2017-01-28 02:50:05.000000 marxs-1.2/marxs/missions/__init__.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/missions/chandra/
--rw-r--r--   0 hamogu     (501) staff       (20)    70950 2015-09-09 00:02:33.000000 marxs-1.2/marxs/missions/chandra/HESSdesign.rdb
--rw-r--r--   0 hamogu     (501) staff       (20)     1002 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6815 2019-02-17 20:31:34.000000 marxs-1.2/marxs/missions/chandra/acis.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1376 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/chandra.py
--rw-r--r--   0 hamogu     (501) staff       (20)     8729 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/data.py
--rw-r--r--   0 hamogu     (501) staff       (20)    12951 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/dither.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9342 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/fitsheaders.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3428 2019-02-17 20:31:34.000000 marxs-1.2/marxs/missions/chandra/hess.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1990 2020-08-11 00:17:58.000000 marxs-1.2/marxs/missions/chandra/hrma_py.py
--rw-r--r--   0 hamogu     (501) staff       (20)      358 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/setup_package.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/missions/chandra/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)   316800 2018-05-04 15:36:35.000000 marxs-1.2/marxs/missions/chandra/tests/sim_asol.fits
--rw-r--r--   0 hamogu     (501) staff       (20)     4817 2020-09-03 10:44:25.000000 marxs-1.2/marxs/missions/chandra/tests/test_chandra.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1580 2019-02-17 20:31:34.000000 marxs-1.2/marxs/missions/chandra/tests/test_hetg.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1421 2020-09-03 10:44:25.000000 marxs-1.2/marxs/missions/chandra/tests/test_hrma.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/missions/mitsnl/
--rw-r--r--   0 hamogu     (501) staff       (20)    28921 2019-06-25 10:16:07.000000 marxs-1.2/marxs/missions/mitsnl/SiTransmission.csv
--rw-r--r--   0 hamogu     (501) staff       (20)       49 2019-02-23 02:40:46.000000 marxs-1.2/marxs/missions/mitsnl/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)    16566 2020-10-23 00:58:58.000000 marxs-1.2/marxs/missions/mitsnl/catgrating.py
--rw-r--r--   0 hamogu     (501) staff       (20)      443 2019-02-23 02:40:46.000000 marxs-1.2/marxs/missions/mitsnl/setup_package.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/missions/mitsnl/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)       49 2019-02-23 02:40:46.000000 marxs-1.2/marxs/missions/mitsnl/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)      514 2019-02-23 02:40:46.000000 marxs-1.2/marxs/missions/mitsnl/tests/grating_efficiency.csv
--rw-r--r--   0 hamogu     (501) staff       (20)      495 2019-02-23 02:40:46.000000 marxs-1.2/marxs/missions/mitsnl/tests/grating_efficiency_broken.csv
--rw-r--r--   0 hamogu     (501) staff       (20)     4612 2020-08-11 00:17:58.000000 marxs-1.2/marxs/missions/mitsnl/tests/test_cat.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/optics/
--rw-r--r--   0 hamogu     (501) staff       (20)      624 2019-02-23 02:40:46.000000 marxs-1.2/marxs/optics/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     8524 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/aperture.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2038 2018-05-04 15:36:35.000000 marxs-1.2/marxs/optics/baffle.py
--rw-r--r--   0 hamogu     (501) staff       (20)    11543 2019-02-23 02:40:46.000000 marxs-1.2/marxs/optics/base.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3476 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/cdef.txt
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/optics/data/
--rwxr-xr-x   0 hamogu     (501) staff       (20)     1569 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/A12113.txt
--rwxr-xr-x   0 hamogu     (501) staff       (20)     1456 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/A13164.txt
--rwxr-xr-x   0 hamogu     (501) staff       (20)     1342 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/A14070B.txt
--rwxr-xr-x   0 hamogu     (501) staff       (20)      761 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/A14080B.txt
--rw-r--r--   0 hamogu     (501) staff       (20)     2555 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/ALSpolarization.txt
--rw-r--r--   0 hamogu     (501) staff       (20)     2521 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/ALSpolarization2.txt
--rw-r--r--   0 hamogu     (501) staff       (20)      162 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/data/testFile_mirror.txt
--rw-r--r--   0 hamogu     (501) staff       (20)     4454 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/detector.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3387 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/filter.py
--rw-r--r--   0 hamogu     (501) staff       (20)    12746 2019-02-23 02:40:46.000000 marxs-1.2/marxs/optics/grating.py
--rw-r--r--   0 hamogu     (501) staff       (20)    26242 2015-09-03 10:21:29.000000 marxs-1.2/marxs/optics/hrma.par
--rw-r--r--   0 hamogu     (501) staff       (20)     9032 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/marx.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1242 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/marx_build.py
--rw-r--r--   0 hamogu     (501) staff       (20)     4522 2020-09-03 10:44:25.000000 marxs-1.2/marxs/optics/mirror.py
--rw-r--r--   0 hamogu     (501) staff       (20)     7308 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/multiLayerMirror.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6399 2020-08-11 00:17:58.000000 marxs-1.2/marxs/optics/scatter.py
--rw-r--r--   0 hamogu     (501) staff       (20)      141 2018-05-04 15:36:35.000000 marxs-1.2/marxs/optics/setup_package.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/optics/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/optics/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9940 2020-09-03 10:44:25.000000 marxs-1.2/marxs/optics/tests/test_all_optics.py
--rw-r--r--   0 hamogu     (501) staff       (20)     4008 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/tests/test_apertures.py
--rw-r--r--   0 hamogu     (501) staff       (20)      763 2018-05-04 15:36:35.000000 marxs-1.2/marxs/optics/tests/test_baffle.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2042 2019-02-17 20:31:34.000000 marxs-1.2/marxs/optics/tests/test_detector.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1734 2019-07-15 10:56:35.000000 marxs-1.2/marxs/optics/tests/test_filter.py
--rw-r--r--   0 hamogu     (501) staff       (20)    14057 2020-08-11 00:17:58.000000 marxs-1.2/marxs/optics/tests/test_grating.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1341 2020-09-03 10:44:25.000000 marxs-1.2/marxs/optics/tests/test_marx.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1413 2020-09-03 10:44:25.000000 marxs-1.2/marxs/optics/tests/test_mirror.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6871 2018-05-04 15:36:35.000000 marxs-1.2/marxs/optics/tests/test_mlMirror.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5477 2020-09-03 10:44:25.000000 marxs-1.2/marxs/optics/tests/test_optics.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5427 2020-08-11 00:17:58.000000 marxs-1.2/marxs/optics/tests/test_scatter.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/simulator/
--rw-r--r--   0 hamogu     (501) staff       (20)      327 2019-02-17 20:31:34.000000 marxs-1.2/marxs/simulator/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)    27179 2020-09-03 10:44:25.000000 marxs-1.2/marxs/simulator/simulator.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/simulator/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/simulator/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3774 2019-02-17 20:31:34.000000 marxs-1.2/marxs/simulator/tests/test_parallel.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2812 2019-02-23 02:40:46.000000 marxs-1.2/marxs/simulator/tests/test_simulator.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/source/
--rw-r--r--   0 hamogu     (501) staff       (20)      457 2018-05-04 15:36:35.000000 marxs-1.2/marxs/source/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5838 2020-09-03 10:44:25.000000 marxs-1.2/marxs/source/labSource.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9206 2018-05-04 15:36:35.000000 marxs-1.2/marxs/source/pointing.py
--rw-r--r--   0 hamogu     (501) staff       (20)    21068 2020-09-18 21:29:09.000000 marxs-1.2/marxs/source/source.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/source/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/source/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)      778 2020-09-03 10:44:25.000000 marxs-1.2/marxs/source/tests/test_farLabPointSource.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3240 2020-09-03 10:44:25.000000 marxs-1.2/marxs/source/tests/test_labPointSource.py
--rw-r--r--   0 hamogu     (501) staff       (20)     5620 2020-09-03 10:44:25.000000 marxs-1.2/marxs/source/tests/test_pointing.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9880 2020-11-06 01:05:19.000000 marxs-1.2/marxs/source/tests/test_source.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)      300 2018-05-04 15:36:35.000000 marxs-1.2/marxs/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)      768 2018-05-04 15:36:35.000000 marxs-1.2/marxs/tests/coveragerc
--rw-r--r--   0 hamogu     (501) staff       (20)      145 2018-05-04 15:36:35.000000 marxs-1.2/marxs/tests/setup_package.py
--rw-r--r--   0 hamogu     (501) staff       (20)     4162 2020-09-03 10:44:25.000000 marxs-1.2/marxs/tests/test_analysis.py
--rw-r--r--   0 hamogu     (501) staff       (20)      420 2019-02-17 20:31:34.000000 marxs-1.2/marxs/tests/test_base.py
--rw-r--r--   0 hamogu     (501) staff       (20)      371 2018-05-04 15:36:35.000000 marxs-1.2/marxs/tests/test_general.py
--rw-r--r--   0 hamogu     (501) staff       (20)     3555 2019-02-17 20:31:34.000000 marxs-1.2/marxs/tests/test_simulator.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1247 2020-09-03 10:44:25.000000 marxs-1.2/marxs/tests/test_src_mir_det.py
--rw-r--r--   0 hamogu     (501) staff       (20)     1178 2019-02-17 20:31:34.000000 marxs-1.2/marxs/utils.py
--rw-r--r--   0 hamogu     (501) staff       (20)      414 2020-11-06 18:53:41.000000 marxs-1.2/marxs/version.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/visualization/
--rw-r--r--   0 hamogu     (501) staff       (20)      167 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     9786 2019-02-17 20:31:34.000000 marxs-1.2/marxs/visualization/mayavi.py
--rw-r--r--   0 hamogu     (501) staff       (20)      533 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/setup_package.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/visualization/tests/
--rw-r--r--   0 hamogu     (501) staff       (20)        0 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/tests/__init__.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6111 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/tests/test_threejsjson.py
--rw-r--r--   0 hamogu     (501) staff       (20)     6107 2019-02-17 20:31:34.000000 marxs-1.2/marxs/visualization/tests/test_utils.py
--rw-r--r--   0 hamogu     (501) staff       (20)    12195 2019-02-17 20:31:34.000000 marxs-1.2/marxs/visualization/threejs.py
-drwxr-xr-x   0 hamogu     (501) staff       (20)        0 2020-11-06 18:53:45.000000 marxs-1.2/marxs/visualization/threejs_files/
--rw-r--r--   0 hamogu     (501) staff       (20)     3222 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/threejs_files/MARXSloader.js
--rw-r--r--   0 hamogu     (501) staff       (20)     3727 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/threejs_files/ModifiedTorusBufferGeometry.js
--rw-r--r--   0 hamogu     (501) staff       (20)     2560 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/threejs_files/jsonschema.json
--rw-r--r--   0 hamogu     (501) staff       (20)     3188 2018-05-04 15:36:35.000000 marxs-1.2/marxs/visualization/threejs_files/loader.html
--rw-r--r--   0 hamogu     (501) staff       (20)     8731 2019-02-17 20:31:34.000000 marxs-1.2/marxs/visualization/threejsjson.py
--rw-r--r--   0 hamogu     (501) staff       (20)    10016 2019-02-17 20:31:34.000000 marxs-1.2/marxs/visualization/utils.py
--rw-r--r--   0 hamogu     (501) staff       (20)     2363 2020-11-06 18:53:06.000000 marxs-1.2/setup.cfg
--rw-r--r--   0 hamogu     (501) staff       (20)     4749 2019-07-15 10:56:35.000000 marxs-1.2/setup.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.780913 marxs-2.0/
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.643394 marxs-2.0/.github/
+-rw-r--r--   0 guenther   (501) staff       (20)      125 2023-01-18 17:46:31.000000 marxs-2.0/.github/dependabot.yml
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.643698 marxs-2.0/.github/workflows/
+-rw-r--r--   0 guenther   (501) staff       (20)     3236 2023-10-12 19:15:03.000000 marxs-2.0/.github/workflows/ci_tests.yml
+-rw-r--r--   0 guenther   (501) staff       (20)      769 2023-01-18 17:46:31.000000 marxs-2.0/.gitignore
+-rw-r--r--   0 guenther   (501) staff       (20)      994 2022-02-05 02:27:35.000000 marxs-2.0/.mailmap
+-rw-r--r--   0 guenther   (501) staff       (20)      501 2023-10-12 19:15:03.000000 marxs-2.0/.readthedocs.yaml
+-rw-r--r--   0 guenther   (501) staff       (20)    12959 2024-05-02 13:07:02.000000 marxs-2.0/CHANGES.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      970 2022-02-05 02:27:35.000000 marxs-2.0/CITATION
+-rw-r--r--   0 guenther   (501) staff       (20)     5417 2024-05-02 03:45:35.000000 marxs-2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 guenther   (501) staff       (20)      860 2022-02-05 02:27:35.000000 marxs-2.0/DESCRIPTION.rst
+-rw-r--r--   0 guenther   (501) staff       (20)    35147 2022-02-05 02:27:35.000000 marxs-2.0/LICENSE
+-rw-r--r--   0 guenther   (501) staff       (20)      298 2023-01-18 17:46:31.000000 marxs-2.0/MANIFEST.in
+-rw-r--r--   0 guenther   (501) staff       (20)     1337 2024-05-02 13:35:13.780809 marxs-2.0/PKG-INFO
+-rw-r--r--   0 guenther   (501) staff       (20)     2130 2024-05-02 13:27:59.000000 marxs-2.0/README.md
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.649902 marxs-2.0/docs/
+-rw-r--r--   0 guenther   (501) staff       (20)     6770 2024-01-30 16:57:08.000000 marxs-2.0/docs/Makefile
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.653571 marxs-2.0/docs/_static/
+-rw-r--r--   0 guenther   (501) staff       (20)   204451 2024-01-30 16:57:31.000000 marxs-2.0/docs/_static/ex_pol.x3d
+-rw-r--r--   0 guenther   (501) staff       (20)      160 2024-01-30 16:57:32.000000 marxs-2.0/docs/_static/notes.txt
+-rw-r--r--   0 guenther   (501) staff       (20)   665045 2024-01-30 16:57:33.000000 marxs-2.0/docs/_static/subaperturing.x3d
+-rw-r--r--   0 guenther   (501) staff       (20)     6217 2024-01-30 16:57:35.000000 marxs-2.0/docs/_static/x3dom.css
+-rw-r--r--   0 guenther   (501) staff       (20)   972069 2024-01-30 16:57:36.000000 marxs-2.0/docs/_static/x3dom.js
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.655590 marxs-2.0/docs/_templates/
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.656374 marxs-2.0/docs/_templates/autosummary/
+-rw-r--r--   0 guenther   (501) staff       (20)      250 2024-01-30 16:57:39.000000 marxs-2.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      251 2024-01-30 16:57:40.000000 marxs-2.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      252 2024-01-30 16:57:41.000000 marxs-2.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      220 2024-01-30 16:57:37.000000 marxs-2.0/docs/_templates/layout.html
+-rw-r--r--   0 guenther   (501) staff       (20)       90 2024-01-30 16:56:31.000000 marxs-2.0/docs/changelog.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     7965 2024-01-30 16:56:36.000000 marxs-2.0/docs/conf.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2248 2024-01-30 16:56:39.000000 marxs-2.0/docs/contributing.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     7617 2024-01-31 17:54:39.000000 marxs-2.0/docs/conventions.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      199 2024-01-30 16:56:46.000000 marxs-2.0/docs/credits.rst
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.657119 marxs-2.0/docs/design/
+-rw-r--r--   0 guenther   (501) staff       (20)     5222 2024-01-30 16:57:47.000000 marxs-2.0/docs/design/rowland.rst
+-rw-r--r--   0 guenther   (501) staff       (20)    16044 2024-01-31 02:54:48.000000 marxs-2.0/docs/design/tolerancing.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      357 2024-01-30 16:57:50.000000 marxs-2.0/docs/design/uncertainties.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      783 2024-01-30 16:56:49.000000 marxs-2.0/docs/design.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     9093 2024-01-31 02:54:48.000000 marxs-2.0/docs/examples.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     1569 2024-05-02 03:30:38.000000 marxs-2.0/docs/index.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     3592 2024-01-30 16:56:58.000000 marxs-2.0/docs/install.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      306 2024-01-30 16:57:04.000000 marxs-2.0/docs/licenses.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      863 2024-01-30 16:57:10.000000 marxs-2.0/docs/missions.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     6516 2024-01-30 16:57:22.000000 marxs-2.0/docs/newopticalelements.rst
+-rw-r--r--   0 guenther   (501) staff       (20)    11199 2024-01-30 16:57:18.000000 marxs-2.0/docs/optics.rst
+-rw-r--r--   0 guenther   (501) staff       (20)       81 2024-01-30 16:57:19.000000 marxs-2.0/docs/requirements.txt
+-rw-r--r--   0 guenther   (501) staff       (20)     5050 2024-01-30 16:57:23.000000 marxs-2.0/docs/results.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     7264 2024-01-31 02:54:48.000000 marxs-2.0/docs/runexample.rst
+-rw-r--r--   0 guenther   (501) staff       (20)    10599 2024-01-31 02:54:48.000000 marxs-2.0/docs/source.rst
+-rw-r--r--   0 guenther   (501) staff       (20)     1541 2024-01-30 16:57:27.000000 marxs-2.0/docs/support.rst
+-rw-r--r--   0 guenther   (501) staff       (20)      429 2024-01-30 16:57:28.000000 marxs-2.0/docs/utils.rst
+-rw-r--r--   0 guenther   (501) staff       (20)    17077 2024-01-31 02:54:48.000000 marxs-2.0/docs/visualization.rst
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.657597 marxs-2.0/examples/
+-rw-r--r--   0 guenther   (501) staff       (20)     2445 2023-10-12 19:15:03.000000 marxs-2.0/examples/chandra.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2232 2023-10-12 19:15:03.000000 marxs-2.0/examples/mlmirror.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.658134 marxs-2.0/licenses/
+-rw-r--r--   0 guenther   (501) staff       (20)     1478 2022-02-05 02:27:35.000000 marxs-2.0/licenses/BSD_LICENSE.rst
+-rw-r--r--   0 guenther   (501) staff       (20)    35366 2022-02-05 02:27:35.000000 marxs-2.0/licenses/LICENSE.rst
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.668668 marxs-2.0/marxs/
+-rw-r--r--   0 guenther   (501) staff       (20)      970 2022-02-05 02:27:35.000000 marxs-2.0/marxs/CITATION
+-rw-r--r--   0 guenther   (501) staff       (20)      439 2023-01-18 17:46:31.000000 marxs-2.0/marxs/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)      355 2023-01-18 17:46:31.000000 marxs-2.0/marxs/_astropy_init.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.670934 marxs-2.0/marxs/analysis/
+-rw-r--r--   0 guenther   (501) staff       (20)      304 2022-02-05 02:27:35.000000 marxs-2.0/marxs/analysis/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3865 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/analysis.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3288 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/coords.py
+-rw-r--r--   0 guenther   (501) staff       (20)    21713 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/gratings.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1070 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/plots.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1755 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/run_helpers.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.671659 marxs-2.0/marxs/analysis/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/analysis/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2300 2022-02-05 02:27:35.000000 marxs-2.0/marxs/analysis/tests/test_analysis.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1431 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/tests/test_coords.py
+-rw-r--r--   0 guenther   (501) staff       (20)     9819 2023-10-12 19:15:03.000000 marxs-2.0/marxs/analysis/tests/test_grating.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.672046 marxs-2.0/marxs/base/
+-rw-r--r--   0 guenther   (501) staff       (20)      112 2023-10-12 19:15:03.000000 marxs-2.0/marxs/base/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    13704 2023-10-12 19:15:03.000000 marxs-2.0/marxs/base/base.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.672406 marxs-2.0/marxs/base/test/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2023-01-18 17:46:31.000000 marxs-2.0/marxs/base/test/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3141 2023-10-12 19:15:03.000000 marxs-2.0/marxs/base/test/test_base.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1477 2024-02-05 14:52:10.000000 marxs-2.0/marxs/conftest.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.673731 marxs-2.0/marxs/design/
+-rw-r--r--   0 guenther   (501) staff       (20)      260 2023-10-12 19:15:03.000000 marxs-2.0/marxs/design/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     7636 2023-10-12 19:15:03.000000 marxs-2.0/marxs/design/bendgratings.py
+-rw-r--r--   0 guenther   (501) staff       (20)    36272 2024-03-18 15:04:20.000000 marxs-2.0/marxs/design/rowland.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.674740 marxs-2.0/marxs/design/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/design/tests/__init__.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.675006 marxs-2.0/marxs/design/tests/data/
+-rw-r--r--   0 guenther   (501) staff       (20)    23040 2022-02-05 02:27:35.000000 marxs-2.0/marxs/design/tests/data/wiggle_global.fits
+-rw-r--r--   0 guenther   (501) staff       (20)    22157 2024-02-09 20:58:17.000000 marxs-2.0/marxs/design/tests/test_design.py
+-rw-r--r--   0 guenther   (501) staff       (20)    14663 2023-10-12 19:15:03.000000 marxs-2.0/marxs/design/tests/test_tolerancing.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2006 2023-10-12 19:15:03.000000 marxs-2.0/marxs/design/tests/test_uncertainties.py
+-rw-r--r--   0 guenther   (501) staff       (20)    28549 2023-10-12 19:15:03.000000 marxs-2.0/marxs/design/tolerancing.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1733 2023-10-12 19:15:03.000000 marxs-2.0/marxs/design/uncertainties.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.676990 marxs-2.0/marxs/math/
+-rw-r--r--   0 guenther   (501) staff       (20)      451 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    24040 2023-01-18 17:46:44.000000 marxs-2.0/marxs/math/geometry.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6124 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/pluecker.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6636 2023-01-18 17:46:31.000000 marxs-2.0/marxs/math/polarization.py
+-rw-r--r--   0 guenther   (501) staff       (20)     4116 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/random.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3095 2023-10-12 19:15:03.000000 marxs-2.0/marxs/math/rotations.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.678213 marxs-2.0/marxs/math/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    10404 2023-10-12 19:15:03.000000 marxs-2.0/marxs/math/tests/test_geometry.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2858 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/tests/test_math.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2457 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/tests/test_polarization.py
+-rw-r--r--   0 guenther   (501) staff       (20)      780 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/tests/test_random.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1537 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/tests/test_rotation.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1961 2022-02-05 02:27:35.000000 marxs-2.0/marxs/math/tests/test_utils.py
+-rw-r--r--   0 guenther   (501) staff       (20)     5591 2023-10-12 19:15:03.000000 marxs-2.0/marxs/math/utils.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.678367 marxs-2.0/marxs/missions/
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.678959 marxs-2.0/marxs/missions/AXIS/
+-rw-r--r--   0 guenther   (501) staff       (20)    10184 2024-02-10 12:13:58.000000 marxs-2.0/marxs/missions/AXIS/AXIS.py
+-rw-r--r--   0 guenther   (501) staff       (20)      539 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/AXIS/AXIS_metashellgeom.dat
+-rw-r--r--   0 guenther   (501) staff       (20)       48 2023-08-08 16:33:59.000000 marxs-2.0/marxs/missions/__init__.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.681182 marxs-2.0/marxs/missions/arcus/
+-rw-r--r--   0 guenther   (501) staff       (20)       88 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     7946 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/analyze_grid.py
+-rw-r--r--   0 guenther   (501) staff       (20)    23112 2024-02-05 14:52:10.000000 marxs-2.0/marxs/missions/arcus/arcus.py
+-rw-r--r--   0 guenther   (501) staff       (20)    12761 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/arfrmf.py
+-rw-r--r--   0 guenther   (501) staff       (20)     5074 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/boom.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.681339 marxs-2.0/marxs/missions/arcus/data/
+-rw-r--r--   0 guenther   (501) staff       (20)     3281 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/data/osip_template.md
+-rw-r--r--   0 guenther   (501) staff       (20)     2656 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/defaults.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2473 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/load_csv.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6068 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/ralfgrating.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2426 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/spo.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.682455 marxs-2.0/marxs/missions/arcus/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)      121 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6574 2024-05-02 04:06:11.000000 marxs-2.0/marxs/missions/arcus/tests/test_arfrmf.py
+-rw-r--r--   0 guenther   (501) staff       (20)      939 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/tests/test_blaze.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1938 2024-02-05 14:52:10.000000 marxs-2.0/marxs/missions/arcus/tests/test_layout.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3557 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/tests/test_orders.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2230 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/arcus/utils.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.682994 marxs-2.0/marxs/missions/athena/
+-rw-r--r--   0 guenther   (501) staff       (20)       48 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/athena/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     9980 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/athena/athecat.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.727593 marxs-2.0/marxs/missions/athena/data/
+-rw-r--r--   0 guenther   (501) staff       (20) 23626824 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/athena/data/coated_reflectivity.csv
+-rw-r--r--   0 guenther   (501) staff       (20)      957 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/athena/data/lossterm.csv
+-rw-r--r--   0 guenther   (501) staff       (20)  1922974 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/athena/data/xous.csv
+-rw-r--r--   0 guenther   (501) staff       (20)     6658 2024-02-11 00:57:39.000000 marxs-2.0/marxs/missions/athena/spo.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.752076 marxs-2.0/marxs/missions/chandra/
+-rw-r--r--   0 guenther   (501) staff       (20)    70950 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/chandra/HESSdesign.rdb
+-rw-r--r--   0 guenther   (501) staff       (20)     1013 2023-08-08 16:33:59.000000 marxs-2.0/marxs/missions/chandra/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1363 2023-08-08 16:33:59.000000 marxs-2.0/marxs/missions/chandra/chandra_global.py
+-rw-r--r--   0 guenther   (501) staff       (20)     8730 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/data.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6777 2023-08-08 16:33:59.000000 marxs-2.0/marxs/missions/chandra/det_acis.py
+-rw-r--r--   0 guenther   (501) staff       (20)    12973 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/dither.py
+-rw-r--r--   0 guenther   (501) staff       (20)     9342 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/chandra/fitsheaders.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3474 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/hess.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1977 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/hrma_py.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.753716 marxs-2.0/marxs/missions/chandra/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/chandra/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    27731 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/chandra/tests/marx.par
+-rw-r--r--   0 guenther   (501) staff       (20)      700 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/chandra/tests/marxasp.par
+-rw-r--r--   0 guenther   (501) staff       (20)   316800 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/chandra/tests/sim_asol.fits
+-rw-r--r--   0 guenther   (501) staff       (20)     5339 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/tests/test_chandra.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1581 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/tests/test_hetg.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1421 2023-01-18 17:46:31.000000 marxs-2.0/marxs/missions/chandra/tests/test_hrma.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.754914 marxs-2.0/marxs/missions/lynx/
+-rw-r--r--   0 guenther   (501) staff       (20)       48 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/__init__.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.756052 marxs-2.0/marxs/missions/lynx/data/
+-rw-r--r--   0 guenther   (501) staff       (20)    29372 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/data/filtersqe.dat
+-rw-r--r--   0 guenther   (501) staff       (20)    98989 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/data/ir_reflectivity.dat
+-rw-r--r--   0 guenther   (501) staff       (20)    30851 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/data/metashelleff.dat
+-rw-r--r--   0 guenther   (501) staff       (20)     1574 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/data/metashellgeom.dat
+-rw-r--r--   0 guenther   (501) staff       (20)     1160 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/load_csv.py
+-rw-r--r--   0 guenther   (501) staff       (20)    11719 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/lynx.py
+-rw-r--r--   0 guenther   (501) staff       (20)     4008 2024-02-14 12:11:32.000000 marxs-2.0/marxs/missions/lynx/mirror.py
+-rw-r--r--   0 guenther   (501) staff       (20)      715 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/lynx/ralfgrating.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.756677 marxs-2.0/marxs/missions/mitsnl/
+-rw-r--r--   0 guenther   (501) staff       (20)       49 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/mitsnl/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    15440 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/catgrating.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.760296 marxs-2.0/marxs/missions/mitsnl/data/
+-rw-r--r--   0 guenther   (501) staff       (20)  1080189 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/data/SiPt_efficiency_5_7.dat
+-rw-r--r--   0 guenther   (501) staff       (20)    28921 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/data/SiTransmission.csv
+-rw-r--r--   0 guenther   (501) staff       (20)  1097959 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/data/Si_efficiency_5_7.dat
+-rw-r--r--   0 guenther   (501) staff       (20)    90860 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/data/Si_efficiency_5_7_widebars.ecsv
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.762139 marxs-2.0/marxs/missions/mitsnl/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)       49 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/mitsnl/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)      514 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/mitsnl/tests/grating_efficiency.csv
+-rw-r--r--   0 guenther   (501) staff       (20)      495 2022-02-05 02:27:35.000000 marxs-2.0/marxs/missions/mitsnl/tests/grating_efficiency_broken.csv
+-rw-r--r--   0 guenther   (501) staff       (20)     5402 2023-03-22 17:41:32.000000 marxs-2.0/marxs/missions/mitsnl/tests/test_cat.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2412 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/tests/test_tolerances.py
+-rw-r--r--   0 guenther   (501) staff       (20)     4099 2023-10-12 19:15:03.000000 marxs-2.0/marxs/missions/mitsnl/tolerances.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.765716 marxs-2.0/marxs/optics/
+-rw-r--r--   0 guenther   (501) staff       (20)      625 2023-08-08 16:33:59.000000 marxs-2.0/marxs/optics/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     8484 2023-10-12 19:15:03.000000 marxs-2.0/marxs/optics/aperture.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2038 2023-08-08 16:33:59.000000 marxs-2.0/marxs/optics/baffles.py
+-rw-r--r--   0 guenther   (501) staff       (20)    13192 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/base.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3482 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/cdef.txt
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.766848 marxs-2.0/marxs/optics/data/
+-rwxr-xr-x   0 guenther   (501) staff       (20)     1569 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/A12113.txt
+-rwxr-xr-x   0 guenther   (501) staff       (20)     1456 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/A13164.txt
+-rwxr-xr-x   0 guenther   (501) staff       (20)     1342 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/A14070B.txt
+-rwxr-xr-x   0 guenther   (501) staff       (20)      761 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/A14080B.txt
+-rw-r--r--   0 guenther   (501) staff       (20)     2555 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/ALSpolarization.txt
+-rw-r--r--   0 guenther   (501) staff       (20)     2521 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/ALSpolarization2.txt
+-rw-r--r--   0 guenther   (501) staff       (20)      162 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/data/testFile_mirror.txt
+-rw-r--r--   0 guenther   (501) staff       (20)     7467 2024-05-02 04:06:11.000000 marxs-2.0/marxs/optics/detector.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3308 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/filter.py
+-rw-r--r--   0 guenther   (501) staff       (20)    12845 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/grating.py
+-rw-r--r--   0 guenther   (501) staff       (20)    26242 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/hrma.par
+-rw-r--r--   0 guenther   (501) staff       (20)     9014 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/marx.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1283 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/marx_build.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6019 2024-02-11 00:57:39.000000 marxs-2.0/marxs/optics/mirror.py
+-rw-r--r--   0 guenther   (501) staff       (20)     7816 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/multiLayerMirror.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6432 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/scatter.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.769235 marxs-2.0/marxs/optics/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/tests/__init__.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.769386 marxs-2.0/marxs/optics/tests/data/
+-rw-r--r--   0 guenther   (501) staff       (20)    82917 2023-10-12 19:15:03.000000 marxs-2.0/marxs/optics/tests/data/ccd_redist_normal.ecsv
+-rw-r--r--   0 guenther   (501) staff       (20)    10012 2023-10-12 19:15:03.000000 marxs-2.0/marxs/optics/tests/test_all_optics.py
+-rw-r--r--   0 guenther   (501) staff       (20)     4008 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/tests/test_apertures.py
+-rw-r--r--   0 guenther   (501) staff       (20)      764 2023-08-08 16:33:59.000000 marxs-2.0/marxs/optics/tests/test_baffle.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1101 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/tests/test_base.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2941 2024-05-02 04:06:11.000000 marxs-2.0/marxs/optics/tests/test_detector.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1734 2022-02-05 02:27:35.000000 marxs-2.0/marxs/optics/tests/test_filter.py
+-rw-r--r--   0 guenther   (501) staff       (20)    14033 2023-03-22 17:41:32.000000 marxs-2.0/marxs/optics/tests/test_grating.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1526 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/tests/test_marx.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2968 2024-02-11 00:57:39.000000 marxs-2.0/marxs/optics/tests/test_mirror.py
+-rw-r--r--   0 guenther   (501) staff       (20)     7653 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/tests/test_mlMirror.py
+-rw-r--r--   0 guenther   (501) staff       (20)     5477 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/tests/test_optics.py
+-rw-r--r--   0 guenther   (501) staff       (20)     5427 2023-01-18 17:46:31.000000 marxs-2.0/marxs/optics/tests/test_scatter.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.770697 marxs-2.0/marxs/reduction/
+-rw-r--r--   0 guenther   (501) staff       (20)       48 2023-10-12 19:15:03.000000 marxs-2.0/marxs/reduction/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    17944 2024-01-29 17:23:45.000000 marxs-2.0/marxs/reduction/lsfparm.py
+-rw-r--r--   0 guenther   (501) staff       (20)    21749 2023-10-12 19:15:03.000000 marxs-2.0/marxs/reduction/ogip.py
+-rw-r--r--   0 guenther   (501) staff       (20)    21961 2024-05-02 04:06:11.000000 marxs-2.0/marxs/reduction/osip.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.772103 marxs-2.0/marxs/reduction/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)       49 2023-10-12 19:15:03.000000 marxs-2.0/marxs/reduction/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1663 2023-10-12 19:15:03.000000 marxs-2.0/marxs/reduction/tests/test_col_or_key.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2575 2023-10-12 19:15:03.000000 marxs-2.0/marxs/reduction/tests/test_ogip.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6573 2024-05-02 04:06:11.000000 marxs-2.0/marxs/reduction/tests/test_osip.py
+-rw-r--r--   0 guenther   (501) staff       (20)      671 2023-10-12 19:15:03.000000 marxs-2.0/marxs/reduction/tests/test_rmf.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.772499 marxs-2.0/marxs/simulator/
+-rw-r--r--   0 guenther   (501) staff       (20)      327 2022-02-05 02:27:35.000000 marxs-2.0/marxs/simulator/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    28511 2023-10-12 19:15:03.000000 marxs-2.0/marxs/simulator/simulator.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.772922 marxs-2.0/marxs/simulator/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/simulator/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3843 2023-10-12 19:15:03.000000 marxs-2.0/marxs/simulator/tests/test_parallel.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3215 2023-01-18 17:46:31.000000 marxs-2.0/marxs/simulator/tests/test_simulator.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.773965 marxs-2.0/marxs/source/
+-rw-r--r--   0 guenther   (501) staff       (20)      462 2023-08-08 16:33:59.000000 marxs-2.0/marxs/source/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)    21002 2023-08-08 16:33:59.000000 marxs-2.0/marxs/source/basesources.py
+-rw-r--r--   0 guenther   (501) staff       (20)     5791 2023-08-08 16:33:59.000000 marxs-2.0/marxs/source/labSource.py
+-rw-r--r--   0 guenther   (501) staff       (20)     9285 2023-01-18 17:46:31.000000 marxs-2.0/marxs/source/pointing.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.774929 marxs-2.0/marxs/source/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/source/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)      778 2023-01-18 17:46:31.000000 marxs-2.0/marxs/source/tests/test_farLabPointSource.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3240 2023-01-18 17:46:31.000000 marxs-2.0/marxs/source/tests/test_labPointSource.py
+-rw-r--r--   0 guenther   (501) staff       (20)     5620 2023-01-18 17:46:31.000000 marxs-2.0/marxs/source/tests/test_pointing.py
+-rw-r--r--   0 guenther   (501) staff       (20)     9885 2023-08-08 16:33:59.000000 marxs-2.0/marxs/source/tests/test_source.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.776389 marxs-2.0/marxs/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)      300 2022-02-05 02:27:35.000000 marxs-2.0/marxs/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     4115 2023-10-12 19:15:03.000000 marxs-2.0/marxs/tests/test_analysis.py
+-rw-r--r--   0 guenther   (501) staff       (20)      420 2022-02-05 02:27:35.000000 marxs-2.0/marxs/tests/test_base.py
+-rw-r--r--   0 guenther   (501) staff       (20)      371 2022-02-05 02:27:35.000000 marxs-2.0/marxs/tests/test_general.py
+-rw-r--r--   0 guenther   (501) staff       (20)     3555 2022-02-05 02:27:35.000000 marxs-2.0/marxs/tests/test_simulator.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1369 2023-01-18 17:46:31.000000 marxs-2.0/marxs/tests/test_src_mir_det.py
+-rw-r--r--   0 guenther   (501) staff       (20)     1400 2023-03-22 17:41:32.000000 marxs-2.0/marxs/tests/test_utils_in_rootdir.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2772 2024-05-02 04:06:11.000000 marxs-2.0/marxs/utils.py
+-rw-r--r--   0 guenther   (501) staff       (20)      335 2024-05-02 13:35:13.000000 marxs-2.0/marxs/version.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.777787 marxs-2.0/marxs/visualization/
+-rw-r--r--   0 guenther   (501) staff       (20)      761 2024-01-31 02:54:48.000000 marxs-2.0/marxs/visualization/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     9056 2023-03-22 17:41:32.000000 marxs-2.0/marxs/visualization/mayavi.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.778807 marxs-2.0/marxs/visualization/tests/
+-rw-r--r--   0 guenther   (501) staff       (20)        0 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/tests/__init__.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6112 2023-03-22 17:41:32.000000 marxs-2.0/marxs/visualization/tests/test_threejsjson.py
+-rw-r--r--   0 guenther   (501) staff       (20)     6107 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/tests/test_utils.py
+-rw-r--r--   0 guenther   (501) staff       (20)     4142 2024-04-09 14:54:55.000000 marxs-2.0/marxs/visualization/tests/test_x3d.py
+-rw-r--r--   0 guenther   (501) staff       (20)    12195 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/threejs.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.779578 marxs-2.0/marxs/visualization/threejs_files/
+-rw-r--r--   0 guenther   (501) staff       (20)     3222 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/threejs_files/MARXSloader.js
+-rw-r--r--   0 guenther   (501) staff       (20)     3727 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/threejs_files/ModifiedTorusBufferGeometry.js
+-rw-r--r--   0 guenther   (501) staff       (20)     2560 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/threejs_files/jsonschema.json
+-rw-r--r--   0 guenther   (501) staff       (20)     3188 2022-02-05 02:27:35.000000 marxs-2.0/marxs/visualization/threejs_files/loader.html
+-rw-r--r--   0 guenther   (501) staff       (20)     8747 2023-08-08 16:33:59.000000 marxs-2.0/marxs/visualization/threejsjson.py
+-rw-r--r--   0 guenther   (501) staff       (20)    11371 2024-01-31 02:54:48.000000 marxs-2.0/marxs/visualization/utils.py
+-rw-r--r--   0 guenther   (501) staff       (20)    13885 2024-04-09 14:54:55.000000 marxs-2.0/marxs/visualization/x3d.py
+drwxr-xr-x   0 guenther   (501) staff       (20)        0 2024-05-02 13:35:13.779835 marxs-2.0/marxs.egg-info/
+-rw-r--r--   0 guenther   (501) staff       (20)     1337 2024-05-02 13:35:13.000000 marxs-2.0/marxs.egg-info/PKG-INFO
+-rw-r--r--   0 guenther   (501) staff       (20)     7390 2024-05-02 13:35:13.000000 marxs-2.0/marxs.egg-info/SOURCES.txt
+-rw-r--r--   0 guenther   (501) staff       (20)        1 2024-05-02 13:35:13.000000 marxs-2.0/marxs.egg-info/dependency_links.txt
+-rw-r--r--   0 guenther   (501) staff       (20)        1 2023-08-08 15:56:10.000000 marxs-2.0/marxs.egg-info/not-zip-safe
+-rw-r--r--   0 guenther   (501) staff       (20)      173 2024-05-02 13:35:13.000000 marxs-2.0/marxs.egg-info/requires.txt
+-rw-r--r--   0 guenther   (501) staff       (20)        6 2024-05-02 13:35:13.000000 marxs-2.0/marxs.egg-info/top_level.txt
+-rw-r--r--   0 guenther   (501) staff       (20)    11520 2024-05-02 03:14:08.000000 marxs-2.0/mysim_result.fits
+-rw-r--r--   0 guenther   (501) staff       (20)      149 2023-03-22 17:41:32.000000 marxs-2.0/pyproject.toml
+-rw-r--r--   0 guenther   (501) staff       (20)     2138 2024-05-02 13:35:13.781407 marxs-2.0/setup.cfg
+-rw-r--r--   0 guenther   (501) staff       (20)     2760 2023-01-18 17:46:31.000000 marxs-2.0/setup.py
+-rw-r--r--   0 guenther   (501) staff       (20)     2780 2023-10-12 19:15:03.000000 marxs-2.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `marxs-1.2/astropy_helpers/LICENSE.rst` & `marxs-2.0/licenses/BSD_LICENSE.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-Copyright (c) 2014, Astropy Developers
-
+Copyright (c) year, author
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
 * Redistributions of source code must retain the above copyright notice, this
   list of conditions and the following disclaimer.
```

### Comparing `marxs-1.2/docs/Makefile` & `marxs-2.0/docs/Makefile`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 	@echo "  xml        to make Docutils-native XML files"
 	@echo "  pseudoxml  to make pseudoxml-XML files for display purposes"
 	@echo "  linkcheck  to check all external links for integrity"
 	@echo "  doctest    to run all doctests embedded in the documentation (if enabled)"
 
 clean:
 	rm -rf $(BUILDDIR)/*
+	rm -rf api
 
 html:
 	$(SPHINXBUILD) -b html $(ALLSPHINXOPTS) $(BUILDDIR)/html
 	@echo
 	@echo "Build finished. The HTML pages are in $(BUILDDIR)/html."
 
 dirhtml:
```

### Comparing `marxs-1.2/docs/_static/ex_pol.x3d` & `marxs-2.0/docs/_static/ex_pol.x3d`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/_static/subaperturing.x3d` & `marxs-2.0/docs/_static/subaperturing.x3d`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/_static/x3dom.css` & `marxs-2.0/docs/_static/x3dom.css`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/_static/x3dom.js` & `marxs-2.0/docs/_static/x3dom.js`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/contributing.rst` & `marxs-2.0/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/conventions.rst` & `marxs-2.0/docs/conventions.rst`

 * *Files 8% similar despite different names*

```diff
@@ -5,59 +5,75 @@
 .. _coordsys:
 .. _pos4d:
 
 Coordinate system
 =================
 Marxs employs a cartesian coordinate system. All optical elements can be freely placed at any position
 and any angle in this space, but we recommend the following conventions for simplicity (examples and
-predefined missions in this pckage follow those conventions as far as possible):
+predefined missions in this package follow those conventions as far as possible):
 
 - The optical axis of the telescope coincides with the x-axis. A source on the optical axis is
   at :math:`x=+\infty` and photons travel towards the origin.
-- The origin of the coordiante system is at the telescope focus.
+- The origin of the coordinate system is at the telescope focus.
 - The y-axis coincides with the dispersion direction of gratings.
 
 Marxs uses `homogeneous coordinates <https://en.wikipedia.org/wiki/Homogeneous_coordinates>`_, which
 describe position and direction in a 4 dimensional coordinate space, for example
 :math:`[3, 0, 0, 1]` describes a point at x=3, y=0 and z=0; :math:`[3, 0, 0, 0]` describes the
 vector from the origin to that point. Homogeneous coordinates have one important advantage compared
-with a normal 3-d description of euklidean space: In homogenous coordinates, rotation, zoom, and
+with a normal 3-d description of Euklidean space: In homogeneous coordinates, rotation, zoom, and
 translations together can be described by a :math:`[4, 4]` matrix and several of these operations can
 be chained simply by multiplying the matrices.
 
 Every optical element in marxs (and some other objects, too) has such a :math:`[4, 4]` matrix
 associated with it in an attribute called ``element.pos4d``.
 
 All optical elements have some default location and position. Typically, their active surface (e.g.
 the surface of a mirror or detector) is in the y-z plane. The center is at the origin of the
-coordiante system and the default size in each dimenstion is 1, measured from the center.
+coordinate system and the default size in each dimension is 1, measured from the center.
 Thus, e.g. the default definition for a `marxs.optics.detector.FlatDetector`, makes a detector surface with
 the following corners (in 3-d x,y,z coordinates): [0, -1, -1], [0, -1, 1], [0,
 1, 1] and [0, 1, -1].
 Note that in a 3D visualization (see :ref:`visualization`), some elements might be shown with a thickness
 2 (from :math:`x=-1` to :math:`x=+1`), so that the "active surface" is in the middle of a box,
 while others might show the "active surface" as the edge of the box as in the
 sketch below. Details depend on the capabilities of the plotting backend
 (backends and options are listed in :ref:`sect-vis-api`).
 
 However, when running the ray-trace the code
 calculates the intersection with the "active surface" in the y-z plane independent of the
-thickeness in x-direction. There are exceptions to these defaults, those are noted in the description
+thickness in x-direction. There are exceptions to these defaults, those are noted in the description
 of the individual optical elements.
 See the following sketch, where the "active surface" is shown in red:
 
-.. plot:: plots/sketch_coords.py optical_element_coords
+.. plot::
    :scale: 50
    :align: center
    :include-source: False
-   :alt: Layout of the default size and position of an optical elements. The "active surface" (e.g. the surface of a mirror) is shown in red.
+   :alt: Layout of the default size and position of an optical element. The "active surface" (e.g. the surface of a mirror) is shown in red.
+
+   import matplotlib.pyplot as plt
+   from mpl_toolkits.mplot3d import Axes3D
+   import numpy as np
+
+   fig = plt.figure()
+   ax = fig.add_subplot(111, projection='3d')
+   ax.quiver([2,0,0],[0,2,0],[0,0, 2],[1,0,0],[0,1,0], [0,0,1], length=4, arrow_length_ratio=.05, color='k', lw=2)
+   ax.bar3d(-1, -1, -1, 1, 2, 2, zsort='average', alpha=0.5, color=['b'] *5 + ['r'], zorder=1)
+   ax.set_axis_off()
+   ax.text(2.1, 0, 0, 'x', None, fontsize='x-large')
+   ax.text(0, 2.1, 0, 'y', None, fontsize='x-large')
+   ax.text(0, 0, 2.1, 'z', None, fontsize='x-large')
+   ax.set_xlim([-1.2,1.2])
+   ax.set_ylim([-1.2,1.2])
+   ax.set_zlim([-1.2,1.2])
 
 
 In order to place elements in the experiment, the optical element needs to be
-scaled (zoomed), rotatated and translated to the the new position.
+scaled (zoomed), rotated and translated to the new position.
 There are two ways to specify that:
 
 - Pass a :math:`[4,4]` matrix to the optical element:
 
       >>> import numpy as np
       >>> from marxs.optics import Baffle
       >>> pos4d = np.array([[1., 0., 0., 5.],
@@ -129,15 +145,14 @@
 MARXS uses `astropy units
 <http://astropy.readthedocs.io/en/stable/units/index.html>` and
 `astropy.coordinates.SkyCoord` for input of source properties and
 coordinates. This makes quantities having a specific unit and avoids confusion
 between degree and radian, eV and keV and so on.
 
 Internally, however, this extra unit makes the computation too slow. Thus, all
-properties are converted to float when they his the first optical element using
-the following conventions:
+properties are converted to float using the following conventions:
 
 - Length: base unit is mm.
 - Energy: base unit is keV.
 - Angles: Always expressed in radian.
 
-When designing an instrument, these units much be used.
+When designing an instrument, these units must be used.
```

### Comparing `marxs-1.2/docs/design/rowland.rst` & `marxs-2.0/docs/design/rowland.rst`

 * *Files 6% similar despite different names*

```diff
@@ -7,78 +7,77 @@
 know the best places for gratings, detectors etc.?
 In some cases, analytical work can tell us where e.g. diffraction gratings and detectors need
 to go to achieve the best possible resolving power. The module `marxs.design.rowland` implements those
 formulas for a spectrometer in a Rowland Torus design (see e.g.
 `Paerels 1999 <http://adsabs.harvard.edu/abs/1999LNP...520..347P>`_ and
 `Paerels 2010 <http://adsabs.harvard.edu/abs/2010SSRv..157...15P>`_ for a derivation).
 
-In the following example, we define a Rowlandtorus based spectrometer. In this
+In the following example, we define a Rowland torus based spectrometer. In this
 case, we select the radius of the Rowland Circle to be very small (1 m) and
 also make the grating constant of the gratings very small. This way we get a
-much larger diffraction angle than usual and we end up with a model that does
+much larger diffraction angle than usual, and we end up with a model that does
 real ray-tracing (albeit with some unrealistic input values) and delivers very
-clear images to demonstante the operating principles for teaching. We begin by
-importing the relevant packages and then we define the Rowland torus.  In this
+clear images to demonstrate the operating principles for teaching. We begin by
+importing the relevant packages, and then we define the Rowland torus.  In this
 case, both radii of the torus are set to 500 mm, so the Rowland circle in the
-x,y plane touches the focal point at (0,0) and has a diameter of 1 m, so
+x, y plane touches the focal point at (0,0) and has a diameter of 1 m, so
 grating on the optical axis would be 1 m away from the focal point::
 
   >>> import numpy as np
   >>> import astropy.units as u
   >>> from marxs import optics
   >>> from marxs import simulator
   >>> from marxs.design import rowland
   >>> my_torus = rowland.RowlandTorus(500, 500)
 
 Our instrument approximates an imaging optic by using a circular aperture that illuminates
 a `marxs.optics.PerfectLens` with some additional scatter
-(an `marxs.optics.RadialMirrorScatter`). The reflection on the mirror and the scatter always
+(`marxs.optics.RadialMirrorScatter`). The reflection on the mirror and the scatter always
 happen at the same position, so those two functions are summarized in a single element
 (a `marxs.optics.FlatStack`) as explained in :ref:`complexgeometry`::
-  
+
   >>> aperture = optics.CircleAperture(position=[1200, 0, 0], zoom=[1, 100, 100])
   >>> mirror = optics.FlatStack(position=[1100, 0, 0], zoom=[20, 100, 100],
   ...                            elements=[optics.PerfectLens, optics.RadialMirrorScatter],
   ...                            keywords = [{'focallength': 1100},
   ...                                        {'inplanescatter': 3 * u.arcmin, 'perpplanescatter': 0.3 * u.arcmin}])
 
 Next, behind the mirror, we place a `~marxs.design.rowland.GratingArrayStructure`, which is simply
 a collection of gratings. The class of the grating is defined in the parameter ``elem_class`` and
-any keyword arguments needed to initialize every individual grating are passed in ``elem_args``. In
-this case, the is the grating constand ``d``, the size of the gratings set by the ``zoom`` and the
+any keyword arguments needed to initialize every individual grating are passed in ``elem_args``.
+``d`` is the grating period, the size of the gratings set by the ``zoom`` and the
 ``order_selector`` that gives the probabilities to decide into which diffraction order a particular
-photons is diffracted. Note that ``position`` and ``orientation`` are missing from this list,
-because they will be calcualted by the `~marxs.design.rowland.GratingArrayStructure`.
+photon is diffracted. Note that ``position`` and ``orientation`` are missing from this list,
+because they will be calculated by the `~marxs.design.rowland.GratingArrayStructure`.
 
 The remaining parameters set how the `~marxs.design.rowland.GratingArrayStructure` places the
 gratings. Looking along the optical axis, it will select y and z positions for the gratings
 such that they lay in a ring, where the inner and outer radius is given by the ``radius`` parameter.
 The x-position of each grating is adjusted to make sure it touches the Rowland torus. To do so,
 we need to pass `~marxs.design.rowland.GratingArrayStructure`
 an instance of the Rowland Torus, the distance ``d_element`` between gratings (measured
 center to center - note that this is typically larger than the size of each element to account for
 the frame the gratings are mounted on), and the range along the optical axis (the x-axis of the torus)
-in which the gratings are expected to fall (the equation of the torus is solved numerically and the
-solver needs a bounded regions with a unique solution to work)::
+in which the gratings are expected to fall (the equation of the torus is solved numerically, and the
+solver needs bounded regions with a unique solution to work)::
 
-  >>> gas = rowland.GratingArrayStructure(rowland=my_torus, d_element=25, x_range=[800, 1000],
+  >>> gas = rowland.GratingArrayStructure(rowland=my_torus, d_element=[25, 25],
   ...                                     radius=[20, 100], elem_class=optics.FlatGrating,
   ...                                     elem_args={'d': 1e-5, 'zoom':[1, 10, 10],
   ...                                                'order_selector': optics.OrderSelector([-1, 0, 1])})
 
 Last, we place detectors on the inner part of the Rowland circle. This is very similar to the
 `~marxs.design.rowland.GratingArrayStructure`, except that the CCD detectors are not placed in a
-2D pattern, but just in a 1D line along the Rowland Circle. Since we do not want to fill the entire
-:math:`2 \pi` of the circle, we set a limit on ``theta``. All other parameters work the same way as above::
-  
-  >>> det = rowland.RowlandCircleArray(my_torus, theta=[np.pi - 0.8, np.pi + 0.8],
-  ...                                  d_element=10.5, elem_class=optics.FlatDetector,
-  ...                                  elem_args={'zoom': [1, 5, 5], 'pixsize': 0.01})
+2D pattern, but just in a 1D line along the Rowland Circle. All other parameters work the same way as above::
+
+  >>> det = rowland.RectangularGrid(rowland=my_torus, y_range=[-50, 50],
+  ...                               d_element=[10.5, 10.5], elem_class=optics.FlatDetector,
+  ...                               elem_args={'zoom': [1, 5, 5], 'pixsize': 0.01})
 
 Last, all the elements above as combined into a single element::
-  
+
   >>> demo = simulator.Sequence(elements=[aperture, mirror, gas, det])
 
 
 Reference / API
 ===============
 .. automodapi:: marxs.design.rowland
```

### Comparing `marxs-1.2/docs/design/tolerancing.rst` & `marxs-2.0/docs/design/tolerancing.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 **********************************
 Estimating tolerances requirements
 **********************************
 
 A common problem when designing an instrument is to estimate how much the performance degrades with increasing misalignments. Detailed alignment work costs time and money, in particular if the alignment has to be done under X-rays and in vacuum. It is much cheaper if the alignment tolerances are loose and machining a surface is precice enough.
 
-There are many different degrees of freedom to consider. Each element can be moved in space in 6 ways, rotation around all three principal axes and translation along all three principal axes. Usually, misalignment will lead to reduced performance, e.g. because a mirror covers only part of the beam or because a detector is not located at the focus position any longer. In addition to positional uncertainties, some elements have other parameters that effect the perfomance in much the same way as misalignment does. For example, for dispersion gratings the grating period could differ a little from the specificed value.
+There are different degrees of freedom to consider. Each element can be moved in space in 6 ways, rotation around all three principal axes and translation along all three principal axes. Usually, misalignment will lead to reduced performance, e.g. because a mirror covers only part of the beam or because a detector is not located at the focus position any longer. In addition to positional uncertainties, some elements have other parameters that effect the perfomance in much the same way as misalignment does. For example, for dispersion gratings the grating period could differ a little from the specificed value.
 MARXS provides tools to help with the tolerancing process. 
 
 
 Test different misalignment values and energies
 ===============================================
 
 Tolerances can be estimated "by hand" by modifying the position and orientation
@@ -28,15 +28,15 @@
     ...                      parameters, analyzefunc)
 
 We will now explain each of these parameters in more detail.
     
 Photon list and definition of the instrument
 --------------------------------------------
 
-The ``instrum`` is the instrument that will be analyzed. This will
+The ``instrum`` is the instrument that will be analysed. This will
 typically be a `marxs.simulator.Sequence`. It can contain
 the entire instrument or only part of it. ``photons_in`` is a photon
 list. If ``instrum`` contains all elements of the instrument, then
 ``photons_in`` is simply a list of photons from any
 source. Alternatively, ``photons_in`` can be processed through the
 first few elements already, and ``instrum`` only contains the
 remaining elements. For example, to determine the misalignments
@@ -46,15 +46,15 @@
 
 Wiggle functions
 ----------------
 
 This function changes the properties of one or more element in
 ``instrum``. The particular element or a list of elements is given as
 ``wiggleparts`` parameter; the ``wiggleparts`` should also be part of
-``instrum`` or the wiggled parameters won't affact the photon
+``instrum`` or the wiggled parameters won't affect the photon
 propagation. The format of the ``wigglefunc`` is a function that
 accepts an optical element (given in ``wiggleparts``) and some
 parameters (given in ``parameters``, see below). This can function
 modifies one or more elements based on the parameters. Users can write
 any ``wigglefunc`` they need. Some common examples for wiggle
 functions are part of this module:
 
@@ -87,21 +87,21 @@
 effective area and resolving power. Any function that accepts a photon
 list and returns a dictionary with resulting values will do::
 
     >>> def get_PSF_width(photons):
     ...     return {'sy': np.std(photons['dety']), 'sx': np.std(photons['detx'])} 
 
 For the analysis of instruments with dispersion gratings, MARXS
-provides `~marxs.design.tolerancing.CaptureResAeff` which can be
+provides `~marxs.design.analysis.gratings.CaptureResAeff` which can be
 initialized with some parameters such as the grating orders that
 matter. The result is an object that can be called just like a
 function::
 
     >>> import astropy.units as u
-    >>> from marxs.design.tolerancing import CaptureResAeff
+    >>> from marxs.analysis.gratings import CaptureResAeff
     >>> resaeff = CaptureResAeff(A_geom=155 * u.cm**2,
     ...                          orders=[-1, 0, 1], dispersion_coord='tdetx')
 
 
 
 
 Quick-look plotting
@@ -117,16 +117,17 @@
 unwanted columns from the table).
 
 That is why the quick-look plotting tools in this module assume that
 the data is stored in a file.
 
 .. doctest-skip::
     
-    >>> from marxs.design.tolerancing import load_and_plot
-    >>> tab, fig = load_and_plot('file.fits', ['dx', 'dy', 'dz', 'rx', 'ry', 'rz'])
+    >>> from marxs.design.tolerancing import DispersedWigglePlotter()
+    >>> plotter = DispersedWigglePlotter()
+    >>> tab, fig = plotter.load_and_plot('file.fits', ['dx', 'dy', 'dz', 'rx', 'ry', 'rz'])
 
 
 Differences for `~marxs.design.tolerancing.run_tolerances_for_energies`
 -----------------------------------------------------------------------
 
 With `~marxs.design.tolerancing.run_tolerances_for_energies`
 simulations are run for different energies. Unlike
@@ -147,15 +148,15 @@
 
     
 Suggested modelling approach
 ============================
 
 In a real instrument, there is misalignment on all degrees of freedom at the same time but. a study of the complete parameter space is usually not computationally feasible. If there are only four elements, each with six degrees of freedom (dof), and we want to simulated just 10 steps for each dof, we would need :math:`10^{4*6}` simulations. Fortunately, such a study is usually not required. Instead, MARXS provides tools to vary one (or a few) degree(s) of freedom at a time to understand how important each of them is. In practice, many dofs do not matter, because their alignment tolerances are loose. For example, if a circular mirror is rotated around its axis, the result will be the same. Another example is a detector that is larger than the image that the optics produce. If this detector is moved around a bit, it will still catch all photons.
 
-So, we suggest to run simulations for one dof at a time and decide on the maximal alignment tolerance for each dof. Then, decide on an alignment budget that assigns a tolerance to each dof. It's easy for those dof where the requirements are loose, for those where the requirements are close to what is technically feasible, this needs some judgement calls: Which element is easiest to calibrate? Which can be manufactured best? Which has the best probability of delivering tighter margins, freeing up some room in the total error budget for other elements?
+So, we suggest running simulations for one dof at a time and decide on the maximal alignment tolerance for each dof. Then, decide on an alignment budget that assigns a tolerance to each dof. It's easy for those dof where the requirements are loose, for those where the requirements are close to what is technically feasible, this needs some judgement calls: Which element is easiest to calibrate? Which can be manufactured best? Which has the best probability of delivering tighter margins, freeing up some room in the total error budget for other elements?
 
 Once this error budget has been build up, as a second step, build up an instrument model where all dof are varied at the same time with the numbers from the eror budget. Run ray-traces with several (e.g. 1000) realizations of this model and see what fraction of the ray-traces fullfills the requirements on e.g. PSF size, spectral resolving power, or effective area.
 
 
 Example: The Chandra HETG
 =========================
 
@@ -193,16 +194,16 @@
     ...     photons['probability'][photons['mirror_shell'] < 2] = 0
     ...     return photons
 
 
 Then, we import from the `marxs.design.tolerancing` module::
   
     >>> from marxs.design.tolerancing import (moveglobal, run_tolerances_for_energies,
-    ...                                       CaptureResAeff, generate_6d_wigglelist,
-    ...                                       load_and_plot)
+    ...                                       generate_6d_wigglelist)
+    >>> from marxs.analysis.gratings import CaptureResAeff
 
 Next, we generate input for the function that will move the HESS
 around in our simulation. We do seven steps for every translation
 direction (-15, -5, -1, 0, 1, 5 and 15 mm) and nine teps for every
 rotation::
   
     >>> changeglobal, changeind = generate_6d_wigglelist([0., 1., 5., 15.] * u.mm,
@@ -218,26 +219,46 @@
     ...                                   Sequence(elements=[pnt, aper, hrma, onlyMEG]),
     ...                                   Sequence(elements=[hetg, acis]),
     ...                                   moveglobal, hetg,
     ...                                   changeglobal,
     ...                                   resaeff,
     ...                                   t_source=10000)
 
-We save the results in a file named ``wiggle_global.fits`` and then make a quick-look plot. We use normal `matplotlib.pyplot` commands to modify the plot appearance slightly.
+We save the results in a file named ``wiggle_global.fits`` and then make a quick-look plot.
+ We use normal `matplotlib.pyplot` commands to modify the plot appearance slightly.
    
-.. plot:: pyplots/chandra_tolerancing.py
-   :include-source:	  
+.. plot::
+   :include-source:
+
+   from marxs.design.tolerancing import DispersedWigglePlotter
+
+   # In this example, we use a file that's included in MARXS for test purposes
+   from astropy.utils.data import get_pkg_data_filename
+   filename = get_pkg_data_filename('data/wiggle_global.fits', 'marxs.design.tests')
+
+   wiggle_plotter = DispersedWigglePlotter()
+   tab, fig = wiggle_plotter.load_and_plot(filename, ['dx', 'dy', 'dz', 'rx', 'ry', 'rz'])
+
+   fig.axes[0].legend()
+
+   for i in range(6):
+       fig.axes[2 * i].set_ylim([0, 1e3])
+       fig.axes[2 * i + 1].set_ylim([0, 70])
+
+   fig.set_size_inches(8, 6)
+   fig.subplots_adjust(left=.09, right=.93, top=.95, wspace=1.)
+
 
 Looking at the plots we see the shifting the whole HETG by a few mm in
 any direction does not change the effective area or resolving power
 significantly. The rings of photons coming from the mirror is very
 narrow, in fact much narrower than the size of the grating facets. So
 shifting the HETG a little just means that the photons hit a different
 part of the grating. A shift in x is a focus change, but as long as
-all all gratings are moved the same way, this has little
+all gratings are moved the same way, this has little
 impact. Similarly, a rotation around x just moves the position of
 the diffracted photons on the detector. As long as the rotation is
 small and the photons do not miss the detector, there is not much
 change. However, rotation around y, the dispersion direction, reduces
 the resolving power because some grating facets get
 defocussed with respect to the others. It also reduces the
 effective area because some gratings are moved out of the beam.
```

### Comparing `marxs-1.2/docs/design.rst` & `marxs-2.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/index.rst` & `marxs-2.0/docs/index.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 Multi-Architecture-Raytrace-Xraymission-Simulator (MARXS)
 =========================================================
 
 .. include:: ../DESCRIPTION.rst
 
-The documentation for MARXS is split into several parts. After intalling MARXS it first explains how to use MARXS to simulate an (astronomical) observation for an existing instrument configuration, e.g. from the examples distributed with MARX or provided by an instrument team. The following section is aimed at instrument teams and proposers.
+The documentation for MARXS is split into several parts. After installing MARXS it first
+explains how to use MARXS to simulate an (astronomical) observation for an existing
+instrument configuration, e.g. from the examples distributed with MARX or provided by
+an instrument team. The following section is aimed at instrument teams and proposers.
 
 .. note:: 
 
    MARXS has been used to simulate several instruments (e.g. ARCUS and Lynx), but is still under
    rapid develoment. We will try to mimimize API changes from now on, but will implement those
    as necessary (e.g. the astropy units system will be used on more places in the future to
    reduce unit mismatches). The :ref:`changelog` will always contain a full list of changes
```

### Comparing `marxs-1.2/docs/install.rst` & `marxs-2.0/docs/install.rst`

 * *Files 10% similar despite different names*

```diff
@@ -12,30 +12,32 @@
 - `astropy`_
 - `transforms3d <https://matthew-brett.github.io/transforms3d/>`_
 
 Numpy and astropy are best installed with a package manager such as conda. See the `astropy installation instructions for a detailed discussion <https://astropy.readthedocs.io/en/stable/install.html>`_. ``transforms3d`` is easily installed with::
 
 .. code-block:: bash
 
-    pip install transforms3d
+   $ pip install transforms3d
 
 The following Python packages are strongly recommended, but most parts of MARXS will work without them:
 
 - `scipy <http://www.numpy.org/>`_
 - matplotlib
 - `mayavi <https://docs.enthought.com/mayavi/mayavi/>`_ (for 3 D output)
+- `x3d <https://pypi.org/project/x3d/>`_
 - jsonschema
+- pyyaml
 
 Again, all but mayavi are available through common package managers such as
 conda, ``apt-get`` etc. For `mayavi
 <https://docs.enthought.com/mayavi/mayavi/>`_ see `the mayavi installation
 instructions <https://docs.enthought.com/mayavi/mayavi/installation.html#installing-with-pip>`_.
-  
+
 In addition MARXS has an interface to the `classic marx`_ C code used to simulate the Chandra mirrors (:ref:`sect-installmarxccode`).
-  
+
 Install the python code
 =======================
 
 setup.py
 --------
 
 To download the latest development version of MARXS:
@@ -50,18 +52,18 @@
 .. code-block:: bash
 
    $ python setup.py install
    $ python setup.py test
    $ python setup.py build_docs
 
 If you want to contribute to MARXS, but are not familiar with Python or
-git or Astropy yet, please have a look at the  
+git or Astropy yet, please have a look at the
 `Astropy developer documentation <http://docs.astropy.org/en/latest/#developer-documentation>`__.
 
-  
+
 .. _sect-installmarxccode:
 
 `classic marx`_ C code
 ======================
 The `classic marx`_ code is an optional dependency. By default, it is not used and all
 modules build on `classic marx`_ will be unavailable.
 
@@ -72,22 +74,22 @@
 
 The current `classic marx`_ default setup compiles static libraries, not
 shared objects. Static libraries are a tiny bit better in performance at the
 cost of extra difficulty of linking them into shared objects. Since `classic marx`_ is
 not meant to be used a library for external functions (like this python
 module), the default installation settings are tuned for performance.
 On some architectures (tested on 32-bit Ubuntu GNU/Linux) linking the static
-libraries works, on other you might see an error like this: ``relocation R_X86_64_32 against `.text' can not be used when making a shared object; recompile with -fPIC``.
+libraries works, on others you might see an error like this: ``relocation R_X86_64_32 against `.text' can not be used when making a shared object; recompile with -fPIC``.
 In that case, simply recompile and install `classic marx`_ as position independent
-code (PIC). In the `classic marx`_ source code directory:: 
+code (PIC). In the `classic marx`_ source code directory::
 
 .. code-block:: bash
 
-    make distclean
-    ./configure --prefix=/path/to/your/instalation/ CFLAGS="-O2 -g -fPIC"
-    make clean
-    make
-    make install
+   $ make distclean
+   $ ./configure --prefix=/path/to/your/instalation/ CFLAGS="-O2 -g -fPIC"
+   $ make clean
+   $ make
+   $ make install
 
 I promise that the performance difference is so small, you won't notice
 it when you run the `classic marx`_ version, but it allows the setup process of
 this python module to compile the interface to use those libraries.
```

### Comparing `marxs-1.2/docs/missions.rst` & `marxs-2.0/docs/missions.rst`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/newopticalelements.rst` & `marxs-2.0/docs/newopticalelements.rst`

 * *Files 2% similar despite different names*

```diff
@@ -51,31 +51,31 @@
 A `~marxs.optics.FlatOpticalElement` already has an `~marxs.optics.FlatOpticalElement.intersect` method implementing the default box geometry discussed in :ref:`pos4d`, so the best us is to implement a ``specific_process_photons`` method.
 
 For performance, we recommend to use vecorized implementation and change the values of the photon table in place (as opposed to making copies of parts of the table and joining them back together) whereever possible.
 
 Example for a derived class
 ===========================
 
-A simpe example for an optical element is the baffle - a rectangular opening in a large metal plate. It can be inserted into the beam and all photons that do not pass through the hole will be absorbed. In practice, the metal plate is not infinite, but has an outer bound, too, but all photons passing on the outside are either absorbed by the satellite housing ot the tube of the lab beamline and are lost from the experiment anyway and do not need to be traced any further.
+A simple example for an optical element is the baffle - a rectangular opening in a large metal plate. It can be inserted into the beam and all photons that do not pass through the hole will be absorbed. In practice, the metal plate is not infinite, but has an outer bound, too, but all photons passing on the outside are either absorbed by the satellite housing ot the tube of the lab beamline and are lost from the experiment anyway and do not need to be traced any further.
 
-.. literalinclude:: ../marxs/optics/baffle.py
+.. literalinclude:: ../marxs/optics/baffles.py
 
 The code above uses the `~marxs.optics.FlatOpticalElement.intersect` method it inherits to calculate which photons intersect at all and if so, at which coordinate. This point is entered into the ``photons['pos']``.
 
 Note that the baffle can be rectangular without writing a single line of code here. ``baf = Baffle(zoom=[1,3,2])`` would create a baffle of size 6*4 (the outer boundaries are 3 or 2 mm from the center) because the `~marxs.optics.OpticalElement` can interpret all :ref:`pos4d` keywords and the `marxs.optics.FlatOpticalElement.intersect` makes use of this information when it calculates intersection points.
 
-The baffles does not add any new descriptive columns to the output, thus the value `~marxs.base.SimulationSequenceElement.id_col` defined in a base class is not overwritten. However, the baffle does have a class dictionary `~marxs.optics.baffle.Baffle.display` that contains default parameters for plotting (see :ref:`visualization`).
+The baffle does not add any new descriptive columns to the output, thus the value `~marxs.base.SimulationSequenceElement.id_col` defined in a base class is not overwritten. However, the baffle does have a class dictionary `~marxs.optics.baffles.Baffle.display` that contains default parameters for plotting (see :ref:`visualization`).
 
 Non-physical elements
 =====================
 
 Above, we discussed elements that are physically present, such as mirrors or detectors. The simulations also allows elements that are not a piece of hardware, for example, a function that just saves a copy of the photon list to disk or prints some diagnostic information would also work::
 
   >>> def backupcopy(photons):
-  ...     photons.write('backup.fits')
+  ...     photons.write('backup.fits', overwrite=True)
   ...     return photons
   >>> photons = backupcopy(photons)
 
 Why have we chosen to return a copy of photons here, although no value in the photon list was changed? This allows us to sneak in the new function into a list of optical elements::
 
   >>> from marxs import simulator
   >>> myinstrument = simulator.Sequence(elements=[myabs1, backupcopy, myabs2])
```

### Comparing `marxs-1.2/docs/optics.rst` & `marxs-2.0/docs/optics.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 .. _sect-optics:
 
 *******************************************
 Optical elements that make up an instrument
 *******************************************
 
-A simulation is defined by creating objects for all optical elements such as mirrors and gratings and
-sorting these optical elements in the order in which a photon encounters them. Marxs works under the
-assumption that the order of elements is fixed. A photon does not have to interact with each element
-(e.g. it can miss a grating, but still be detected by another focal plane instrument), but under no circumstance will a photon ever go back
-to an element it already passed.
-
-There are ways to describe layouts where photons split between different paths, such as in the
-design of XMM-Newton where some photons pass the gratings and get reflected into the RGS detectors,
-while others continue on their path without ever encountering a grating until they hit the imaging
-detectors. Such complex setups are described in :ref:`complexgeometry`.
+A simulation is defined by creating objects for all optical elements
+such as mirrors and gratings and sorting these optical elements in the
+order in which a photon encounters them. Marxs works under the
+assumption that the order of elements is fixed. A photon does not have
+to interact with each element (e.g. it can miss a grating, but still
+be detected by another focal plane instrument), but under no
+circumstance will a photon ever go back to an element it already
+passed.
+
+There are ways to describe layouts where photons split between
+different paths, such as in the design of XMM-Newton where some
+photons pass the gratings and get reflected into the RGS detectors,
+while others continue on their path without ever encountering a
+grating until they hit the imaging detectors. Such complex setups are
+described in :ref:`complexgeometry`.
 
 
 .. _args for optical elements:
 
 Define an optical element for the simulation
 ============================================
-All optical elements have to be derived from :obj:`marxs.optics.base.OpticalElement` and they all share a common interface. 
+
+All optical elements have to be derived from
+:obj:`marxs.optics.base.OpticalElement` and they all share a common
+interface.
 
 Optical elements are generated with the following keywords:
 
 - Optical elements are placed in 3-d space with either the ``pos4d`` keyword, or the ``zoom``, ``orientation`` and ``position`` keywords as explained in :ref:`coordsys`:
 
   >>> from marxs.optics import FlatDetector
   >>> det1 = FlatDetector(position=[5., 1., 0.], zoom=[1, 50.2, 50.2], pixsize=0.1)  
@@ -41,20 +49,37 @@
   >>> det1 = FlatDetector(pixsize=0.04)
 
 
 .. _sect-optics-output:
 
 Output columns for the photon list
 ==================================
-Each MARXS run starts with a source and a pointing. The source generates the physical properties of each photon (energy, polarization) and places it in the universe (RA, dec, time). The pointing transforms position and polarization angle into vectors in spacecraft coordiantes (these vectors are called "dir" and "polarization") - see :ref:`sect-results-output`.
 
-Next, we need to assign an initial position in spacecraft coordinates to each photon. This is done by an aperture. One common approach in ray-tracing is to subdivide the entrace aperture into a regular grid and trace one ray per grid cell; alternatively, a large number of photons can be randomly distributed on the aperture. MARXS takes this second approach because (i) the result does not only depend on the position in the entrance aperture, but on a number of other parmeters (energy, polarization, time for time variable sources or pointings) and (ii) the photon list produced by the simulation closely resembles the photons lists from real observations.
-The column "pos" in the table holds the photon position as assigned on the aperture in homogeneous coordinates.
+Each MARXS run starts with a source and a pointing. The source
+generates the physical properties of each photon (energy,
+polarization) and places it in the universe (RA, dec, time). The
+pointing transforms position and polarization angle into vectors in
+spacecraft coordiantes (these vectors are called "dir" and
+"polarization") - see :ref:`sect-results-output`.
+
+Next, we need to assign an initial position in spacecraft coordinates
+to each photon. This is done by an aperture. One common approach in
+ray-tracing is to subdivide the entrace aperture into a regular grid
+and trace one ray per grid cell; alternatively, a large number of
+photons can be randomly distributed on the aperture. MARXS takes this
+second approach because (i) the result does not only depend on the
+position in the entrance aperture, but on a number of other parmeters
+(energy, polarization, time for time variable sources or pointings)
+and (ii) the photon list produced by the simulation closely resembles
+the photons lists from real observations.  The column "pos" in the
+table holds the photon position as assigned on the aperture in
+homogeneous coordinates.
 
-After passing through the aperture, the photon list will have at least the following columns:
+After passing through the aperture, the photon list will have at least
+the following columns:
 
 pos
   Position where the photon last interacted with an optical element in homogeneous coordinates.
 dir
   Direction of the phootn ray in homogeneous coordiantes.
 polarization
   Polarization vector in homogeneous coordinates (can be complex for cicularly polarized light).
@@ -101,36 +126,37 @@
 
 Last, we process the photons through both detectors::
   
   >>> photons = det1(photons)
   >>> photons = det2(photons)
   >>> photons  # doctest: +IGNORE_OUTPUT
   <Table length=5>
-  polarization [4]  energy   pos [4]     dir [4]   probability  det_x   det_y  detpix_y detpix_x  CCD_ID
-      float64      float64   float64     float64     float64   float64 float64 float64  float64  float64
-  ---------------- ------- ----------- ----------- ----------- ------- ------- -------- -------- -------
-        0.0 .. 0.0     1.0 0.0 .. -1.0 -1.0 .. 0.0         1.0     0.0     0.0      9.5      9.5     1.0
-        0.0 .. 0.0     1.0 0.0 .. -1.0 -1.0 .. 0.0         1.0     1.0     0.0      9.5     19.5     1.0
-        0.0 .. 0.0     1.0 0.0 .. -1.0 -1.0 .. 0.0         1.0    -0.5     0.0      4.5      2.0     2.0
-        0.0 .. 0.0     1.0 0.0 .. -1.0 -1.0 .. 0.0         1.0     0.5     0.0      4.5      7.0     2.0
-        0.0 .. 0.0     1.0  1.0 .. 1.0 -1.0 .. 0.0         1.0     nan     nan      nan      nan    -1.0 
+   pos [4]     dir [4]    energy polarization [4] ...  CCD_ID  det_x   det_y 
+   float64     float64   float64     float64      ... float64 float64 float64
+  ---------- ----------- ------- ---------------- ... ------- ------- -------
+  0.0 .. 1.0 -1.0 .. 0.0     1.0       0.0 .. 0.0 ...     1.0     0.0     0.0
+  0.0 .. 1.0 -1.0 .. 0.0     1.0       0.0 .. 0.0 ...     1.0     1.0     0.0
+  0.0 .. 1.0 -1.0 .. 0.0     1.0       0.0 .. 0.0 ...     2.0    -0.5     0.0
+  0.0 .. 1.0 -1.0 .. 0.0     1.0       0.0 .. 0.0 ...     2.0     0.5     0.0
+  1.0 .. 1.0 -1.0 .. 0.0     1.0       0.0 .. 0.0 ...    -1.0     nan     nan
+
 
 In this example, the two detectors are set up by hand. MARXS offers the class `marxs.simulator.Paralell` to set up elements with parallel functions, such as several CCD detectors next to each other.
 	
 List of optical elements provided by marxs
 ==========================================
 Note that elements which generate photons (astropysical sources or lab sources) are not listed here. See :ref:`sources`.
 For convenience the following elements can be imported directly from `marxs.optics` such as:
 
 
   >>> from marxs.optics import Baffle
 
 This short from is recommended over the long form:
 
-  >>> from marxs.optics.baffle import Baffle
+  >>> from marxs.optics.baffles import Baffle
 
 .. _sect-apertures:
     
 Entrance apertures
 ------------------
 
 For astrophysical sources, we assume that the rays are parallel when they reach the experiment. The direction of the photons is given by the location of the source on the sky and the pointing model, but we still need to select which of the parallel rays we select for the simulation. This is done by an optical element that we call an "aperture" in Marxs. In the case of the `~marxs.optics.MarxMirror` this fuctionality is already included in the code that describes the mirror. For designs that do not use the `~marxs.optics.MarxMirror` the following entrance apertures are included in Marxs:
```

### Comparing `marxs-1.2/docs/results.rst` & `marxs-2.0/docs/results.rst`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 
 
 Save results to disk
 ====================
 The photon list is just an `astropy.table.Table` which can be saved to many formats out-of-the-box, most importantly to fits files::
 
-  >>> photons.write('mysim_result.fits')
+  >>> photons.write('mysim_result.fits', overwrite=True)
 
 Sometimes, an instrument specification might provide a specific writing method to add more metadata and header keywords to the table before it is written.
 
 Visualize results
 =================
 The most important output of a MARXS simulation will be the photon event list with simulated detector (x, y) coordinates for each photon. This can be plotted in the same python session or in any plotting package of your choice that reads the photon event list from a file.
```

### Comparing `marxs-1.2/docs/runexample.rst` & `marxs-2.0/docs/runexample.rst`

 * *Files 10% similar despite different names*

```diff
@@ -50,16 +50,15 @@
 
    >>> pointing = chandra.LissajousDither(coords=ngc1313_X1)
 
 and also set up the instrument components. The entrace aperture was already initialized above, and the rest is easy because it is already included in MARXS (but keep in mind that the Chandra model used here includes only the geometry. It leaves out many important effects which require aceess to CALDB data, such as ACIS contamination, order probabilities for gratings etc. Use `classic marx`_ to simulate Chandra data for real.)
 ::
 
    >>> hrma = chandra.HRMA()
-   >>> acis = chandra.ACIS(chips=[4,5,6,7,8,9], aimpoint=chandra.AIMPOINTS['ACIS-S'])  # doctest: +IGNORE_OUTPUT
-   Some warnings that ACIS 1024 * pixel size does not match chip size exactly ...
+   >>> acis = chandra.ACIS(chips=[4,5,6,7,8,9], aimpoint=chandra.AIMPOINTS['ACIS-S'])
 
 That was easy!
 
 If you are simulating an instrument that is not part pf the MARXS package itself you can either specify everything yourself (see :ref:`sect-optics` for more details) or use files provided, e.g. by the instrument team. In that case, you have probably also received more detailed instructions on how to use these files.
 
 Run the simulation
 ==================
@@ -91,11 +90,47 @@
 We can now look at the distribution of photons on the detector::
 
   >>> from matplotlib import pyplot as plt
   >>> line = plt.plot(photons['tdetx'], photons['tdety'], '.')
 
 The plot clearly shows the dither pattern on the sky.
 
-.. plot:: pyplots/runexample.py
+.. plot::
+
+   import numpy as np
+   from matplotlib import pyplot as plt
+   from astropy.coordinates import SkyCoord
+   import astropy.units as u
+   from astropy.table import QTable
+
+   from marxs.source import poisson_process
+   from marxs.missions import chandra
+   from marxs.source import PointSource
+
+   ngc1313_X1 = SkyCoord("3h18m19.99s -66d29m10.97s")
+
+   energies = np.arange(.3, 8., .01) * u.keV
+   fluxdensity = 6.3e-4 * energies.value**(-1.9) / u.s / u.cm**2 / u.keV
+   fluxperbin = fluxdensity[1:] * np.diff(energies)
+   flux = poisson_process(fluxperbin.sum())
+   energytab = QTable({'energy': energies, 'fluxdensity': fluxdensity})
+
+   aperture = chandra.Aperture()
+
+   src1 = PointSource(coords=ngc1313_X1, energy=energytab,
+                      flux=flux, geomarea=aperture.area)
+
+   pointing = chandra.LissajousDither(coords=ngc1313_X1)
+   hrma = chandra.HRMA()
+   acis = chandra.ACIS(chips=[4,5,6,7,8,9], aimpoint=chandra.AIMPOINTS['ACIS-S'])
+
+   photons = src1.generate_photons(5 * u.ks)
+   photons = pointing(photons)
+   photons = aperture(photons)
+   photons = hrma(photons)
+   photons = acis(photons)
+
+   line = plt.plot(photons['tdetx'], photons['tdety'], '.')
+
 
 For more details on visualization see :ref:`visualization`.
```

### Comparing `marxs-1.2/docs/source.rst` & `marxs-2.0/docs/source.rst`

 * *Files 2% similar despite different names*

```diff
@@ -2,42 +2,53 @@
 
 .. _sources:
 
 ********************************
 Define the source in a MARXS run
 ********************************
 
-A "source" in MARXS is anything that sends out X-ray photons. This can be an astrophyical object (such as a star or an AGN, but also a dust cloud that scatters photons from some other direction into our line-of-sight) or a man-made piece of hardware, such as a X-ray tube in the lab or a radioactive calibration source in a sattelite. An important distinction in Marxs is weather the source is located at a finite distance (lab source) or so far away that all rays can be treated as parallel (astrophysical source).
+A "source" in MARXS is anything that sends out X-ray photons. This can be an
+astrophysical object (such as a star or an AGN, but also a dust cloud that
+scatters photons from some other direction into our line-of-sight) or a
+man-made piece of hardware, such as a X-ray tube in the lab or a radioactive
+calibration source in a satellite. An important distinction in Marxs is weather
+the source is located at a finite distance (lab source) or so far away that all
+rays can be treated as parallel (astrophysical source).
 
 For each type of source, we need to specifiy the following properties:
 
 - Total flux (or flux density)
 - Spectrum of photon energies
 - Polarization
 
 MARXS offers many options to specify the flux, spectrum and polarization that are designed to make common use cases very easy, while allowing for arbitrarily complex models if needed. Examples are given here, the formal specification is written in `~marxs.source.Source`.
 
 In addition, we need to give the location of the source and its size and shape (most of the currently implemented sources are point sources, but additional shapes will be added in the future):
 
-- **Astrophysical source**: Needs coordiantes on the sky and a pointing model to translate from sky coordinates to the coordiante system of the satellite. See :ref:`sect-source-radec`. 
-- **Lab source**: Needs x,y,z coordianates in the coordinate system of the experiement as explained in :ref:`pos4d`. Lab sources are described in more detail in :ref:`sect-source-lab`.
+- **Astrophysical source**: Needs coordinates on the sky and a pointing model
+  to translate from sky coordinates to the coordinate system of the satellite.
+  See :ref:`sect-source-radec`.
+- **Lab source**: Needs x, y, z coordinates in the coordinate system of the
+  experiment as explained in :ref:`pos4d`. Lab sources are described in more
+  detail in :ref:`sect-source-lab`.
 
 
  .. _sect-source-fluxenpol:
 
-Specify flux, energy and polarizarion for a source
+Specify flux, energy and polarization for a source
 ==================================================
 
-The source flux, the energy and the polarization of sources are specified in the same way for astrophysical sources and lab sources. We show a few examples here and spell out the full specification below.
+The source flux, the energy and the polarization of sources are specified in
+the same way for astrophysical sources and lab sources. We show a few examples
+here and spell out the full specification below.
 
 Flux
 ----
 The source flux can just be a number with units::
 
-     >>> from __future__ import print_function
      >>> from marxs.source import PointSource
      >>> from astropy.coordinates import SkyCoord
      >>> import astropy.units as u
      >>> star = PointSource(coords=SkyCoord("23h12m2.3s -3d4m12.3s"), flux=5. / u.s / u.cm**2)
      >>> photons = star.generate_photons(20 * u.s)
      >>> photons['time'].format='4.1f'
      >>> print(photons['time'][:6])
@@ -57,17 +68,20 @@
 
     >>> from scipy.stats import expon
     >>> def poisson_rate(exposuretime):
     ...     times = expon.rvs(scale=0.01, size=exposuretime.to(u.s).value * 0.01 * 2.)
     ...     return times[times < exposuretime] * u.s
     >>> star = PointSource(coords=SkyCoord(0, 0, unit="deg"), flux=poisson_rate)
 
-Note that this simple implementation is incomplete (it can happen by chance that it does not generate enough photons). MARXS provides a better implementation called `~marxs.source.poisson_process` which will generate the appropriate function automatically given the expected rate:
+Note that this simple implementation is incomplete (it can happen by chance
+that it does not generate enough photons). MARXS provides a better implementation
+called `~marxs.source.poisson_process` which will generate the appropriate
+function automatically given the expected rate:
 
-    >>> from marxs.source.source import poisson_process
+    >>> from marxs.source import poisson_process
     >>> star = PointSource(coords=SkyCoord("23h12m2.3s -3d4m12.3s"), flux=poisson_process(100. / u.s / u.cm**2))
 
 Energy
 ------
 Similarly to the flux, the input for ``energy`` can just be a number with a unit, which specifies the energy of a monochromatic source:
 
     >>> FeKalphaline = PointSource(coords=SkyCoord(255., -33., unit="deg"), energy=6.7 * u.keV)
@@ -80,17 +94,38 @@
        6.7
        6.7
        6.7
        6.7
 
 We can also specify a spectrum, by giving binned energy and flux density values. The energy values are taken as the *upper* egde of the bin; the first value of the flux density array is ignored since the lower bound for this bin is undefined. The format of the spectrum should be a `~astropy.table.QTable` with columns named "energy" and "fluxdensity" (photons/s/area/keV):
 
-.. plot:: pyplots/sourcespectrum.py
+.. plot::
    :include-source:
 
+   import numpy as np
+   import matplotlib.pyplot as plt
+   from astropy.table import QTable
+   import astropy.units as u
+   from marxs.source import Source
+   en = np.arange(0.5, 7., .5) * u.keV
+   fluxperbin = en.value**(-2) / u.s / u.cm**2 / u.keV
+
+   # Input as astropy QTable
+   tablespectrum = QTable([en, fluxperbin], names=['energy', 'fluxdensity'])
+   s = Source(energy=tablespectrum, name='table')
+
+   fig = plt.figure()
+
+   photons = s.generate_photons(1e3 * u.s)
+   plt.hist(photons['energy'], histtype='step', label=s.name, bins=20)
+
+   leg = plt.legend()
+   lab = plt.xlabel('Energy [keV]')
+   lab = plt.ylabel('Counts / bin')
+
 Two helpful hints:
 
 - If the input spectrum is in some type of file, e.g. fits or ascii, the `astropy.table.QTable` `read/write interface <https://astropy.readthedocs.org/en/stable/io/unified.html>`_ offers a convenient way to read it into python::
 
       >>> from astropy.table import QTable
       >>> spectrum = QTable.read('AGNspec.dat', format='ascii')  # doctest: +SKIP
       >>> agn = PointSource(coords=SkyCoord("11h11m1s -2d3m2.3s", energy=spectrum)  # doctest: +SKIP
@@ -100,15 +135,15 @@
     >>> flux = (spectrum['fluxdensity'][1:] * np.diff(spectrum['energy'])).sum()   # doctest: +SKIP
     >>> agn = PointSource(coords=SkyCoord("11h11m1s -2d3m2.3s", energy=spectrum,
     ...         flux=flux)  # doctest: +SKIP
       
     
 Lastly, "energy" can be a function that assigns energy values based on the timing of each photon. This allows for time dependent spectra. As an example, we show a function where the photon energy is 0.5 keV for times smaller than 5 s and 2 keV for larger times.
   
-    >>> from marxs.source.source import Source
+    >>> from marxs.source import Source
     >>> import numpy as np
     >>> def time_dependent_energy(t):
     ...     t = t.value  # convert quantity to plain numpy array
     ...     en = np.ones_like(t)
     ...     en[t <= 5.] = 0.5
     ...     en[t > 5.] = 2.
     ...     return en * u.keV
@@ -127,24 +162,26 @@
      6.0    2.0
 
 Polarization
 ------------
 An unpolarized source can be created with ``polarization=None`` (this is also
 the default). In this case, a random polarization is assigned to every
 photon. The other options are very similar to "energy": Allowed are a constant
-angle or a table with columns "angle" and "probabilitydensity". Here is an example where most polarizations are randomly oriented, but an orientation around :math:`35^{\circ}` (0.6 in radian) is a lot more likely.
+angle or a table with columns "angle" and "probabilitydensity". Here is an example
+where most polarizations are randomly oriented, but an orientation around
+:math:`35^{\circ}` (0.6 in radian) is a lot more likely.
 
     >>> angles = np.array([0., 30., 40., 360]) * u.degree
     >>> prob = np.array([1, 1., 8., 1.]) / u.degree
     >>> polsource = PointSource(coords=SkyCoord(11., -5.123, unit='deg'), polarization=QTable({'angle': angles, 'probabilitydensity': prob}))
 
 Lastly, if polarization is a function, it will be called with time and energy
 as parameters allowing for time and energy dependent polarization
 distributions. The following function returns a 50% polarization fraction in
-the 6.4 keV Fe flourescence line after some polarized feature comes into view at t=1000 s.
+the 6.4 keV Fe florescence line after some polarized feature comes into view at t=1000 s.
 
     >>> def polfunc(time, energy):
     ...     pol = np.random.uniform(high=2*np.pi, size=len(time))
     ...     ind = (time > 1000. * u.s) & (energy > 6.3 * u.keV) & (energy < 6.5 * u.keV)
     ...     # set half of all photons with these conditions to a specific polarization angle
     ...     pol[ind & (np.random.rand(len(time))> 0.5)] = 1.234
     ...     return pol * u.rad
@@ -155,15 +192,15 @@
 
 Specify the sky position of an astrophysical source
 ===================================================
 
 An astrophysical source in marxs must be followed by a pointing model as first optical element that translates the sky coordiantes into the coordinate system of the satellite (see :ref:`pos4d`) and an entrace aperture that selects an initial position for each ray (all rays from astrophysical sources are parallel, thus the position of the source on the sky only determines the direction of a photon but not if it hits the left or the right side of a mirror). See :ref:`sect-apertures` for more details.
 
 
-The following astropysical sources are included in marxs:
+The following astrophysical sources are included in marxs:
 
 - `marxs.source.PointSource`
 - `marxs.source.RadialDistributionSource`
 - `marxs.source.GaussSource`
 - `marxs.source.DiskSource`
 - `marxs.source.SphericalDiskSource` 
 - `marxs.source.SymbolFSource`
@@ -179,21 +216,20 @@
 ===========================================
 
 Sources in the lab are specified in the same coordinate system used for all other optical elements, see :ref:`pos4d` for details.
 
 The following laboratory sources are provided:
 
 - `~marxs.source.FarLabPointSource`
-- `~marxs.source.LabPointSource`
 - `~marxs.source.LabPointSourceCone`
 
 Design your own sources and pointing models
 ===========================================
 
-The base class for all marxs sources is `~marxs.source.Source`. The only method required for a source is ``generate_photons``. We recommend to look at the implementation of the included sources to see how this is done best.
+The base class for all marxs sources is `~marxs.sources.Source`. The only method required for a source is ``generate_photons``. We recommend to look at the implementation of the included sources to see how this is done best.
 
 - `marxs.source.Source`
 
 
 Reference/API
 =============
```

### Comparing `marxs-1.2/docs/support.rst` & `marxs-2.0/docs/support.rst`

 * *Files identical despite different names*

### Comparing `marxs-1.2/docs/visualization.rst` & `marxs-2.0/docs/visualization.rst`

 * *Files 26% similar despite different names*

```diff
@@ -13,157 +13,263 @@
 =======================
 Specifically when designing an instrument, we might want a 3-D rendering of the mirrors, detectors, and gratings as well as the photon path. We want to see where photons are absorbed and where they are scattered.
 
 Depending on the target audience of the visualization (e.g. a detailed technical rendering for a publication, or a 3D display in a webpage) different output formats are required. `marxs.visualization` supports different backends for display and rendering with different display options. Not every backend supports every option and we welcome code contributions to improve the plotting.
 
 Currently, the following plotting packages are supported: 
 
-- `Mayavi <http://docs.enthought.com/mayavi/mayavi/>`__ is a python package for interactive 3-D displays that uses VTK underneath. Using plotting routines from `marxs.visualization.mayavi` scenes can be displayed right in the same Python session or `jupyter notebook <http://docs.enthought.com/mayavi/mayavi/tips.html#using-mayavi-in-jupyter-notebooks>`_ where the MARXS simulation is running or be exported as static images (e.g. PNG) or as X3D suitable for inclusion in a web page or `AAS journal paper <http://adsabs.harvard.edu/abs/2016ApJ...818..115V>`_.
+- `X3D <https://www.web3d.org/x3d/what-x3d>`__ is an open XML-based standard to 3D models in the web-browser and can be displayed with different libraries. Importantly, it can also be rendered directly in a Jupyter notebook.
+- `Mayavi <http://docs.enthought.com/mayavi/mayavi/>`__ is a Python package for interactive 3-D displays that uses VTK underneath. Using plotting routines from `marxs.visualization.mayavi` scenes can be displayed right in the same Python session or `jupyter notebook <http://docs.enthought.com/mayavi/mayavi/tips.html#using-mayavi-in-jupyter-notebooks>`_ where the MARXS simulation is running or be exported as static images (e.g. PNG) or as X3D suitable for inclusion in a web page or `AAS journal paper <http://adsabs.harvard.edu/abs/2016ApJ...818..115V>`_.
 - `three.js <https://threejs.org/>`__ is a javascript package to render 3d content in a web-browser using WebGL technology. MARXS does not display this content directly, but outputs code (`marxs.visualization.threejs`) or json formatted data (`marxs.visualization.threejsjson`) that can be included in a web page.
 
-All backends support a function called ``plot_object`` which plots objects in the simulation such as apertures, mirrors, or detectors and a function called ``plot_rays`` which shows the path the photons have taken through the instrument in any specific simulation. In the example below, we use the `~marxs.visualization.mayavi` backend to explain these functions. The arguments for these functions are very similar for all backends, but some differences are unavoidable. For example, `marxs.visualization.mayavi.plot_rays` needs a reference to the scene where the rays will be added, while `marxs.visualization.threejs.plot_rays` requires a file handle where relevant javascript commands can be written - see :ref:`sect-vis-api` for a more details.
+All backends support a function called ``plot_object`` which plots objects in the simulation such as apertures, mirrors, or detectors and a function called ``plot_rays`` which shows the path the photons have taken through the instrument in any specific simulation. In the example below, we use the `~marxs.visualization.mayavi` backend to explain these functions. The arguments for these functions are very similar for all backends, but some differences are unavoidable. For example, `marxs.visualization.mayavi.plot_rays` needs a reference to the scene where the rays will be added, while `marxs.visualization.threejs.plot_rays` requires a file handle where relevant javascript commands can be written - see :ref:`sect-vis-api` for more details.
 
-First, we need to set up mirrors, gratings and detectors (here gratings on a Rowland torus). The entrace aperture is just a thin ring, like the effective area of a single shell in a Wolter type-I telescope::
+First, we need to set up mirrors, gratings and detectors (here gratings on a Rowland torus). The entrance aperture is just a thin ring, like the effective area of a single shell in a Wolter type-I telescope::
 
-  >>> from marxs import optics, design, analysis
-  >>> from marxs.design import rowland
-  >>> import astropy.units as u
-  >>> rowland = design.rowland.RowlandTorus(5000, 5000)
-  >>> aper = optics.CircleAperture(position=[12000, 0, 0],
-  ...                              zoom=[1, 1000, 1000],
-  ...                              r_inner=960)
-  >>> mirr = optics.FlatStack(position=[11000, 0, 0], zoom=[20, 1000, 1000],
-  ...                         elements=[optics.PerfectLens,
-  ...                         optics.RadialMirrorScatter],
-  ...                         keywords = [{'focallength': 11000},
-  ...                                     {'inplanescatter': 4 * u.arcsec,
-  ...                                      'perpplanescatter': 0.6 * u.arcsec}])
+    >>> from marxs import optics, design, analysis
+    >>> from marxs.design import rowland
+    >>> import astropy.units as u
+    >>> rowland = design.rowland.RowlandTorus(5000, 5000)
+    >>> aper = optics.CircleAperture(position=[12000, 0, 0],
+    ...                              zoom=[1, 1000, 1000],
+    ...                              r_inner=960)
+    >>> mirr = optics.FlatStack(position=[11000, 0, 0],
+    ...                         zoom=[20, 1000, 1000],
+    ...                         elements=[optics.PerfectLens,
+    ...                         optics.RadialMirrorScatter],
+    ...                         keywords = [{'focallength': 11000},
+    ...                                     {'inplanescatter': 4 * u.arcsec,
+    ...                                      'perpplanescatter': 0.6 * u.arcsec}])
 
 In our figure, we want to color the diffraction gratings and the photons that pass through them. For this purpose we make a new class of grating that inherits from `~marxs.optics.FlatGrating` but additionally assigns a value to the ``colorid``. The method ``specific_process_photons` is defined as part of `~marxs.optics.FlatOpticalElement` and it returns a dictionary of arrays that are assigned to the corresponding column in the ``photons`` table. Here, we simply add another column to that::
 
-  >>> class ColoredFlatGrating(optics.FlatGrating):
-  ...     '''Flat grating that also assigns a color to all passing photons.'''
-  ...     def specific_process_photons(self, *args, **kwargs):
-  ...         out = super(ColoredFlatGrating, self).specific_process_photons(*args, **kwargs)
-  ...         out['colorid'] = self.colorid if hasattr(self, 'colorid') else np.nan
-  ...         return out
+    >>> class ColoredFlatGrating(optics.FlatGrating):
+    ...     '''Flat grating that also assigns a color to all passing photons.'''
+    ...     def specific_process_photons(self, *args, **kwargs):
+    ...         out = super(ColoredFlatGrating, self).specific_process_photons(*args, **kwargs)
+    ...         out['colorid'] = self.colorid if hasattr(self, 'colorid') else np.nan
+    ...         return out
 
 We place a set of transmission gratings below the mirror and add CCDs on the Rowland torus::
 
-  >>> gas = design.rowland.GratingArrayStructure(rowland=rowland, d_element=180,
-  ...                                            x_range=[8000, 10000],
-  ...                                            radius=[870, 910],
-  ...                                            elem_class=ColoredFlatGrating,
-  ...                                            elem_args={'d': 2e-4, 'zoom': [1, 80, 80],
-  ...                                                       'order_selector': optics.OrderSelector([-1, 0, 1])})
-  >>> det_kwargs = {'d_element': 105, 'elem_class': optics.FlatDetector,
-  ...               'elem_args': {'zoom': [1, 50, 20], 'pixsize': 0.01}}
-  >>> det = design.rowland.RowlandCircleArray(rowland, theta=[3.1, 3.2], **det_kwargs)
-  >>> projectfp = analysis.ProjectOntoPlane()
+    >>> gas = design.rowland.GratingArrayStructure(rowland=rowland, d_element=[180, 180],
+    ...                                            radius=[870, 910],
+    ...                                            elem_class=ColoredFlatGrating,
+    ...                                            elem_args={'d': 2e-4, 'zoom': [1, 80, 80],
+    ...                                                       'order_selector': optics.OrderSelector([-1, 0, 1])})
+    >>> det_kwargs = {'d_element': [105, 50], 'elem_class': optics.FlatDetector,
+    ...               'elem_args': {'zoom': [1, 50, 20], 'pixsize': 0.01}}
+    >>> det = design.rowland.RectangularGrid(rowland=rowland, y_range=[-200, 200], **det_kwargs)
+    >>> projectfp = analysis.ProjectOntoPlane()
 
 Each optical element in MARXS has some default values to customize its looks in its ``display`` property, which may or may not be used by the individual backend since not every backend supports the same display settings.
 The most common settings are ``display['color']`` (which can be any RGB tuple or any color valid in `matplotlib <http://matplotlib.org>`_) and ``display['opacity']`` (a number between 0 and 1).
 Usually, ``display`` is a class dictionary, so any change on any one object will affect all elements of that class::
 
   >>> mirr.display['opacity'] = 0.5
   >>> optics.FlatDetector.display['color'] = 'orange'
    
 To change just one particular element we copy the class dictionary to that element and set the color. In this example, we calculate the angle that each grating has from the y-axis. We split that in three regions and color the gratings accordingly::
 
-  >>> import copy
-  >>> import numpy as np
-  >>> gratingcolors = 'bgr'
-  >>> for e in gas.elements:
-  ...     e.display = copy.deepcopy(e.display)
-  ...     e.ang = (np.arctan(e.pos4d[1,3] / e.pos4d[2, 3]) + np.pi/2) % (np.pi)
-  ...     e.colorid = int(e.ang / np.pi * 3)
-  ...     e.display['color'] = gratingcolors[e.colorid]
+    >>> import copy
+    >>> import numpy as np
+    >>> gratingcolors = 'bgr'
+    >>> for e in gas.elements:
+    ...     e.display = copy.deepcopy(e.display)
+    ...     e.ang = (np.arctan(e.pos4d[1,3] / e.pos4d[2, 3]) + np.pi/2) % (np.pi)
+    ...     e.colorid = int(e.ang / np.pi * 3)
+    ...     e.display['color'] = gratingcolors[e.colorid]
 
   
 .. _sect-vis-example:
 
 Using MARXS to visualize sub-aperturing
 =======================================
-In this example, we use MARXS to explain how sub-aperturing works. Continuing the code from above, we define an instrument setup, run a simulation, and plot results both in 2d and in 3d. This is a fully functional ray-trace simulation; the only unrealsitic point is the grating constant of the diffraction gratings which is about an order of magnitude smaller than current gratings.
+In this example, we use MARXS to explain how sub-aperturing works. Continuing the code from above, we define an instrument setup, run a simulation, and plot results both in 2d and in 3d. This is a fully functional ray-trace simulation; the only unrealistic point is the grating constant of the diffraction gratings which is about an order of magnitude smaller than current gratings.
 
 
 2d plot
 -------
 
 We want to know how photons that go through a particular set of gratings are distributed compared to the total point-spread function (PSF). Therefore, we assign a color to every sector of gratings and in our plots, we color gratings in this sector and photons that passed through it accordingly.
 
-.. plot:: pyplots/vis_subaperturing.py
+.. plot::
 
-On the plot, we see that photons from each sector (e.g. the sector that colors photons red) form a strip on the detector. Only adding up photons from all sectors gives us a round PSF. Subaperturing is the idea to disperse only photons from one sector, such that the PSF in cross-dispersion direction is large, but the dispersion in cross-dispersion direction is much smaller (the green sector in the figure). Thus, the spectral resolution of the dispersed spectrum will be higher than for a spectrograph that uses the full PSF. Note that the first order photons are asymetrically distributed unlike the zeroth order. This is due to the finite sizes of the flat diffraction gratings that deviate from the curved Rowland torus. Based on this simulation, we can now decide to implement sub-aperturing in our instrument. We will instruct the engineers to mount ggratings only at the green colored positions so that we get a sharper line (a better resolving power) compared with using every photon that passes through the mirror.
+   import copy
+   import numpy as np
+   import matplotlib.pyplot as plt
+   from marxs import optics, design, analysis, source, simulator
+   from astropy.coordinates import SkyCoord
+   import astropy.units as u
+
+   rowland = design.rowland.RowlandTorus(5000, 5000)
+   aper = optics.CircleAperture(position=[12000, 0, 0],
+                                zoom=[1, 1000, 1000],
+                                r_inner=960)
+   mirr = optics.FlatStack(position=[11000, 0, 0], zoom=[20, 1000, 1000],
+                           elements=[optics.PerfectLens,
+                                     optics.RadialMirrorScatter],
+                           keywords = [{'focallength': 11000},
+                                       {'inplanescatter': 4 * u.arcsec,
+                                        'perpplanescatter': 0.6 * u.arcsec}])
+   mirr.display['opacity'] = 0.5
+
+   class ColoredFlatGrating(optics.FlatGrating):
+       '''Flat grating that also assigns a color to all passing photons.'''
+       def specific_process_photons(self, *args, **kwargs):
+           out = super(ColoredFlatGrating, self).specific_process_photons(*args, **kwargs)
+           out['colorid'] = self.colorid if hasattr(self, 'colorid') else np.nan
+           return out
+
+   gas = design.rowland.GratingArrayStructure(rowland=rowland, d_element=[180, 180],
+                                              radius=[870, 910],
+                                              elem_class=ColoredFlatGrating,
+                                              elem_args={'d': 2e-4, 'zoom': [1, 80, 80],
+                                                         'order_selector': optics.OrderSelector([-1, 0, 1])})
+   det_kwargs = {'d_element': [105, 105], 'elem_class': optics.FlatDetector,
+                 'elem_args': {'zoom': [1, 50, 20], 'pixsize': 0.01}}
+   det = design.rowland.RectangularGrid(rowland=rowland, y_range=[-120, +120], **det_kwargs)
+   projectfp = analysis.ProjectOntoPlane()
+
+   gratingcolors = 'bgr'
+   for e in gas.elements:
+       e.display = copy.deepcopy(e.display)
+       e.ang = (np.arctan(e.pos4d[1,3] / e.pos4d[2, 3]) + np.pi/2) % (np.pi)
+       e.colorid = int(e.ang / np.pi * 3)
+       e.display['color'] = gratingcolors[e.colorid]
+
+   instrum = simulator.Sequence(elements=[aper, mirr, gas, det, projectfp])
+   star = source.PointSource(coords=SkyCoord(30., 30., unit='deg'),
+                             energy=1. * u.keV, flux=1. / u.s / u.cm**2)
+   pointing = source.FixedPointing(coords=SkyCoord(30., 30., unit='deg'))
+
+   photons = star.generate_photons(4000 * u.s)
+   photons = pointing(photons)
+   photons = instrum(photons)
+   ind = (photons['probability'] > 0) & (photons['facet'] >=0)
+
+   fig = plt.figure()
+   ax0 = fig.add_subplot(221, aspect='equal')
+   ax1 = fig.add_subplot(222, aspect='equal', sharey=ax0)
+   ax0h = fig.add_subplot(223, sharex=ax0)
+   ax1h = fig.add_subplot(224, sharex=ax1, sharey=ax0h)
+
+   ind0 = photons['order'] == 0
+   # It is arbitrary which direction if called +1 or -1 order
+   ind1 = np.abs(photons['order']) == 1
+   out = ax0h.hist(photons['proj_x'][ind & ind0], range=[-1, 1], bins=20,
+                   lw=0, color='0.8')
+   out = ax1h.hist(photons['proj_x'][ind & ind1], range=[61, 63], bins=20,
+                   lw=0, color='0.8')
+
+   for i in [0, 2, 1]:  # make green plotted on top
+       c = gratingcolors[i]
+       indcolor = photons['colorid'] == i
+       ax0.plot(photons['proj_x'][ind & ind0 & indcolor],
+                photons['proj_y'][ind & ind0 & indcolor],
+                '.', color=c)
+       ax1.plot(photons['proj_x'][ind & ind1 & indcolor],
+                photons['proj_y'][ind & ind1 & indcolor],
+                '.', color=c)
+       out = ax0h.hist(photons['proj_x'][ind & ind0 & indcolor],
+                       range=[-1, 1], bins=20,
+                       histtype='step', color=c, lw=2)
+       out = ax1h.hist(photons['proj_x'][ind & ind1 & indcolor],
+                       range=[61, 63], bins=20,
+                       histtype='step', color=c, lw=2)
+
+   ax0.set_xlim([-.5,0.5])
+   ax1.set_xlim([61.65, 62.4])
+   ax0h.set_xlim([-.5,0.5])
+   ax1h.set_xlim([61.65, 62.4])
+
+   ax0.text(0.1, 0.9, '0th order', transform=ax0.transAxes)
+   ax1.text(0.1, 0.9, '1st order', transform=ax1.transAxes)
+   ax0h.set_xlabel('dispersion direction [mm]')
+   ax0.set_ylabel('cross-dispersion [mm]')
+   ax0.tick_params(axis='x', labelbottom='off')
+   ax1.tick_params(axis='both', labelleft='off', labelbottom='off')
+   ax1h.tick_params(axis='y', labelleft='off')
+   ax0h.set_ylabel('photons / bin')
+
+   for ax in [ax0, ax1, ax0h, ax1h]:
+       ax.xaxis.set_major_locator(plt.MaxNLocator(4))
+       ax.yaxis.set_major_locator(plt.MaxNLocator(4))
+
+   fig.subplots_adjust(hspace=0, wspace=0, left=.18, right=.96, top=.97, bottom=.1)
+
+
+On the plot, we see that photons from each sector (e.g. the sector that colors photons red) form a strip on the detector. Only adding up photons from all sectors gives us a round PSF. Subaperturing is the idea to disperse only photons from one sector, such that the PSF in cross-dispersion direction is large, but the dispersion in cross-dispersion direction is much smaller (the green sector in the figure). Thus, the spectral resolution of the dispersed spectrum will be higher than for a spectrograph that uses the full PSF. Note that the first order photons are asymmetrically distributed unlike the zeroth order. This is due to the finite sizes of the flat diffraction gratings that deviate from the curved Rowland torus. Based on this simulation, we can now decide to implement sub-aperturing in our instrument. We will instruct the engineers to mount ggratings only at the green colored positions so that we get a sharper line (a better resolving power) compared with using every photon that passes through the mirror.
 
 3d output
 ---------
 
 Next, we want to show how the instrument that we use above looks in the 3d.
 Very similar to the previous example, we combine mirror, detector, and grating into `~marxs.simulator.Sequence`. We also define a `marxs.simulator.KeepCol` object, which we pass into our `~marxs.simulator.Sequence`. When we call the `~marxs.simulator.Sequence`, the `~marxs.simulator.KeepCol` object will make a copy of a column (here the "pos" column) and store that.
 Another change compared to the 2d plotting is that we generate a lot fewer photons because the lines indicating the photon paths can make the gratings hard to see in 3d if there are too many of them::
   
-  >>> import numpy as np
-  >>> from astropy.coordinates import SkyCoord
-  >>> import astropy.units as u
-  >>> from marxs import source, simulator
-  >>> # object to save intermediate photons positions after every step of the simulaion
-  >>> pos = simulator.KeepCol('pos')
-  >>> instrum = simulator.Sequence(elements=[aper, mirr, gas, det, projectfp], postprocess_steps=[pos])
-  >>> star = source.PointSource(coords=SkyCoord(30., 30., unit='deg'))
-  >>> pointing = source.FixedPointing(coords=SkyCoord(30., 30., unit='deg'))
-  >>> photons = star.generate_photons(100 * u.s)
-  >>> photons = pointing(photons)
-  >>> photons = instrum(photons)
-  >>> ind = (photons['probability'] > 0) & (photons['facet'] >=0)
-  >>> posdat = pos.format_positions()[ind, :, :]
+    >>> import numpy as np
+    >>> from astropy.coordinates import SkyCoord
+    >>> import astropy.units as u
+    >>> from marxs import source, simulator
+    >>> # object to save intermediate photons positions after every step of the simulation
+    >>> pos = simulator.KeepCol('pos')
+    >>> instrum = simulator.Sequence(elements=[aper, mirr, gas, det, projectfp], postprocess_steps=[pos])
+    >>> star = source.PointSource(coords=SkyCoord(30., 30., unit='deg'))
+    >>> pointing = source.FixedPointing(coords=SkyCoord(30., 30., unit='deg'))
+    >>> photons = star.generate_photons(100 * u.s)
+    >>> photons = pointing(photons)
+    >>> photons = instrum(photons)
+    >>> ind = (photons['probability'] > 0) & (photons['facet'] >=0)
+    >>> posdat = pos.format_positions()[ind, :, :]
 
 First, plot the objects that make up the instrument (aperture, mirror, gratings, detectors)::
 
 .. doctest-requires:: mayavi
 
-  >>> from mayavi import mlab
-  >>> from marxs.visualization.mayavi import plot_object, plot_rays
-  >>> fig = mlab.figure(bgcolor=(1,1,1))
-  >>> obj = plot_object(instrum, viewer=fig)
+    >>> from mayavi import mlab
+    >>> from marxs.visualization.mayavi import plot_object, plot_rays
+    >>> fig = mlab.figure(bgcolor=(1,1,1))
+    >>> obj = plot_object(instrum, viewer=fig)
 
-Now, we plot the rays using their colorid and a global color map that matches the blue-red values that we assinged to the gratings already::
+Now, we plot the rays using their colorid and a global color map that matches the blue-red values that we assigned to the gratings already::
   
 .. doctest-requires:: mayavi
 
-  >>> rays = plot_rays(posdat, scalar=photons['colorid'][ind],
-  ...                  kwargssurface={'opacity': .5,
-  ...                                 'line_width': 1,
-  ...                                  'colormap': 'blue-red'})
+    >>> rays = plot_rays(posdat, scalar=photons['colorid'][ind],
+    ...                  kwargssurface={'opacity': .5,
+    ...                                 'line_width': 1,
+    ...                                  'colormap': 'blue-red'})
 
 MARXS can also display non-physical objects. The following code will add a fraction of the Rowland torus::
 
 .. doctest-requires:: mayavi
   
-  >>> rowland.display['coo2'] = np.linspace(-.2, .2, 60)
-  >>> obj = plot_object(rowland, viewer=fig)
+    >>> rowland.display['coo2'] = np.linspace(-.2, .2, 60)
+    >>> obj = plot_object(rowland, viewer=fig)
 
 .. raw:: html
 
   <div class="figure" align="center">
   <x3d width='500px' height='400px'> 
   <scene>
   <inline url="_static/subaperturing.x3d"> </inline> 
   </scene> 
   </x3d>
   <p class="caption" style="clear:both;"><span class="caption-text">
-  3D view of the instrument set up. Lines are photon paths. All detectors are orange and the gratings are red, green, and blue, depending on their position. The mirror and the aperture are shown with their default representation (white box and transparent green plate with the aperture hole). Part of the Rowland torus is shown as a red surface. Use your mouse to rotate, pan and zoom. <a href="https://www.x3dom.org/documentation/interaction/">(Detailed instructions for camera navigation).</a> </span></p>
+  3D view of the instrument set up. Lines are photon paths. All detectors are orange, and the gratings are red, green, and blue, depending on their position. The mirror and the aperture are shown with their default representation (white box and transparent green plate with the aperture hole). Part of the Rowland torus is shown as a red surface. Use your mouse to rotate, pan and zoom. <a href="https://www.x3dom.org/documentation/interaction/">(Detailed instructions for camera navigation).</a> </span></p>
   </div>
         
 .. _sect-vis-api:
 
 Reference/API
 =============
 
 .. automodapi:: marxs.visualization
+.. automodapi:: marxs.visualization.x3d
 .. automodapi:: marxs.visualization.mayavi
    :skip: format_doc
 .. automodapi:: marxs.visualization.threejs
    :skip: format_doc
 .. automodapi:: marxs.visualization.threejsjson
    :skip: format_doc
 .. automodapi:: marxs.visualization.utils
```

### Comparing `marxs-1.2/licenses/LICENSE.rst` & `marxs-2.0/licenses/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/analysis/analysis.py` & `marxs-2.0/marxs/analysis/analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Licensed under GPL version 3 - see LICENSE.rst
-from __future__ import division
-
 import numpy as np
 import scipy.optimize
 from astropy.stats import sigma_clipped_stats
 
 from ..optics import FlatDetector
 
+
 def sigma_clipped_std(photons, colname='det_x', **kwargs):
     '''Return stddev of sigma-clipped data.
 
     Parameters
     ----------
     photons : `astropy.table.Table`
         Input photon list.
@@ -74,23 +73,23 @@
     def width(x, photons):
         mdet = FlatDetector(position=np.dot(orientation, np.array([x, 0, 0])),
                             orientation=orientation,
                             zoom=1e5, pixsize=1.)
         p = mdet(photons.copy())
         return objective_func(p, **objective_func_args)
 
-    return scipy.optimize.minimize_scalar(width, args=(photons,), options={'maxiter': 20, 'disp': False},
-                                   **kwargs)
+    return scipy.optimize.minimize_scalar(width, args=(photons,),
+                                          **kwargs)
 
 
 def detected_fraction(photons, labels, col='order'):
     '''Calculate the fraction of photons detected for some integer label
 
-    While written for calculating Aeff per order, this can be used with any discrete
-    quantity, e.g. Aeff per CCD.
+    While written for calculating Aeff per order, this can be used
+    with any discrete quantity, e.g. Aeff per CCD.
 
     Parameters
     ----------
     photons : `astropy.table.Table`
         Photon event list
     labels : np.array
         Numeric (integer) labels that are found in column ``col``. When, e.g.,
@@ -99,15 +98,14 @@
     col : string
         Column name for the order column.
 
     Returns
     -------
     prop : np.array
         Probability for a photon in a specific order to be detected.
+
     '''
     prob = np.zeros_like(labels, dtype=float)
     for i, o in enumerate(labels):
         ind = (photons[col] == o)
-        if filterfunc is not None:
-            ind = ind & filterfunc(photons)
         prob[i] = np.sum(photons['probability'][ind]) / len(photons)
     return prob
```

### Comparing `marxs-1.2/marxs/analysis/gratings.py` & `marxs-2.0/marxs/optics/grating.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,258 +1,301 @@
 # Licensed under GPL version 3 - see LICENSE.rst
-from __future__ import division
-
+'''Gratings and efficiency files'''
+import math
 import numpy as np
-from astropy.stats import sigma_clipped_stats
 
-from ..optics import FlatDetector, CircularDetector, OrderSelector
-from ..design import RowlandTorus
-from . import (find_best_detector_position)
-from .analysis import sigma_clipped_std
-from ..math.geometry import Cylinder
-
-
-class AnalysisError(Exception):
-    pass
-
-def resolvingpower_per_order(gratings, photons, orders, detector=None,
-                             colname='det_x'):
-    '''Calculate the resolving power in every grating order.
-
-    As input this function takes a Grating Array Structure (``gratings``) and
-    a list of photons ready to hit the grating, i.e. the photons have already
-    passed through aperture and mirror in e.g. a Chandra-like design. The
-    function will take the same input photons and send them through the gas
-    looping over the grating orders. In each step of the loop all photons are
-    send to the same order, thus the statistical uncertainty on the measured
-    spectral resolving power (calculated as ``pos_x / FWHM_x``) is the same
-    for every order and is set by the number of photons in the input list.
-
-    As a side effect, the function that selects the grating orders for
-    diffraction in ``gas`` will be changed. Pass a deep copy of the GAS if
-    this could affect consecutive computations.
-
-    Unlike `~marxs.analysis.gratings.resolvingpower_from_photonlist` this
-    function ray-traces the input photon list from the gratings to the
-    detectors.
+from ..math.utils import norm_vector
+from ..math.polarization import parallel_transport
+from .. import energy2wave
+from .base import FlatOpticalElement
+
+
+class OrderSelector(object):
+    '''Select from a list of order numbers independent of energy.
 
     Parameters
     ----------
-    gratings : `marxs.simulator.Parallel`
-        Structure that holds individual grating elements,
-        e.g. `marxs.design.GratingArrayStructure`
-    photons : `astropy.table.Table`
-        Photon list to be processed for every order
-    orders : np.array of type int
-        Order numbers
-    detector : marxs optical element or `marxs.design.RowlandTorus` or ``None``.
-        Photons are projected onto a detector. There are three ways to define
-        this detector:
-
-        - Pass in an instance of an optical element (e.g. a
-          `marxs.optics.FlatDetector`).
-        - Pass in a `marxs.design.RowlandTorus`. This function will generate
-          a detector that follows the Rowland circle.
-        - ``None``. A flat detector in the yz plane is used, but the x position
-          for this detector is numerically optimized in each step.
-
-    colname : string
-        Name of the column that labels the dispersion direction. This is only
-        used if a detector instance is passed in explicitly.
-
-    Returns
-    -------
-    res : np.array
-        Resolution defined as FWHM / position for each order.
-    fwhm : np.array
-        FWHM for each order
-    info : dict
-        Dictionary with more information, e.g. fit results
+    orderlist : array
+        This are the order numbers to chose from. They must be integers.
+    p : None or array
+        Probability for a photon to end up in each order. The sum of
+        all probabilities can be smaller than 1, if a certain fraction
+        of photons is absorbed by the grating. If this is ``None``,
+        equal probability is assigned to all orders.
+
+    Examples
+    --------
+    Two common use cases for testing are a grating where every photon gets
+    diffracted into the same order or where all photons get distributed with
+    equal probability into a set of orders.
+
+    >>> import numpy as np
+    >>> from marxs.optics import FlatGrating, OrderSelector
+    >>> singleordergrating = FlatGrating(d=1e-4, order_selector=OrderSelector([3]))
+    >>> setofordersgrating = FlatGrating(d=1e-4, order_selector=OrderSelector(np.arange(-3, 4)))
+
     '''
-    res = np.zeros_like(orders, dtype=float)
-    fwhm = np.zeros_like(orders, dtype=float)
-    info = {}
-
-    if detector is None:
-        info['method'] = 'Detector position numerically optimized'
-        info['fit_results'] = []
-        col = 'det_x' # 0 at center, detpix_x is 0 in corner.
-        zeropos = 0.
-    elif isinstance(detector, RowlandTorus):
-        det = CircularDetector(geometry=Cylinder.from_rowland(detector, width=1e5,
-                                                              rotation=np.pi,
-                                                              kwargs={'phi_lim':[-np.pi/2, np.pi/2]}))
-        info['method'] = 'Circular detector on Rowland circle'
-        col = 'detpix_x'
-        # Find position of order 0.
-        # if Rowland torus is tilted, might not be at phi=0.
-        pg = photons.copy()
-        pg = det(pg)
-        # Remove photons that miss a mirror etc.
-        pg = pg[pg['probability'] > 0.]
-        zeropos, temp1, temp2 = sigma_clipped_stats(pg[col])
-    else:
-        det = detector
-        info['method'] = 'User defined detector'
-        col = colname
-        # Find position of order 0.
-        pg = photons.copy()
-        pg = det(pg)
-        zeropos, temp1, temp2 = sigma_clipped_stats(pg[col])
-
-    for i, order in enumerate(orders):
-        gratingeff = OrderSelector([order])
-        gratings.elem_args['order_selector'] = gratingeff
-        for elem in gratings.elements:
-            elem.order_selector = gratingeff
-
-        pg = photons.copy()
-        pg = gratings(pg)
-        # Remove photons that slip between the gratings
-        pg = pg[(pg['order'] == order) & (pg['probability'] > 0.)]
-        if detector is None:
-            xbest = find_best_detector_position(pg, objective_func=sigma_clipped_std)
-            info['fit_results'].append(xbest)
-            det = FlatDetector(position=np.array([xbest.x, 0, 0]), zoom=1e5)
-        pg = det(pg)
-        meanpos, medianpos, stdpos = sigma_clipped_stats(pg[col])
-        fwhm[i] = 2.3548 * stdpos
-        res[i] = np.abs((meanpos - zeropos) / fwhm[i])
-    return res, fwhm, info
-
-
-def weighted_per_order(data, orders, energy, gratingeff):
-    '''Summarize a per-order table of a quantity such as spectral resolution.
-
-    `marxs.analysis.fwhm_per_order` produces a set of data for each grating
-    order, most notably the spectral resolution achieved in every spectral
-    order for every energy. In practice, however, most orders see only a very
-    small number of photons and will not contribute significantly to the
-    observed signal.
-
-    This method provides one way to summarize the data by calculating the
-    weighted mean of the resolution for each energy, weighted by the
-    probability of photons for be diffracted into that order ( = the expected
-    fraction).
+    def __init__(self, orderlist, p=None):
+        self.orderlist = orderlist
+        if p is None:
+            self.p = np.ones(len(orderlist)) / len(orderlist)
+        else:
+            p = np.asanyarray(p)
+            if len(p) != len(orderlist):
+                raise ValueError('Number of elements in orderlist and probabilities does not match.')
+            if p.sum() > 1.:
+                raise ValueError('Sum of all probabilities must be <= 1.')
+            if np.any(p < 0):
+                raise ValueError('Probabilities cannot be negative')
+            self.p = p
+
+    def __call__(self, energy, *args):
+        p_sum = self.p.sum()
+        p = self.p / p_sum
+        if np.isscalar(energy):
+            return np.random.choice(self.orderlist, p=p), self.p.sum()
+        else:
+            return np.random.choice(self.orderlist, size=len(energy), p=p), p_sum * np.ones_like(energy)
+
+
+class EfficiencyFile(object):
+    '''Select grating order from a probability distribution in a data file.
+
+    The file format supported by this class is as follows: The first
+    colum contains energy values in keV, all remaining columns have
+    the probability that a photons with this energy is diffracted into
+    the respective order. The probabilities for each order do not have
+    to add up to 1.
 
     Parameters
     ----------
-    data : (N, M) np.array
-        Array with data for N orders and M energies, e.g. spectral resolution
-    orders : np.array of length N of type int
-        Order numbers
-    energy : np.array for length M of type float
-        Energies for each entry in resolution
-    gratingeff : `marxs.optics.gratings.EfficiencyFile`
-        Object that holds the probability that a photon on a certain energy is
-        diffracted to a specific order.
-
-    Returns
-    -------
-    weighted_res : np.array of length M
-        Weighted resolution for each energy
+    filename : string
+        Path to the efficiency file.
+    orders : list
+        List of orders in the file. Must match the number of columns with
+        probabilities.
+
     '''
-    if len(orders) != data.shape[0]:
-        raise ValueError('First dimension of "data" must match length of "orders".')
-    if len(energy) != data.shape[1]:
-        raise ValueError('Second dimension of "data" must match length of "energy".')
-
-    weights = np.zeros_like(data)
-    for i, o in enumerate(orders):
-        ind_o = (gratingeff.orders == o).nonzero()[0]
-        if len(ind_o) != 1:
-            raise KeyError('No data for order {0} in gratingeff'.format(o))
-        en_sort = np.argsort(gratingeff.energy)
-        weights[i, :] = np.interp(energy, gratingeff.energy[en_sort],
-                                  gratingeff.prob[:, ind_o[0]][en_sort])
-
-    return np.ma.average(data, axis=0, weights=weights)
-
-
-def resolvingpower_from_photonlist(photons, orders,
-                                   col='proj_x', zeropos=None,
-                                   ordercol='order'):
-    '''Calculate the resolving power for several grating orders
-
-    If fewer than 20 photons are detected in a single order, this function
-    returns nan values.
-
-    Unlike `~marxs.analysis.gratings.resolvingpower_per_order` this method does
-    not run any ray-trace simulations. It just extracts information from a
-    photon list that is passed in.
+    def __init__(self, filename, orders):
+        dat = np.loadtxt(filename)
+        self.energy = dat[:, 0]
+        if len(orders) != (dat.shape[1] - 1):
+            raise ValueError('orders has len={0}, but data files has {1} order columns.'.format(len(orders), dat.shape[1] - 1))
+        self.orders = np.array(orders)
+        self.prob = dat[:, 1:]
+        # Probability to end up in any order
+        self.totalprob = np.sum(self.prob, axis=1)
+        # Cumulative probability for orders, normalized to 1.
+        self.cumprob = np.cumsum(self.prob, axis=1) / self.totalprob[:, None]
+
+    def __call__(self, energies, *args):
+        orderind = np.empty(len(energies), dtype=int)
+        ind = np.empty(len(energies), dtype=int)
+        for i, e in enumerate(energies):
+            ind[i] = np.argmin(np.abs(self.energy - e))
+            orderind[i] = np.min(np.nonzero(self.cumprob[ind[i]] > np.random.rand()))
+        return self.orders[orderind], self.totalprob[ind]
+
+
+class FlatGrating(FlatOpticalElement):
+    '''Flat grating
+
+    The grating is assumed to be geometrically thin, i.e. all photons enter on
+    the face of the grating, not through the sides.
 
     Parameters
     ----------
-    photons : `astropy.table.Table`
-        Photon event list
-    orders : np.array
-        Orders for which the resolving power will be calculated
-    col : string
-        Column name for the column holding the dispersion coordinate.
-    zeropos : float or ``None``
-        Value of column `col` where the zeroth order is found. If not given,
-        this is calculated (assuming the zeroth order photons are part of the
-        event list).
-    ordercol : string
-        Name of column that lists grating order for each photon
-
-    Returns
-    -------
-    res : np.array
-        resolving power for each order
-    pos : np.array
-        mean value of ``col`` for each order
-    std : np.array
-        standard deviation of the distribution of ``col`` for each order
+    d : float or callable
+        grating constant in mm. If ``d`` is callable, then it will be
+        called as ``d(intercoos)``, where ``intercoos`` is a (N, 2)
+        array holding the positions where photons hit the gratings in
+        the local coordinate system.  This can be used to simulate
+        manufacturing uncertainties or intentional grating period
+        variation. The callable has to return a vector of lengths N
+        that contains the grating constant for each photon in mm.
+
+    order_selector : callable
+        A function or callable object that accepts arrays of photon
+        energy, polarization and the blaze angle as input and returns
+        arrays for grating order (integer) and probability
+        (float). The probabiliy expresses the chance that the photon
+        passes the grating and is not absorbed, e.g. if the
+        probability that a photon at energy E ends up in order=[-2,
+        -1, 0, 1, 2] is [0, 0, .5, .3, .0] , then the returned
+        probability for all photons should be 0.8.
+
+    transmission : bool
+        Set to ``True`` for a transmission grating and to ``False`` for a
+        reflection grating. (*Default*: ``True`` ) **Warning: Reflection
+        gratings have not yet been tested**
+
+    groove_angle : float
+        Angle between the local z axis and the direction of the
+        grooves in radian.  (*Default*: ``0.``)
     '''
-    if zeropos is None:
-        ind = (photons[ordercol] == 0)
-        if ind.sum() < 20:
-            raise AnalysisError('Too few photons in list to determine position of order 0 automatically.')
-        zeropos, medzeropos, stdzero = sigma_clipped_stats(photons[col][ind])
-
-    pos = np.zeros_like(orders, dtype=float)
-    std = np.zeros_like(orders, dtype=float)
-
-    for i, o in enumerate(orders):
-        ind = (photons[ordercol] == o)
-        if ind.sum() > 20:
-            meanpos, medianpos, stdpos = sigma_clipped_stats(photons[col][ind])
-        else:
-            meanpos, stdpos = np.nan, np.nan
-        pos[i] = meanpos
-        std[i] = stdpos
-    res = np.abs(pos - zeropos) / (std * 2.3548)
-    return res, pos, std
 
+    loc_coos_name = ['grat_y', 'grat_z']
+    '''name for output columns that contain the interaction point in local coordinates.'''
 
-def effectivearea_from_photonlist(photons, orders, n_photons, A_geom=1.,
-                                   ordercol='order'):
-    '''Calculate the effective area several grating orders
-
-    This is based on the probabilities of the photons in the list, so
-    this photons list must already account for all instrument
-    components, for example, do not forgot to set the probability to 0
-    for photons that falls into a chip gap.
+    order_name = 'order'
+    '''Column name for diffraction order.'''
 
-    Parameters
-    ----------
-    photons : `astropy.table.Table`
-        Photon event list
-    orders : np.array
-        Orders for which the resolving power will be calculated
-    n_photons : int
-        Number of photons originally simulated
-    A_geom : number
-        Geometric area of aperture that was used for photon list.
-    ordercol : string
-        Name of column that lists grating order for each photon
-
-    Returns
-    -------
-    aeff : np.array
-        effective area for each order
+    blaze_name = 'blaze'
+    '''Column name for blaze angle.'''
+
+    def order_sign_convention(self, p, e_perp_groove):
+        '''Set sign convention for grating orders.
+
+        This sets the following, somewhat arbitrary convention:
+        Positive grating orders will are displaced along the local
+        :math:`\hat e_z` vector, negative orders in the opposite
+        direction. If the grating is rotated by :math:`-\pi` the
+        physical situation is the same, but the sign of the grating
+        order will be reversed.  In this sense, the convention chosen
+        is arbitrarily. However, it has some practical advantages: The
+        implementation is fast and all photons passing through the
+        grating in the same diffraction order are displaced in the
+        same way. (Contrary to the convention in :class:`CATGrating`.)
+        ``order_sign_convention`` has to be a callable that accepts an
+        array of eukledian direction vectors as input and returns
+        ``+1``, ``-1``, or an array filled with ``-1`` or ``+1``.
+
+        Parameters
+        ----------
+        p : np.array
+            Array of Eucleadian direction vectors
+        e_perp_groove : np.array
+            Array of local groove directions at the positions where the photons
+            hit
+        '''
+        # -1 because n, l, d should be right-handed coordinate system
+        # while n = e_x, l = e_x, and d = e_y would be left-handed.
+        return -1
+
+    def __init__(self, **kwargs):
+        self.order_selector = kwargs.pop('order_selector')
+        self.transmission = kwargs.pop('transmission', True)
+        if 'd' not in kwargs:
+            raise ValueError('Input parameter "d" (Grating constant) is required.')
+        self._d = kwargs.pop('d')
+        groove_angle = kwargs.pop('groove_angle', 0.)
+
+        super().__init__(**kwargs)
+
+        self.geometry._geometry['groove_angle'] = groove_angle
+
+    def e_groove_coos(self, intercoos):
+        '''Get coordiante orthonormal coordinate system along groove direction.
+
+        Parameters
+        ----------
+         intercoos : `numpy.ndarray` of shape (N, 2)
+            coordinates in the coordiante system of the geometry (e.g. (x, y), or
+            (r, phi)).
+
+        Returns
+        -------
+        e_groove, e_perp_groove, n : `numpy.ndarray` of shape (N, 4)
+            Vectors pointing along the groove direction (parallel to the surface),
+            perpendicular to the groove direction (parallel to surface),
+            and normal to surface.
+        '''
+
+        groove = self.geometry['groove_angle']
+        ex, ey, en = self.geometry.get_local_euklid_bases(intercoos)
+        e_groove = math.sin(-groove) * ex + math.cos(-groove) * ey
+        e_perp_groove = math.cos(-groove) * ex - math.sin(-groove) * ey
+        return e_groove, e_perp_groove, en
+
+    def d(self, intercoos):
+        '''Method that returns the grating constant at given positions.
+
+        For a grating with constant grating constant, this will just return the
+        number input as ``d`` when the element was initialized. For gratings
+        where the grating constant varies with position on the facet, this
+        calculates the appropriate number for every position.
+        '''
+        if not callable(self._d):
+            return self._d
+        else:
+            return self._d(intercoos)
+
+    def blaze_angle_modifier(self, intercoos):
+        '''Modify blaze angle
+
+        In `diffract_photons` the blaze angle is calculated relative
+        to the surface of the grating. In cases where that number has
+        to be modified (e.g. when the grating bars are not
+        perpendicular to the surface) the blaze angle can be modified
+        by overriding this function.
+        '''
+        return np.zeros(intercoos.shape[0])
+
+    def diffract_photons(self, photons, intersect, interpos, intercoos):
+        '''Vectorized implementation'''
+        p = norm_vector(photons['dir'].data[intersect])
+        l, d, n = self.e_groove_coos(intercoos[intersect])
+        # Minus sign here because we want n, l, d to be a right-handed coordinate system
+        d = - d
+
+        wave = energy2wave / photons['energy'].data[intersect]
+        # calculate angle between normal and (ray projected in plane perpendicular to groove)
+        # -> this is the blaze angle
+        p_perp_to_grooves = norm_vector(p - np.einsum("ij,ij->i", p, l)[:, None] * l)
+        # Use abs here so that blaze angle is always in 0..pi/2
+        # independent of the relative orientation of p and n.
+        # Also, clip because rounding errors can lead to products slightly larger than 1
+        blazeangle = np.arccos(np.clip(np.abs(np.einsum("ij,ij->i", p_perp_to_grooves,
+                                                n)), 0, 1))
+        blazeangle += self.blaze_angle_modifier(intercoos[intersect, :])
+        m, prob = self.order_selector(photons['energy'].data[intersect],
+                                      photons['polarization'].data[intersect],
+                                      blazeangle)
+
+        # The idea to calculate the components in the (d,l,n) system separately
+        # is taken from MARX
+        sign = self.order_sign_convention(p, d)
+        p_d = np.einsum("ij,ij->i", p, d) + sign * m * wave / self.d(intercoos[intersect, :])
+        p_l = np.einsum("ij,ij->i", p, l)
+        # The norm for p_n can be derived, but the direction needs to be chosen.
+        p_n = np.sqrt(1. - p_d**2 - p_l**2)
+        # Check if the photons have same direction compared to normal before
+        direction = np.sign(np.einsum("ij,ij->i", p, n), dtype=float)
+        if not self.transmission:
+            direction *= -1
+        dir = p_d[:, None] * d + p_l[:, None] * l + (direction * p_n)[:, None] * n
+        return dir, m, prob, blazeangle
+
+    def specific_process_photons(self, photons,
+                                 intersect, interpos, intercoos):
+
+        dir, m, p, blaze = self.diffract_photons(photons, intersect, interpos,
+                                                 intercoos)
+        pol = parallel_transport(photons['dir'].data[intersect, :], dir,
+                                 photons['polarization'].data[intersect, :])
+        out = {'dir': dir, 'probability': p, 'polarization': pol,
+               self.order_name: m, self.blaze_name: blaze}
+        return out
+
+
+class CATGrating(FlatGrating):
+    '''Critical-Angle-Transmission Grating
+
+    CAT gratings are a special case of :class:`FlatGrating` and accept
+    the same arguments.
+
+    They differ from a :class:`FlatGrating` in the sign convention of
+    the grating orders: Blazing happens on the side of the negative
+    orders. Obviously, this convention is only meaningful if the
+    photons do not arrive perpendicular to the grating.
     '''
-    aeff = np.zeros(len(orders))
-    for i, o in enumerate(orders):
-        aeff[i] = photons['probability'][photons[ordercol] == o].sum()
-    return aeff / n_photons * A_geom
+    def order_sign_convention(self, p, e_perp_groove):
+        '''Convention to chose the sign for CAT grating orders
+
+        Blazing happens on the side of the negative orders. Obviously, this
+        convention is only meaningful if the photons do not arrive
+        perpendicular to the grating.
+        '''
+        dotproduct = np.einsum("ij,ij->i", p, e_perp_groove)
+        sign = np.sign(dotproduct)
+        sign[sign == 0] = 1
+        return sign
```

### Comparing `marxs-1.2/marxs/analysis/tests/test_analysis.py` & `marxs-2.0/marxs/analysis/tests/test_analysis.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/base/base.py` & `marxs-2.0/marxs/base/base.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,37 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 from collections import OrderedDict
 import inspect
-import warnings
 from copy import deepcopy
+import re
+from datetime import datetime
 
 import numpy as np
 from transforms3d import affines
 from astropy.table import Column
 
 from ..visualization.utils import DisplayDict
+from marxs import __version__
+
+__all__ = ['GeometryError',
+           'DocMeta',
+           'MarxsElement',
+           'TagVersion',
+           'check_meta_consistent',
+           'check_energy_consistent',
+           'SimulationSequenceElement',
+           ]
+
 
 class GeometryError(Exception):
     pass
 
 
 class DocMeta(type):
-    '''Metaclass to inherit docstrings when reqired.
+    '''Metaclass to inherit docstrings when required.
 
     When a derived class overwrites a method that was already defined in its
     base class, the new method usually has the same purpose as the original
     method and often uses the same parameters, too, although the implementation
     differs slightly.  In this case, it should have the same docstring, too.
     This metaclass will look for methods that are undocumented and add the
     docstring of the appropriate parent method to them.
@@ -51,17 +63,17 @@
 
         return type.__new__(mcs, name, bases, dict)
 
 
 class MarxsElement(metaclass=DocMeta):
     '''Base class for all elements in a MARXS simulation.
 
-    This includes elements that actually change photon properties such as grating and
-    mirrors, but also abstract concepts that do not have a direct hardware
-    representation such as a "Rowland Torus".
+    This includes elements that actually change photon properties such
+    as grating and mirrors, but also abstract concepts that do not
+    have a direct hardware representation such as a "Rowland Torus".
     '''
 
     display = {'shape': 'None'}
     'Dictionary for display specifications, e.g. color'
 
     def __init__(self, **kwargs):
         '''Define a new MARXS element.'''
@@ -73,27 +85,132 @@
         if len(kwargs) > 0:
             raise ValueError('Initialization arguments {0} not understood'.format(', '.join(kwargs.keys())))
         self.display = DisplayDict(self, deepcopy(self.display))
 
     def describe(self):
         return OrderedDict(element=self.name)
 
+
+reexp = re.compile(r"(?P<version>[\d.dev]+[\d]+)[+]?(g(?P<gittag>\w+))?[.]?(d(?P<dirtydate>[\d]+))?")
+'''Regex to parse scm version string'''
+
+ver = reexp.match(__version__)
+'''Parsed version of the marxs code'''
+
+
+class TagVersion(MarxsElement):
+    '''Tag a photons list with diagnostic information such as a the program version.
+
+    All keyword arguments passed when this element is initialized or when it is called
+    will be added to the meta information of the photon list, some additional
+    information on program version and runtime is added automatically.
+    As such, the format of the keyword values is very flexible. However, if they are
+    going to be written to fits files it is useful to follow fits conventions and
+    the default paraemter values also invoke fits conventions.
+
+
+    Parameters
+    ----------
+    origin : tuple of strings
+        according to fits convention, the Institution where file was created
+    creator : string or tuple of strings
+        according to fits convention, the Person or program creating file'
+    '''
+    def __init__(self,
+                 ORIGIN=('unkwown', 'Institution where file was created'),
+                 CREATOR=('MARXS', 'Person or program creating file'),
+                 **kwargs):
+        super().__init__(name=kwargs.pop('name', self.__class__))
+
+        kwargs['MARXSVER'] = (ver.group('version'), 'MARXS code version')
+        if not ver.group('gittag') is None:
+            kwargs['MARXSGIT'] = (ver.group('gittag'),
+                                        'Git hash of MARXS code')
+        if not ver.group('dirtydate') is None:
+            kwargs['MARXSTIM'] = (ver.group('dirtydate'),
+                                        'Date of dirty version ARCUS code')
+        self.tags = kwargs
+
+    def __call__(self, photons, *args, **kwargs):
+        photons.meta['DATE'] = (datetime.now().isoformat()[:10], 'Date/time of computation')
+        for k, v in self.tags.items():
+            photons.meta[k] = v
+        for k, v in kwargs.items():
+            photons.meta[k] = v
+        return photons
+
+
+def check_meta_consistent(meta1, meta2, keywords=['ORIGIN', 'CREATOR',
+                                                  'MARXSVER', 'MARXSGIT', 'MARXSTIM',
+                                                  ],
+                          allow_missing=True):
+    '''Check that the meta data between two simulations indicates consistency.
+
+    This check compares a number of keywords (e.g. the version of marxs) to
+    indicate if the simulations where run with the same version of marxs.
+    If a simulation records more information in the metadata,
+    the check can be more complete.
+    This function raises an `AssertionError` if the two sets of
+    meta information are different.
+
+    Parameters
+    ----------
+    meta1 : dict
+        header from photon list 1
+    meta2 : dict
+        header from photon list 2
+    keywords : list
+        Keywords to be checked
+    allow_missing : bool
+        This flag allows a keyword to be missing from both dictionaries
+        (e.g. MARXSGIT is not set if run with a released version); however,
+        it is still an error if a key is present only in one, but not the
+        dictionary.
+
+    Raises
+    ------
+    AssertionError, KeyError
+    '''
+    for k in keywords:
+        if (k in meta1) and (k in meta2):
+            assert meta1[k] == meta2[k]
+        else:
+            if not allow_missing:
+                raise KeyError(f'{k} not found in both dicts.')
+            # Even with allow_missing=True
+            # it's an error to have a key in only one dict
+            if (k in meta1) or (k in meta2):
+                raise KeyError(f'{k} found in one, but not both dicts.')
+
+
+def check_energy_consistent(photons):
+    '''Check if the energy is the same for all photons.
+
+    If there is no energy colum, then this also passes.
+    '''
+    if 'energy' in photons.colnames:
+        assert np.allclose(photons['energy'], photons['energy'][0])
+
+
 class SimulationSequenceElement(MarxsElement):
-    '''Base class for all elements in a simulation sequence that processes photons.'''
+    '''Base class for all elements in a simulation that processes photons.'''
 
     output_columns = []
     '''This is a list of strings that names the output properties.
 
-    This gives the names of the output properties from this optical element.
-    `process_photon` or `process_photons` are responsible for calculating the values of these
-    properties. For example, for a mirror of nested shells one might set
-    ``output_columns = ['mirror_shell']`` to pass the information on which shell the interaction
-    took place to the user.
+    This gives the names of the output properties from this optical
+    element.  `process_photon` or `process_photons` are responsible
+    for calculating the values of these properties. For example, for a
+    mirror of nested shells one might set
+    ``output_columns = ['mirror_shell']``
+    to pass the information on which shell the interaction took place to the
+    user.
 
-    The following properties are always included in the output and do not need to be listed here:
+    The following properties are always included in the output and do not need
+    to be listed here:
 
         dir : `numpy.ndarray`
             4-d direction vector of ray in homogeneous coordinates
         pos : `numpy.ndarray`
             4-d position of last interaction pf the photons with any optical
             element in homogeneous coordinates. Together with ``dir`` this
             determines the equation of the ray.
@@ -101,14 +218,15 @@
             Photon energy in keV.
         polarization : float
             Polarization angle of the photons.
         probability : float
             Probability that the photon continues. Set to 0 if the photon is
             absorbed, to 1 if it passes the optical element and to number
             between 0 and 1 to express a probability that the photons passes.
+
     '''
 
     id_col = None
     '''String that names an id column for output.
 
     Set this to a string to add an automatic numbering to the output. This is
     especially useful if there are several identical optical components that
@@ -122,72 +240,85 @@
     '''
 
     def __init__(self, **kwargs):
         self.id_num = kwargs.pop('id_num', -9)
         # We want to use id_col as a class attribute, but overwrite it if given as a kwarg
         if 'id_col' in kwargs:
             self.id_col = kwargs.pop('id_col')
-        super(SimulationSequenceElement, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def add_output_cols(self, photons, colnames=[]):
-        '''Add output columns of the correct format (currently: float) to the photon array.
+        '''Add output columns to the photon array.
 
         This function takes the column names that are added to ``photons`` from
         several sources:
 
         - `id_col` (if not ``None``)
         - `output_columns`
         - the ``colnames`` parameter.
 
         Parameters
         ----------
         photons : `astropy.table.Table`
             Table columns are added to.
-        colnames : list of strings
+        colnames : list of elements
+            Each element can be a string (in this case a float column with
+            initial value ``np.nan`` is added) or a dictionay of arguments
+            for `astropy.table.column.Column`. If the dictionay has a keys
+            "value" then the column will be initialized to that value.
             Column names to be added; in addition several object properties can
             be used to set the column names, see description above.
         '''
-        temp = np.empty(len(photons))
-        temp[:] = np.nan
         for n in self.output_columns + colnames:
-            if n not in photons.colnames:
-                photons.add_column(Column(name=n, data=temp))
-
-        if self.id_col is not None:
-            if self.id_col not in photons.colnames:
-                photons.add_column(Column(name=self.id_col, data=-np.ones(len(photons))))
+            if (n is not None) and (n not in photons.colnames):
+                if not isinstance(n, dict):
+                    n = {'name': n, 'value': np.nan}
+                val = n.pop('value', None)
+                newcol = Column(length=len(photons), **n)
+                if val is not None:
+                    newcol[:] = val
+                photons.add_column(newcol)
+
+        # We can call this recursively, because the column will be added
+        # before reaching this line agian, so we avoid infinite recursion.
+        if (self.id_col is not None) and (self.id_col not in photons.colnames):
+            self.add_output_cols(photons, colnames=[{'name': self.id_col,
+                                                     'dtype': int,
+                                                     'value': -1}])
 
     def __call__(self, photons, *args, **kwargs):
         return self.process_photons(photons, *args, **kwargs)
 
 
 def _parse_position_keywords(kwargs):
     '''Parse keywords to define position.
 
     If ``pos4d`` is given, use that, otherwise look for ``position``, ``zoom``
     and ``orientation``.
 
     Parameters
     ----------
     pos4d : 4x4 array
-        Transformation to bring an element from the default position (see description of
-        individual elements) to a certain point in the space of homogeneous coordinates.
+        Transformation to bring an element from the default position
+        (see description of individual elements) to a certain point in
+        the space of homogeneous coordinates.
     position : 3-d vector in real space
         Measured from the origin of the spacecraft coordinate system.
     orientation : Rotation matrix or ``None``
         Relative orientation of the base vectors of this optical
         element relative to the orientation of the coordinate system
         of the spacecraft. The default is no rotation (i.e. the axes of both
         coordinate systems are parallel).
     zoom : float or 3-d vector
-        Scale the size of an optical element in each dimension by ``zoom``. If ``zoom`` is a scalar,
-        the same scale is applied in all dimesions. This only affects the oter dimensions of
-        the optical element, not internal scales like the pixel size or grating constant (if
-        defined for the optical element in question).
-    '''
+        Scale the size of an optical element in each dimension by
+        ``zoom``. If ``zoom`` is a scalar, the same scale is applied
+        in all dimesions. This only affects the oter dimensions of the
+        optical element, not internal scales like the pixel size or
+        grating constant (if defined for the optical element in
+        question).  '''
     pos4d = kwargs.pop('pos4d', None)
     if pos4d is None:
         position = kwargs.pop('position', np.zeros(3))
         orientation = kwargs.pop('orientation', np.eye(3))
         zoom = kwargs.pop('zoom', 1.)
         if np.isscalar(zoom):
             zoom = np.ones(3) * zoom
```

### Comparing `marxs-1.2/marxs/design/rowland.py` & `marxs-2.0/marxs/design/rowland.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,44 +2,45 @@
 '''Tools for setting up instruments in the Rowland Torus geometry.
 
 This includes an object that represents the Rowland torus itself (imaginatively
 called `~marxs.design.rowland.RowlandTorus`), some helper functions used to set
 the right parameters for the torus and a few classes that are derived from
 `marxs.simulator.ParallelCalculated`, each placing elements such as gratings
 or detectors on the Rowland torus. There are many ways to do that, e.g. the
-limits can be defined in x,y,z coordiantes or in theta, phi coordinates on the
+limits can be defined in x,y,z coordinates or in theta, phi coordinates on the
 torus, gratings can be ordered in concentric circles or pack densely in a
-rectoangular area etc. At this point, the different classes do not exploit all
+rectangular area etc. At this point, the different classes do not exploit all
 these possibilities, they merely give a few of many possible ways to set up an
 instrument.
 
 These classes may be generalized in the future.
 '''
-
-from __future__ import division
-
 import numpy as np
 from scipy import optimize
 import transforms3d
-from transforms3d.utils import normalized_vector
 
 from ..optics.base import OpticalElement
 from ..base import MarxsElement
 from ..optics import FlatDetector
-from ..math.rotations import ex2vec_fix
 from ..math.utils import e2h, h2e, anglediff
 from ..simulator import ParallelCalculated
 from ..math.geometry import Geometry
 
-__all__ = ['find_radius_of_photon_shell', 'design_tilted_torus',
+__all__ = ['find_radius_of_photon_shell',
+           'design_tilted_torus',
+           'double_rowland_from_channel_distance',
+           'add_offset_double_rowland_channels',
            'RowlandTorus',
-           'ElementPlacementError', 'GratingArrayStructure', 'LinearCCDArray',
-           'RectangularGrid', 'RowlandCircleArray']
+           'ElementsOnTorus',
+           'GratingArrayStructure',
+           'RectangularGrid', 'CircularMeshGrid',
+           ]
 
-def find_radius_of_photon_shell(photons, mirror_shell, x, percentile=[1,99]):
+
+def find_radius_of_photon_shell(photons, mirror_shell, x, percentile=[1, 99]):
     '''Find the radius the photons coming from a single mirror shell have.
 
     For nested Wolter Type I mirrors the ray of photons reflected from a single
     mirror shell essentially form a cone in space. The tip of the cone is at
     the focal point and the base is at the mirror. There is a certain thickness
     to this cone depending on where exactly on the mirror the individual photon
     was reflected.
@@ -58,30 +59,30 @@
         ``photons`` for filtering).
     x : float
         Distance along the optical axis (assumed to coincide with the x axis
         with focal point at 0).
     percentile : list of floats
         The radius is calculated at the given percentiles. ``50`` would give
         the median radius. The default of ``[1, 99]`` gives a radius range
-        excluding extrem outliers such as stray rays scattered into the extreme
+        excluding extreme outliers such as stray rays scattered into the extreme
         wing of the PSF.
 
     '''
     p = photons.copy()
     mdet = FlatDetector(position=np.array([x, 0, 0]), zoom=1e8, pixsize=1.)
     p = mdet(p)
     ind = (p['probability'] > 0) & (p['mirror_shell'] == mirror_shell)
     r = np.sqrt(p['det_x'][ind]**2+p['det_y'][ind]**2.)
     return np.percentile(r, percentile)
 
 
 class RowlandTorus(MarxsElement, Geometry):
     '''Torus with y axis as symmetry axis.
 
-    Note that the origin of the torus is the focal point, which is
+    Note that the origin of the torus is the focal point, which
     **may or may not** be the same as the center of the torus.
 
     Parameters
     ----------
     R : float
         Radius of Rowland torus. ``r`` determines the radius of the Rowland
         circle, ``R`` is then used to rotate that circle around the axis of
@@ -107,87 +108,83 @@
         '''Quartic torus equation.
 
         Roots of this equation are points on the torus.
 
         Parameters
         ----------
         xyz : np.array of shape (N, 3) or (3)
-            Coordinates of points in euklidean space. The quartic is calculated
+            Coordinates of points in euclidean space. The quartic is calculated
             for those points.
         transform : bool
             If ``True`` transform ``xyz`` from the global coordinate system
             into the local coordinate system of the torus. If this
             transformation is done in the calling function already, set to
         ``False``.
 
         Returns
         -------
         q : np.array of shape (N) or scalar
             Quartic at the input location
         '''
         if xyz.shape[-1] != 3:
-            raise ValueError('Input coordinates must be defined in Eukledian space.')
+            raise ValueError('Input coordinates must be defined in Euclidean space.')
 
         if transform:
             invpos4d = np.linalg.inv(self.pos4d)
             xyz = h2e(np.einsum('...ij,...j', invpos4d, e2h(xyz, 1)))
         return ((xyz**2).sum(axis=-1) + self.R**2. - self.r**2.)**2. - 4. * self.R**2. * (xyz[..., [0,2]]**2).sum(axis=-1)
 
-    def solve_quartic(self, x=None, y=None, z=None, interval=[0, 1], transform=True):
-        '''Solve the quartic on the Rowland torus in Cartesian coordinates.
+    def solve_quartic(self, origin, v, transform=True):
+        '''Solve the quartic on the Rowland torus.
 
         This method solves the quartic equation for positions on the Rowland
-        Torus for cases where two of the Cartesian coordinates are fixed
-        (e.g. y and z) and the third one (e.g. x) needs to be computed. This
-        function is intended as a convenience for a common use case. In more
-        general cases, evaluate the :meth:`RowlandTorus.quartic` and search for
-        the roots of that function.
+        Torus, i.e. it intersects a line with the torus. To that end, the
+        location on the line is varied and the root of the quartic is found
+        through numerical optimization.
 
         Parameters
         ----------
-        x, y, z : float or None
-            Set two of these coordinates to fixed numbers. This method will
-            solve for the coordinate set to ``None``.
-            x, y, z are defined in the global coordinate system.
-        interval : np.array
-            [min, max] for the search. The quartic can have up to four
-            solutions because a line can intersect a torus in four points and
-            this interval must bracket one and only one solution.
+        origin : np.array
+            Origin of line as homogeneous coordinate.
+            This is also used as approximate starting point for the numerical
+            optimization, so it should be reasonably close to the
+            solution.
+        v : np.array
+            Direction of the line as homogeneous coordinate.
         transform : bool
-            If ``True`` transform ``xyz`` from the global coordinate system
+            If ``True`` transform input from the global coordinate system
             into the local coordinate system of the torus. If this
             transformation is done in the calling function already, set to
             ``False``.
 
         Returns
         -------
-        coo : float
-            Value of the fitted coordinate.
+        coo : np.array
+            Position of intersection as homogeneous coordinate.
 
         '''
-        n_Nones = 0
-        for i, c in enumerate([x, y, z]):
-            if c is None:
-                n_Nones +=1
-                ind = i
-        if n_Nones != 1:
-            raise ValueError('Exactly one of the input numbers for x,y,z must be None.')
-        # Need to give it a number for vstack to work
-        if ind == 0: x = 0.
-        if ind == 1: y = 0.
-        if ind == 2: z = 0.
-
-        xyz = np.vstack([x,y,z]).T
-        def f(val_in):
-            xyz[..., ind] = val_in
-            return self.quartic(xyz, transform=transform)
-        val_out, brent_out = optimize.brentq(f, interval[0], interval[1], full_output=True)
-        if not brent_out.converged:
+        origin = h2e(origin)
+        v = h2e(v)
+        def fun(k, origin, v):
+            out = self.quartic(origin + k[..., None] * v, transform=transform)
+            return out
+        out = optimize.root(fun,
+                            # The starting guess also serves to set the scale
+                            # in the absence of a jacobian.
+                            # So, can't start at 0. Instead, need to guess
+                            # reasonable scale from torus parameters.
+                            # r-R seems like a good guess but does not work at r = R.
+                            # In that case, just pick a number that's small
+                            # relative to r.
+                            max(np.abs(self.r - self.R), self.r * 1e-2) * 0.1,
+                            args=(origin, v))
+        if not out.success:
             raise Exception('Intersection with torus not found.')
-        return val_out
+        else:
+            return e2h(origin + out.x[..., None] * v, 1)
 
     def parametric_surface(self, theta, phi, display):
         '''Parametric representation of surface of torus.
 
         In contrast to `parametric` the input parameters here are 1-d arrays
         and the functions converts that to a rectangular grid.
 
@@ -238,15 +235,15 @@
     def xyzw2parametric(self, xyzw, transform=True, intersectvalid=True):
         '''Calculate (theta, phi) coordinates for point on torus surface.
 
         Parameters
         ----------
         xyzw : np.array of shape (N, 4)
             Coordinates of points on the torus surface in homogeneous
-            coordiantes.
+            coordinates.
 
         transform : bool
             If ``True`` transform ``xyz`` from the global coordinate system
             into the local coordinate system of the torus. If this
             transformation is done in the calling function already, set to
             ``False``.
 
@@ -281,15 +278,15 @@
             phi[~factor] = np.nan
 
         return theta, phi
 
     def normal_parametric(self, theta, phi):
         '''Return the gradient vector field.
 
-        Following the usual concentions, the vector is pointing outwards
+        Following the usual convention, the vector is pointing outwards
         of the torus volume.
 
         Parameters
         ----------
         theta, phi : 1-d np.arrays
             Theta and phi coordinates for points on the torus surface.
 
@@ -305,73 +302,76 @@
         normal = np.empty((len(theta), 3))
         normal[:, 0] = np.cos(theta) * np.cos(phi)
         normal[:, 1] = np.sin(theta)
         normal[:, 2] = np.cos(theta) * np.sin(phi)
 
         return np.einsum('...ij,...j', self.pos4d, e2h(normal, 0))
 
-
     def normal(self, xyzw):
         '''Return the gradient vector field.
 
-        Following the usual concentions, the vector is pointing outwards
+        Following the usual conventions, the vector is pointing outwards
         of the torus volume.
 
         Parameters
         ----------
         xyzw : np.array of shape (N, 4)
-            Coordinates of points in euklidean space. The quartic is calculated
+            Coordinates of points in euclidean space. The quartic is calculated
             for those points. All points need to be on the surface of the torus.
 
         Returns
         -------
         gradient : np.array
-            Gradient vector field in euklidean coordinates. One vector
+            Gradient vector field in euclidean coordinates. One vector
             corresponds to each input point. The shape of ``gradient`` is the
             same as the shape of ``xyz``.
         '''
         if not len(xyzw.shape) == 2:
             raise ValueError('Shape of input array must be (N, 4).')
         theta, phi = self.xyzw2parametric(xyzw, 1)
         return self.normal_parametric(theta, phi)
 
-    def xyz_from_radiusangle(self, radius, angle, interval):
-        '''Get Cartesian coordiantes for radius, angle on the rowland circle.
+    def xyz_from_radiusangle(self, radius, angle, start):
+        '''Get Cartesian coordinates for radius, angle on the rowland circle.
 
-        y, z are calculated from the radius and angle of polar coordiantes in a
+        y, z are calculated from the radius and angle of polar coordinates in a
         plane; then x is determined from the condition that the point lies on
         the Rowland circle.  The plane is perpendicular to the optical axis
         that defines the Rowland circle.
 
         Parameters
         ----------
         radius, angle : float or np.array of shape (n,)
             Polar coordinates in a plane perpendicular to the optical axis
             (where the optical axis is parallel to the x-axis and goes through
             the origin of the `RowlandTorus`.
-            ``angle=0`` conicides with the local y-axis.
-        interval : np.array
-            [min, max] for the search. The quartic can have up to four
-            solutions because a line can intersect a torus in four points and
-            this interval must bracket one and only one solution.
+            ``angle=0`` coincides with the local y-axis.
+        start : number
+            Starting value for the search. The quartic can have up to four
+            solutions because a line can intersect a torus in four points.
+            The solution found thus depends on where the numerical root solver
+            starts the search.
 
         Returns
         -------
         xyz : np.array of shape (n, 3)
-            Eukledian coordinates in the global coordinate system.
+            Euclidean coordinates in the global coordinate system.
         '''
         y = radius * np.cos(angle)
         z = radius * np.sin(angle)
-        x = self.solve_quartic(y=y,z=z, interval=interval, transform=False)
-        xyz = np.vstack([x,y,z, np.ones_like(x)]).T
-        return h2e(np.einsum('...ij,...j', self.pos4d, xyz))
+        # Use np.mean for backwards compatibility.
+        # This used to take a bracketing interval instead of a first guess.
+        out = self.solve_quartic(np.array([np.mean(start), y, z, 1]),
+                               np.array([1, 0, 0, 0]),
+                               transform=False)
+        return h2e(np.einsum('...ij,...j', self.pos4d, out))
 
 
 def design_tilted_torus(f, alpha, beta):
-    '''Design a torus with specifications similar to Heilmann et al. 2010
+    """Design a torus with specifications similar to Heilmann et al. 2010
 
     A `RowlandTorus` is fully specified with the parameters ``r``, ``R`` and
     ``pos4d``.  However, in practice, these numbers might be derived from other
     values.  This function calculates the parameters of a RowlandTorus, based
     on a different set of input values.
 
     Parameters
@@ -406,226 +406,392 @@
     Notes
     -----
     The geometry used here really needs to be explained in a figure.
     However, some notes to explain at least the meaning of the symbols on the
     code are in order:
 
     - Cat : position of on-axis CAT grating (where the Rowland circle intersects the on-axis beam)
-    - H : position of hinge
-    - Ct : Center of Rowland Torus
-    - F : Focal point on axis (at the origin of the coordinate system)
-    - CatH, HF, FCt, etc. : distance between Cat and H, F and Ct, etc.
-    - gamma : see sketch.
-    '''
+    """
     r = f / (2. * np.cos(alpha))
-    CatH = r * np.sqrt(2 * (1 + np.cos(2 * (beta - alpha))))
-    HF = np.sqrt(f**2 + CatH**2 - 2 * f * CatH * np.cos(beta))
-    # If alpha is negative, then everything is "on the other side".
-    # The sign of gamma cannot be found through the arccos, so need to set it here
-    # with sign(alpha).
-    # Another gotcha: np.sign(0) = 0, but we want 1 (or -1)
-    gamma = np.arccos(HF / (2 * r)) * (np.sign(alpha) or 1)
-    R = f / np.sin(np.pi - alpha - (alpha + gamma)) * np.sin(alpha + gamma) - r
-    FCt = f / np.sin(np.pi - alpha - (alpha + gamma)) * np.sin(alpha)
-    x_Ct = FCt * np.cos(alpha + gamma)
-    z_Ct = 0
-    y_Ct = FCt * np.sin(alpha + gamma)
-    orientation = transforms3d.axangles.axangle2mat([0, 0, -1], np.pi/2 - alpha - gamma)
-    pos4d = transforms3d.affines.compose([x_Ct, y_Ct, z_Ct], orientation, np.ones(3))
+    R = r * np.sin(np.pi / 2 - beta)
+    orientation = transforms3d.axangles.axangle2mat([0, 0, -1], beta - alpha)
+    x_Ct = f / 2 - R * np.cos(beta - alpha)
+    y_Ct = f / 2 * np.tan(alpha) + R * np.sin(beta - alpha)
+    pos4d = transforms3d.affines.compose([x_Ct, y_Ct, 0], orientation, np.ones(3))
     return R, r, pos4d
 
 
-class ElementPlacementError(Exception):
-    pass
+def double_rowland_from_channel_distance(d_BF, R, f):
+    '''This prescription is borne out of the engineering needs where it turns out
+    that the spacing between channels d_BF is actually an important parameter
+    so it makes sense to use that here to parameterize the torus, too.
+
+    f is the distance between a theoretical on-axis CAT grating and the focal
+    point.  It's default is a little smaller than 12 m, to leave space to mount
+    the SPOs.
 
+    Parameters
+    ----------
+    d_BF : float
+        Distance between the optical axes of two channels measured
+        in the dispersion direction.
+    R : float
+        Radius of Rowland torus.
+    f : float
+        Distance between a theoretical on-axis CAT grating and the focal
+        point.
 
-class RowlandCircleArray(ParallelCalculated, OpticalElement):
-    '''A 1D collection of elements (e.g. CCDs) arranged on a Rowland circle.
+    Returns
+    -------
+    geometry : dict
+        Dictionary with the keys that hold the input parameters,
+        derived dimensions of the geometry, and the constructed
+        Rowland tori. Three Rowland tori are constructed: One for
+        each channel called (rowland_central, rowland_central_m) and
+        one for the detector (rowland_detector).
 
-    When a `RowlandCircleArray` is initialized, it places a number of elements
-    on the Rowland circle. These elements could be any optical element, but the
-    most common use for this structure is an array of CCDs capturing a
-    spread-out grating spectrum like ACIS-S in Chandra.
+    '''
+    d = 0.5 * d_BF
+    r = 0.5 * np.sqrt(f**2 + d_BF**2)
+    alpha = np.arctan2(d_BF, f)
+    pos = [f - (r + R) * np.cos(alpha),
+           (r + R) * np.sin(alpha),
+           0]
+    orient = [[np.cos(alpha), np.sin(alpha), 0],
+              [-np.sin(alpha), np.cos(alpha), 0],
+              [0., 0., 1]]
+
+
+    posm = [f - (r + R) * np.cos(-alpha),
+           (r + R) * np.sin(-alpha),
+            0]
+
+    orientm = [
+        [np.cos(-alpha), np.sin(-alpha), 0],
+        [-np.sin(-alpha), np.cos(-alpha), 0],
+        [0.0, 0.0, 1],
+    ]
+
+    geometry = {'d_BF': d_BF,
+                'd': d,
+                'f': f,
+                'rowland_central': RowlandTorus(R=R, r=r, position=pos,
+                                                orientation=orient),
+                'rowland_central_m': RowlandTorus(R=R, r=r, position=posm,
+                                                  orientation=orientm)}
+
+    geometry['pos_det_rowland'] = np.array([0, -d, 0, 1])
+    geometry['shift_det_rowland'] = np.eye(4)
+    geometry['shift_det_rowland'][:, 3] = geometry['pos_det_rowland']
+    geometry['rowland_detector'] = RowlandTorus(R, r,
+                                                pos4d=geometry['rowland_central'].pos4d)
+    geometry['rowland_detector'].pos4d = np.dot(geometry['shift_det_rowland'],
+                                                geometry['rowland_detector'].pos4d)
+    geometry['pos_opt_ax'] = {'1': np.array([0, -d, 0, 1]),
+                              '1m': np.array([0, d, 0, 1])}
+    return geometry
+
+
+def add_offset_double_rowland_channels(geometry,
+                                       offsets={'1': [0, -2.5, -7.5],
+                                                '1m': [0, -2.5, -2.5],
+                                                '2': [0, 2.5, 2.5],
+                                                '2m': [0, 2.5, 7.5],
+                                                }):
+    '''Generate Rowland tori for multiple spectral channels in a double-tori design.
+
+    While this function can generate four separate channels (splitting the
+    original and the original mirrored channel in two each).
+    Rowland tori are added to the input geometry dictionary.
 
-    After generation, individual positions can be adjusted by hand by
-    editing the attributes `elem_pos` or `elem_uncertainty`.
-    See `marxs.simulator.Parallel` for details.
+    Parameters
+    ----------
+    geometry : dict
+        Dictionary with the keys from ` double_rowland_from_channel_distance`.
+    offsets : dict
+        Dictionary with the keys that hold the channel ids and the
+        values that hold the offsets in the x, y, and z direction.
+        The default value is set for a total of four channels, where each
+        of the original and the original mirrored channel is split in two.
+        However, the function can be used to generate any number of channels
+        with the naming convention that channels 1, 2, 3, ... are generated
+        from the original channel and channels 1m, 2m, 3m, ... are generated
+        from the original mirrored channel.
+    '''
+    d = geometry['d']
+    geometry['pos_opt_ax'] = {}
+    for k in offsets:
+        sign = 1 if 'm' in k else -1
+        geometry['pos_opt_ax'][k] = np.array([0, sign * d, 0, 1])
+
+    for k, v in offsets.items():
+        geometry['pos_opt_ax'][k][:3] += v
+    # Now offset that Rowland torus in a z axis by a few mm.
+    # Shift is measured from point on symmetry plane.
+    for channel in geometry['pos_opt_ax']:
+        shift_matrix = np.eye(4)
+        shift_matrix[:, 3] = geometry['pos_opt_ax'][channel][:]
+        if channel in ['1', '2']:
+            base_rowland = 'rowland_central'
+        elif channel in ['1m', '2m']:
+            base_rowland = 'rowland_central_m'
+        namer = 'rowland_' + channel
+        geometry[namer] = RowlandTorus(geometry[base_rowland].R,
+                                       geometry[base_rowland].r,
+                                       pos4d=geometry[base_rowland].pos4d)
+        geometry[namer].pos4d = np.dot(shift_matrix,
+                                       geometry[namer].pos4d)
+
+
+class ElementsOnTorus(ParallelCalculated, OpticalElement):
+    '''A collection of elements on a Rowland torus.
+
+    When initialized, it places elements in the space available on the
+    Rowland torus, most commonly, this class is used to place grating facets.
+
+    After generation, individual facet positions can be adjusted by hand by
+    editing the attributes `elem_pos` or `elem_uncertainty`. See
+    `marxs.simulation.Parallel` for details.
 
     After any of the `elem_pos`, `elem_uncertainty` or
     `uncertainty` is changed, `generate_elements` needs to be
-    called to regenerate the final CCD positions.
+    called to regenerate the facets on the GAS.
 
     Parameters
     ----------
-    rowland : RowlandTorus
-    d_element : float
-        Size of the edge of each element, which is assumed to be flat and
-        square. ``d_element`` can be larger than the actual size of the optical
-        element to accommodate a minimum distance between elements from
-        mounting structures.
-    theta : list of floats
-        Angle on the Rowland circle to be covered by detectors.
-        For a continuous array of detectors, this is just a list with two
-        elements ``[inner, outer]``. However, it is also possible to list more
-        than one range in a flat list, to e.g. set one detector in the focus to
-        detect the zeroth order and offset others:
-        ``[inner_1, outer_1, inner_2, outer_2, ...]``.
+    rowland : `marxs.design.rowland.RowlandTorus`
+        Torus on which the elements are placed.
+    d_element : list of two floats
+        Size of the edge of elements along the two (y and z in canonical marxs orientation)
+        edges.
+        ``d_element`` can be larger than the actual size of the silicon
+        membrane or the active area of a CCD chip to accommodate a minimum
+        thickness of the surrounding frame.
+    guess_distance : float
+        A ray can intersect a torus in up to four
+        points. ``guess_distance`` specifies the starting distance for the numerical search for
+        the intersection point to resolve this ambiguity.
+        Default is the start close to outer rim of the torus.
+    optimize_axis : np.array
+        Homogeneous coordinate of the axis along which elements will be moved. This will
+        usually coincide with the optical axis of the telescope.
+        Default is the x-axis in the coordinate system of the torus.
+    normal_spec : np.array or callable
+        see `~marxs.simulator.simulator.ParallelCalculated` for details.
+        Default for this class: Pointing **inward** into the Rowlandtorus,
+        as one would do for an array of e.g. CCDs.
+    parallel_spec : np.array or callable
+        see `~marxs.simulator.simulator.ParallelCalculated` for details.
+        Default for this class: Symmetry axis of the torus.
     '''
+    def __init__(self, **kwargs):
+        self.rowland = kwargs.pop('rowland')
+        # Default to a slightly positive number
+        self.guess_distance = kwargs.pop('guess_distance',
+                                         self.rowland.r + self.rowland.R)
+        self.d_element = kwargs.pop('d_element')
+        self.optimize_axis = np.asanyarray(kwargs.pop('optimize_axis',
+                                           self.rowland.pos4d @ np.array([1, 0, 0, 0])))
+        self.id_col = kwargs.pop('id_col', 'facet')
 
-    id_col = 'CCD_ID'
-
-    def __init__(self, rowland, d_element, theta, **kwargs):
-        self.rowland = rowland
-        if not len(theta) % 2 == 0:
-            raise ValueError('radius must be a list of [inner_1, outer_1, inner_2, outer_2, ...].')
-        if np.max(np.abs(theta)) > 10:
-            raise ValueError('Input angles >> 2 pi. Did you use degrees (radian expected)?')
-        self.theta = theta
-        self.d_element = d_element
-        kwargs['normal_spec'] = self.rowland_normal
-        kwargs['parallel_spec'] =  self.rowland.parametric(0., 0.) - self.rowland.parametric(1., 0.)
-        kwargs['pos_spec'] = self.xyzwpos
-
-        super(RowlandCircleArray, self).__init__(**kwargs)
+        # Defaults changes from parent classes. Document! Or remove?
+        if 'normal_spec' not in kwargs.keys():
+            kwargs['normal_spec'] = lambda xyzw: -self.rowland.normal(xyzw)
+        if 'parallel_spec' not in kwargs.keys():
+            # If not given, make parallel to Rowland circle at origin.
+            kwargs['parallel_spec'] = self.rowland.pos4d @ np.array([0, 1, 0, 0])
+        kwargs['pos_spec'] = self.elempos
 
-    def rowland_normal(self, xyzw):
-        return self.rowland.normal(xyzw)
+        super().__init__(**kwargs)
 
-    def xyzwpos(self):
-        radii = self.distribute_elements_on_arc()
-        return self.rowland.parametric(radii, 0.)
+    def elemposyz(self):
+        '''Specify the element position in the yz plane
 
-    def max_elements_on_arc(self, theta):
-        '''Max number of elements that fit on an arc
+        For the torus, the Rowland circle lies in the xy plane and the symmetry
+        axis of the torus is the y-axis. In this class, the position of the
+        elements is specified in the yz plane in the coordinates of the
+        torus and the remaining coordinate.
 
-        Parameters
-        ----------
-        theta : list of two floats
-            angle range that should be covered by elements
+        This function will be customized by derived classes.
 
         Returns
         -------
-        n : int
-            Number of elements needed to cover a given radius segment.
-            Elements might reach beyond the limits if the arc length
-            is not an integer multiple of the element size.
+        ypos, zpos : np.array
+            1D arrays of y and z positions for the elements distributed in 2D.
         '''
-        return int(np.ceil(self.rowland.r * (theta[1] - theta[0]) / self.d_element))
+        raise NotImplementedError
 
-    def distribute_elements_on_arc(self):
-        '''Distributes elements as evenly as possible along an arc segment.
+    def elempos(self):
+        '''Generate 3D positions of elements
 
-        Returns
-        -------
-        theta : np.ndarray
-            Theta coordinates of the element *center* positions.
-        '''
-        theta = []
-        for i in range(len(self.theta) // 2):
-            bracket = self.theta[2 * i: 2 * i + 2]
-            n = self.max_elements_on_arc(bracket)
-            theta.append(np.mean(bracket) +
-                         np.arange(- n / 2 + 0.5, n / 2 + 0.5) * self.d_element / self.rowland.r)
-        return np.hstack(theta)
+        For each element, y and z coordinates in the torus coordinate system
+        are generated from ``self.elemposyz`` and the elements are placed at
+        x=0. Then, that initial coordinate is transformed into the global
+        coordinate system and moved by
+        ``self.guess_distance * self.optimize_axis``. The resulting position
+        is the starting point for numerical optimization along
+        ``self.optimize_axis`` to find the on-torus location.
+        '''
+        ypos, zpos = self.elemposyz()
+        posyz = np.vstack([np.zeros_like(ypos), ypos, zpos])
+        origin = np.einsum('...ij,...j', self.rowland.pos4d, e2h(posyz.T, 1)) + self.guess_distance * self.optimize_axis
+        # solve_quartic is not vectorized (because scipy.optimize is not)
+        # so need to pass in one element at a time.
+
+        # now, origin is in the global coordinate system.
+        # Because transform=True is the default in solve_quartic that works.
+        return np.vstack([self.rowland.solve_quartic(o, self.optimize_axis) for o in origin])
 
 
-class LinearCCDArray(ParallelCalculated, OpticalElement):
-    '''A 1D collection of elements (e.g. CCDs) arranged on a Rowland circle.
+class RectangularGrid(ElementsOnTorus):
+    '''A collection of diffraction gratings on the Rowland torus.
+
+    This class is similar to ``marxs.design.rowland.GratingArrayStructure`` but
+    instead of placing elements on concentric circles, they are placed to fill
+    a rectangular area.
 
-    When a `LinearCCDArray` is initialized, it places a number of elements on
-    the Rowland circle. These elements could be any optical element, but the
-    most common use for this structure is an array of CCDs capturing a
-    spread-out grating spectrum like ACIS-S in Chandra.
+    When initialized, it places elements in the space available on the
+    Rowland circle, most commonly, this class is used to place grating facets.
 
-    After generation, individual positions can be adjusted by hand by editing
-    the attributes `elem_pos` or `elem_uncertainty`. See `Parallel` for
-    details.
+    After generation, individual facet positions can be adjusted by hand by
+    editing the attributes `elem_pos` or `elem_uncertainty`. See
+    `marxs.simulation.Parallel` for details.
 
     After any of the `elem_pos`, `elem_uncertainty` or
     `uncertainty` is changed, `generate_elements` needs to be
-    called to regenerate the final CCD positions.
+    called to regenerate the facets on the GAS.
 
     Parameters
     ----------
-    rowland : RowlandTorus
-    d_element : float
-        Size of the edge of each element, which is assumed to be flat and
-        square. (``d_element`` can be larger than the actual size of the
-        optical element to accommodate a minimum distance between elements
-        from mounting structures.
-    x_range: list of 2 floats
-        Minimum and maximum of the x coordinate that is searched for an
-        intersection  with the torus. A line can intersect a torus in up to
-        four points. ``x_range`` specifies the range for the numerical search
-        for the intersection point.
-    radius : list of floats
-        Inner and outer radius as measured in the yz-plane from the center of
-        the `LinearCCDArray`. Can be negative to place elements on both sides
-        of the center of the `LinearCCDArray`. Elements will be placed
-        ``d_element`` apart; if a non-integer number of elements is needed to
-        cover the ``radius``, elements will reach beyond the given numbers.
-        For a continuous array of detectors, this is just a list with two
-        elements ``[r_inner, r_outer]``. However, it is also possible to list
-        more than one range in a flat list, to e.g. set one detector in the
-        focus to detect the zeroth order and offset others:
-        ``[r_inner_1, r_outer_1, r_inner_2, r_outer_2, ...]``.
-    phi : floats
-        Direction of line through the centers of all elements. :math:`\phi=0`
-        is on the positive y axis. Angles are given in radian.
+    y_range, z_range: list of two floats
+        Limits of the rectangular area where gratings are placed.
+        To place only one element, make both limits the same, e.g.
+        ``z_range=[5, 5]`` will place one element in each row in z
+        centered on $z=5$.
+        This is given in the coordinate system of the torus, i.e. y is the
+        plane of the Rowland circle and both numbers are measured from the
+        center of the Rowland torus.
+        Default for z-range: [-1e-10, 1e-10]. This will make one element
+        centered on 0 in z-range.
+
     '''
+    def __init__(self, **kwargs):
+        self.y_range = kwargs.pop('y_range')
+        self.z_range = kwargs.pop('z_range', [-1e-10, 1e-10])
 
-    id_col = 'CCD_ID'
+        super().__init__(**kwargs)
 
-    def __init__(self, rowland, d_element, x_range, radius, phi, **kwargs):
-        self.rowland = rowland
-        if not len(radius) % 2 == 0:
-            raise ValueError('radius must be a list of [inner_1, outer_1, inner_2, outer_2, ...].')
-        radarray = np.array(radius)
-        if not np.all(radarray[1::2] > radarray[::2]):
-            raise ValueError('Outer radius must be larger than inner radius.')
-        self.radius = radius
-
-        if np.max(np.abs(phi)) > 10:
-            raise ValueError('Input angles >> 2 pi. Did you use degrees (radian expected)?')
-        self.phi = phi
-        self.x_range = x_range
-        self.d_element = d_element
+    def elemposyz(self):
+        n_y = int(np.ceil((self.y_range[1] - self.y_range[0]) / self.d_element[0]))
+        n_z = int(np.ceil((self.z_range[1] - self.z_range[0]) / self.d_element[1]))
+        n_y = max(1, n_y)
+        n_z = max(1, n_z)
+
+        # n_y and n_z are rounded up, so they cover a slightly larger range than y/z_range
+        width_y = n_y * self.d_element[0]
+        width_z = n_z * self.d_element[1]
 
-        if 'normal_spec' not in kwargs.keys():
-            kwargs['normal_spec'] = self.rowland_normal
+        ypos = np.arange(0.5 * (self.y_range[0] - width_y + self.y_range[1] + self.d_element[0]), self.y_range[1], self.d_element[0])
+        zpos = np.arange(0.5 * (self.z_range[0] - width_z + self.z_range[1] + self.d_element[1]), self.z_range[1], self.d_element[1])
 
-        if 'parallel_spec' not in kwargs.keys():
-            radii = self.distribute_elements_on_radius()
-            kwargs['parallel_spec'] =  e2h(normalized_vector(self.xyz_from_radiusangle(radii[1], self.phi, self.x_range) - self.xyz_from_radiusangle(radii[0], self.phi, self.x_range)), 0)
+        ypos, zpos = np.meshgrid(ypos, zpos)
+
+        return ypos.flatten(), zpos.flatten()
 
-        if 'pos_spec' not in kwargs.keys():
-            kwargs['pos_spec'] = self.xyzwpos
 
-        super(LinearCCDArray, self).__init__(**kwargs)
+class CircularMeshGrid(ElementsOnTorus):
+    '''A collection of diffraction gratings on the Rowland torus filling a circle.
+
+    When initialized, it places elements in the space available on the
+    Rowland circle, most commonly, this class is used to place grating facets.
+
+    After generation, individual facet positions can be adjusted by hand by
+    editing the attributes `elem_pos` or `elem_uncertainty`. See
+    `marxs.simulation.Parallel` for details.
+
+    After any of the `elem_pos`, `elem_uncertainty` or
+    `uncertainty` is changed, `generate_elements` needs to be
+    called to regenerate the facets on the GAS.
+
+    Parameters
+    ----------
+    radius : list of two floats
+        Inner and outer radius of the circle.
+    '''
+
+    def __init__(self, **kwargs):
+        self.radius = kwargs.pop('radius')
+        super().__init__(**kwargs)
 
-    def rowland_normal(self, xyzw):
-        return self.rowland.normal(xyzw)
-
-    def xyz_from_radiusangle(self, r, phi, x_range):
-        '''Wrap `marxs.design.RowlandTorus.xyz_from_radiusangle` for better error message'''
-        try:
-            xyz = self.rowland.xyz_from_radiusangle(r, phi, x_range)
-        except ValueError as e:
-            if 'f(a) and f(b) must have different signs' in str(e):
-                raise ElementPlacementError('No intersection with Rowland torus in range {0}'.format(self.x_range))
+    def elemposyz(self):
+        n_y = int(np.ceil(2 * self.radius[1] / self.d_element[0]))
+        y_width = n_y * self.d_element[0]
+        y_pos = np.arange(- y_width / 2, self.radius[1], self.d_element[0])
+
+        ypos = []
+        zpos = []
+
+        for y in y_pos:
+            if np.abs(y) > self.radius[1]:
+                # Outermost layer. Center might be outside outer radius
+                z = np.array([0])
             else:
-                # Something else went wrong
-                raise e
-        return xyz
+                z_outer = np.sqrt(self.radius[1]**2 - y**2)
+                if np.abs(y) > self.radius[0]:
+                    n_z = int(np.ceil(2 * z_outer / self.d_element[1]))
+                    z_width = n_z * self.d_element[1]
+                    z = np.arange(- z_width / 2, z_outer, self.d_element[1])
+                else:
+                    z_inner = np.sqrt(self.radius[0]**2 - y**2)
+                    z_mid = 0.5 * (z_inner + z_outer)
+                    n_z = int(np.ceil((z_outer - z_inner) / self.d_element[1]))
+                    z_width = n_z * self.d_element[1]
+                    z = np.arange(z_mid - z_width / 2, z_outer, self.d_element[1])
+                    z = np.hstack([-z, z])
+
+            ypos.extend([y] * len(z))
+            zpos.extend(z)
+        return ypos, zpos
 
-    def xyzwpos(self):
-        radii = self.distribute_elements_on_radius()
-        facet_pos = np.array([self.xyz_from_radiusangle(r, self.phi, self.x_range).flatten() for r in radii])
-        return e2h(facet_pos, 1)
 
+class GratingArrayStructure(ElementsOnTorus):
+    '''Collection of diffraction gratings on the Rowland Torus
+
+    When a ``GratingArrayStructure`` (GAS) is initialized, it places elements
+    in the space available on the Rowland circle, most commonly, this class is
+    used to place grating facets.
+
+    After generation, individual facet positions can be adjusted by hand by
+    editing the attributes `elem_pos` or `elem_uncertainty`. See `Parallel` for
+    details.
+
+    After any of the `elem_pos`, `elem_uncertainty` or `uncertainty` is
+    changed, `generate_elements` needs to be called to regenerate the facets on
+    the GAS.
+
+    Parameters
+    ----------
+    radius : list of 2 floats
+        Inner and outer radius of the GAS as measured in the yz-plane from the
+        origin.
+
+    phi : float or list of 2 floats
+        Bounding angles for a segment covered by the GSA. :math:`\phi=0` is on
+        the positive y axis. The segment fills the space from ``phi1`` to
+        ``phi2`` in the usual mathematical way (counterclockwise).  Angles are
+        given in radian. Note that ``phi[1] < phi[0]`` is possible if the
+        segment crosses the y axis.
+        Alternatively, ``phi`` can just be a single number. In that case, there
+        will be exactly one element per radius.
+
+    '''
+    def __init__(self, **kwargs):
+        self.phi = kwargs.pop('phi', [0., 2*np.pi])
+        self.radius = kwargs.pop('radius')
+        super().__init__(**kwargs)
 
     def max_elements_on_radius(self, radius):
         '''Distribute elements on a radius.
 
         Parameters
         ----------
         radius : list of two floats
@@ -634,15 +800,15 @@
         Returns
         -------
         n : int
             Number of elements needed to cover a given radius segment.
             Elements might reach beyond the radius limits if the difference between
             inner and outer radius is not an integer multiple of the element size.
         '''
-        return int(np.ceil((radius[1] - radius[0]) / self.d_element))
+        return int(np.ceil((radius[1] - radius[0]) / self.d_element[0]))
 
     def distribute_elements_on_radius(self):
         '''Distributes elements as evenly as possible along a radius.
 
         .. note::
            Unlike `distribute_elements_on_arc`, this function will have
            elements reaching beyond the limits of the radius, if the distance
@@ -656,253 +822,65 @@
 
         '''
         radii = []
         for i in range(len(self.radius) // 2):
             radiusbracket = self.radius[2 * i: 2 * i + 2]
             n = self.max_elements_on_radius(radiusbracket)
             radii.append(np.mean(radiusbracket) +
-                         np.arange(- n / 2 + 0.5, n / 2 + 0.5) * self.d_element)
+                         np.arange(- n / 2 + 0.5, n / 2 + 0.5) * self.d_element[0])
         return np.hstack(radii)
 
 
-class GratingArrayStructure(LinearCCDArray):
-    '''A collection of diffraction gratings on the Rowland torus.
-
-    When a ``GratingArrayStructure`` (GAS) is initialized, it places elements
-    in the space available on the Rowland circle, most commonly, this class is
-    used to place grating facets.
-
-    After generation, individual facet positions can be adjusted by hand by
-    editing the attributes `elem_pos` or `elem_uncertainty`. See `Parallel` for
-    details.
-
-    After any of the `elem_pos`, `elem_uncertainty` or `uncertainty` is
-    changed, `generate_elements` needs to be called to regenerate the facets on
-    the GAS.
-
-    Parameters
-    ----------
-    rowland : RowlandTorus
-    d_element : float
-        Size of the edge of a element, which is assumed to be flat and square.
-        (``d_element`` can be larger than the actual size of the silicon
-        membrane to accommodate a minimum thickness of the surrounding frame.)
-
-    x_range: list of 2 floats
-        Minimum and maximum of the x coordinate that is searched for an
-        intersection with the torus. A ray can intersect a torus in up to four
-        points. ``x_range`` specififes the range for the numerical search for
-        the intersection point.
-
-    radius : list of 2 floats
-        Inner and outer radius of the GAS as measured in the yz-plane from the
-        origin.
-
-    phi : list of 2 floats
-        Bounding angles for a segment covered by the GSA. :math:`\phi=0` is on
-        the positive y axis. The segment fills the space from ``phi1`` to
-        ``phi2`` in the usual mathematical way (counterclockwise).  Angles are
-        given in radian. Note that ``phi[1] < phi[0]`` is possible if the
-        segment crosses the y axis.
-
-    Notes
-    -----
-    This class derives from `LinearCCDArray`, which is a 1D arrangement of
-    elements.  `GratingArrayStructure` also picks radii, but places several
-    elements at each radius.
-
-    '''
-
-    tangent_to_torus = False
-    '''If ``True`` the default orientation (before applying blaze, uncertainties etc.) of elements is
-    such that they are tangents to the torus in the center of the element.
-    If ``False`` they are perpendicular to perfectly focussed rays.
-    '''
-
-    id_col = 'facet'
-
-    def __init__(self, rowland, d_element, x_range, radius, phi=[0., 2*np.pi],
-                 parallel_spec=np.array([0., 1., 0., 0.]), **kwargs):
-        if np.min(radius) < 0:
-            raise ValueError('Radius must be positive.')
-        kwargs['parallel_spec'] = parallel_spec
-        kwargs['pos_spec'] = self.xyzwpos
-
-        super(GratingArrayStructure, self).__init__(rowland, d_element, x_range, radius, phi, **kwargs)
-
-    def calc_ideal_center(self):
-        '''Position of the center of the GSA, assuming placement on the Rowland circle.'''
-        a = (self.phi[0] + anglediff(self.phi) / 2 ) % (2. * np.pi)
-        r = sum(self.radius) / 2
-        return self.rowland.xyz_from_radiusangle(r, a, self.x_range).flatten()
-
     def max_elements_on_arc(self, radius):
         '''Calculate maximal number of elements that can be placed at a certain radius.
 
         Parameters
         ----------
         radius : float
             Radius of circle where the centers of all elements will be placed.
         '''
-        return radius * anglediff(self.phi) // self.d_element
+        return radius * anglediff(self.phi) // self.d_element[1]
 
     def distribute_elements_on_arc(self, radius):
         '''Distribute elements on an arc.
 
         The elements are distributed as evenly as possible over the arc.
 
         .. note::
 
           Contrary to `distribute_elements_on_radius`, elements never stretch
           beyond the limits set by the ``phi`` parameter of the GAS. If an arc
           segment is not wide enough to accommodate at least a single element,
           it will go empty.
+          (The exception to that is is ``phi`` is a single value. In that case,
+          there will be exactly one element.)
 
         Parameters
         ----------
         radius : float
             radius of arc where the elements are to be distributed.
 
         Returns
         -------
         centerangles : array
             The phi angles for centers of the elements at ``radius``.
 
         '''
+        if len(self.phi) == 1:
+            return self.phi
         # arc is most crowded on inner radius
-        n = self.max_elements_on_arc(radius - self.d_element / 2)
-        element_angle = self.d_element / (2. * np.pi * radius)
+        n = self.max_elements_on_arc(radius - self.d_element[0] / 2)
+        element_angle = self.d_element[1] / (2. * np.pi * radius)
         # thickness of space between elements, distributed equally
         d_between = (anglediff(self.phi) - n * element_angle) / (n + 1)
         centerangles = d_between + 0.5 * element_angle + np.arange(n) * (d_between + element_angle)
         return (self.phi[0] + centerangles) % (2. * np.pi)
 
-    def getelem_xyzw(self):
-        pos = []
+    def elemposyz(self):
+        angles = []
         radii = self.distribute_elements_on_radius()
         for r in radii:
-            angles = self.distribute_elements_on_arc(r)
-            for a in angles:
-                pos.append(self.rowland.xyz_from_radiusangle(r, a, self.x_range).flatten())
-        return e2h(np.array(pos), 1)
-
-    def calculate_elempos(self):
-        '''Calculate the position of elements based on some algorithm.
-
-        Returns
-        -------
-        pos4d : list of arrays
-            List of affine transformations that bring an optical element
-            centered on the origin of the coordinate system with the active
-            plane in the yz-plane to the required facet position on the Rowland
-            torus.
-        '''
-        pos4d = []
-
-        xyzw = self.getelem_xyzw()
-        normals = self.get_spec('normal_spec', xyzw)
-        parallels = self.get_spec('parallel_spec', xyzw, normals)
-
-        for i in range(xyzw.shape[0]):
-
-            # Find the rotation between [1, 0, 0] and the new normal
-            # Keep grooves (along e_y) parallel to e_y
-            rot_mat = ex2vec_fix(h2e(normals[i, :]), h2e(parallels[i, :]))
-
-            pos4d.append(transforms3d.affines.compose(h2e(xyzw[i, :]), rot_mat, np.ones(3)))
-        return pos4d
-
-
-class RectangularGrid(ParallelCalculated, OpticalElement):
-    '''A collection of diffraction gratings on the Rowland torus.
-
-    This class is similar to ``marxs.design.rowland.GratingArrayStructure`` but
-    instead of placing elements on concentric circles, they are placed to fill
-    a rectangular area.
-
-    When initialized, it places elements in the space available on the
-    Rowland circle, most commonly, this class is used to place grating facets.
-
-    After generation, individual facet positions can be adjusted by hand by
-    editing the attributes `elem_pos` or `elem_uncertainty`. See
-    `marxs.simulation.Parallel` for details.
-
-    After any of the `elem_pos`, `elem_uncertainty` or
-    `uncertainty` is changed, `generate_elements` needs to be
-    called to regenerate the facets on the GAS.
-
-    Parameters
-    ----------
-    rowland : RowlandTorus
-    d_element : float
-        Size of the edge of a element, which is assumed to be flat and square.
-        (``d_element`` can be larger than the actual size of the silicon
-        membrane to accommodate a minimum thickness of the surrounding frame.)
-    x_range: list of 2 floats
-        Minimum and maximum of the x coordinate that is searched for an
-        intersection with the torus. A ray can intersect a torus in up to four
-        points. ``x_range`` specififes the range for the numerical search for
-        the intersection point.
-    y_range, z_range: lost of two floats
-        limits of the rectangular area where gratings are placed.
-
-    '''
-
-    id_col = 'facet'
-
-    def __init__(self, **kwargs):
-        self.x_range = kwargs.pop('x_range')
-        self.y_range = kwargs.pop('y_range')
-        self.z_range = kwargs.pop('z_range')
-        self.rowland = kwargs.pop('rowland')
-        self.d_element = kwargs.pop('d_element')
-        kwargs['pos_spec'] = self.elempos
-        if 'normal_spec' not in kwargs.keys():
-            kwargs['normal_spec'] = np.array([0., 0., 0., 1.])
-        if 'parallel_spec' not in kwargs.keys():
-            kwargs['parallel_spec'] = np.array([0., 1., 0., 0.])
-
-        super(RectangularGrid, self).__init__(**kwargs)
-
-    def elempos(self):
-
-        n_y = int(np.ceil((self.y_range[1] - self.y_range[0]) / self.d_element))
-        n_z = int(np.ceil((self.z_range[1] - self.z_range[0]) / self.d_element))
-
-        # n_y and n_z are rounded up, so they cover a slighty larger range than y/z_range
-        width_y = n_y * self.d_element
-        width_z = n_z * self.d_element
-
-        ypos = np.arange(0.5 * (self.y_range[0] - width_y + self.y_range[1] + self.d_element), self.y_range[1], self.d_element)
-        zpos = np.arange(0.5 * (self.z_range[0] - width_z + self.z_range[1] + self.d_element), self.z_range[1], self.d_element)
-        ypos, zpos = np.meshgrid(ypos, zpos)
-
-        xpos = []
-        for y, z in zip(ypos.flatten(), zpos.flatten()):
-            xpos.append(self.rowland.solve_quartic(y=y, z=z, interval=self.x_range))
-
-        return np.vstack([np.array(xpos), ypos.flatten(), zpos.flatten(), np.ones_like(xpos)]).T
-
-    def calculate_elempos(self):
-        '''Calculate the position of elements based on some algorithm.
-
-        Returns
-        -------
-        pos4d : list of arrays
-            List of affine transformations that bring an optical element centered
-            on the origin of the coordinate system with the active plane in the
-            yz-plane to the required facet position on the Rowland torus.
-        '''
-        pos4d = []
-
-        xyzw = self.elempos()
-        normals = self.get_spec('normal_spec', xyzw)
-        parallels = self.get_spec('parallel_spec', xyzw, normals)
-
-        for i in range(xyzw.shape[0]):
-
-            # Find the rotation between [1, 0, 0] and the new normal
-            # Keep grooves (along e_y) parallel to e_y
-            rot_mat = ex2vec_fix(h2e(normals[i, :]), h2e(parallels[i, :]))
-
-            pos4d.append(transforms3d.affines.compose(h2e(xyzw[i, :]), rot_mat, np.ones(3)))
-        return pos4d
+            angles.append(self.distribute_elements_on_arc(r))
+        # Turn lists of lists into flat numpy array
+        radii = np.concatenate([[radii[i]] * len(a) for i, a in enumerate(angles)])
+        angles = np.concatenate(angles)
+        return radii * np.sin(angles), radii * np.cos(angles)
```

### Comparing `marxs-1.2/marxs/design/tests/data/wiggle_global.fits` & `marxs-2.0/marxs/design/tests/data/wiggle_global.fits`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/design/tests/test_design.py` & `marxs-2.0/marxs/design/tests/test_design.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
+from numpy.testing import assert_allclose
 from scipy.stats import kstest
 import transforms3d
 import pytest
 from astropy.coordinates import SkyCoord
 import astropy.units as u
+from astropy.utils.data import get_pkg_data_filename
 
-from ..rowland import (RowlandTorus, GratingArrayStructure, LinearCCDArray,
-                       RowlandCircleArray,
+from ..rowland import (RowlandTorus, GratingArrayStructure,
+                       RectangularGrid,
                        find_radius_of_photon_shell, design_tilted_torus,
-                       ElementPlacementError)
+                       CircularMeshGrid,
+                       double_rowland_from_channel_distance,
+                       add_offset_double_rowland_channels,
+                       )
 from ...optics.base import FlatOpticalElement
 from ...source import PointSource, FixedPointing
 from ...optics import MarxMirror, OrderSelector, FlatGrating
-from ...math.utils import h2e
+from ...math.utils import h2e, xyz2zxy
 
 class mock_facet(FlatOpticalElement):
     '''Lightweight class with no functionality for tests.'''
     pass
 
 def test_radius_of_photon_shell():
     mysource = PointSource(coords=SkyCoord(30., 30., unit="deg"))
     photons = mysource.generate_photons(1. * u.ks)
     mypointing = FixedPointing(coords=SkyCoord(30, 30., unit='deg'))
     photons = mypointing.process_photons(photons)
-    marxm = MarxMirror('./marxs/optics/hrma.par', position=np.array([0., 0, 0]))
+    marxm = MarxMirror(get_pkg_data_filename('hrma.par', package='marxs.optics'), position=np.array([0., 0, 0]))
     photons = marxm(photons)
     r1, r2 = find_radius_of_photon_shell(photons, 1, 9e3)
     assert abs(r1 - 433.) < 1.
     assert abs(r2 - 442.) < 1.
     r1, r2 = find_radius_of_photon_shell(photons, 1, 9e3, percentile=[49, 49.001])
     assert (r2 - r1) < 0.01
 
@@ -36,30 +41,30 @@
     '''Test the trivial case with analytic answers and consistency for other angles'''
     R, r, pos4d = design_tilted_torus(10, 0., 0.)
     assert R == 5
     assert r == 5
     assert np.all(pos4d == np.eye(4))
     # This is a solution that looks good by hand, but could still be slightly wrong...
     R, r, pos4d = design_tilted_torus(10, np.deg2rad(3), np.deg2rad(6))
-    assert r == 5.0068617299896054
-    assert R == 4.9794336175561327
-    assert pos4d[0,3] == 0.027390523158633273
+    assert r == pytest.approx(5.0068617299896054)
+    assert R == pytest.approx(4.9794336175561327)
+    assert pos4d[0,3] == pytest.approx(0.027390523158633273)
     # The z axis should be unchanged
     assert np.allclose(pos4d[[0,1],2], 0)
 
 def test_design_tilted_torus_negative_angles():
     '''Tilt the torus the other way. Should be same geometry in general.'''
     R, r, pos4d = design_tilted_torus(10, np.deg2rad(3), np.deg2rad(6))
     Rn, rn, pos4dn = design_tilted_torus(10, np.deg2rad(-3), np.deg2rad(-6))
-    assert R == Rn
-    assert r == rn
-    assert pos4d[0,3] == pos4dn[0, 3]
+    assert R == pytest.approx(Rn)
+    assert r == pytest.approx(rn)
+    assert pos4d[0,3] == pytest.approx(pos4dn[0, 3])
     assert pos4d[2, 3] == 0 # torus in xy plane
     assert pos4dn[2, 3] == 0
-    assert pos4d[1, 3] == - pos4dn[1, 3]
+    assert pos4d[1, 3] == pytest.approx(-pos4dn[1, 3])
 
 def test_torus():
     '''Compare parametric equation of torus with non-parametric.
     '''
     R = 2.
     r = 1.
 
@@ -73,35 +78,29 @@
     xyz = h2e(xyzw)
 
     assert np.allclose(mytorus.quartic(xyz), 0.)
     # This torus has pos4d=eye(4), so the same results should come out with this shortcut
     assert np.allclose(mytorus.quartic(xyz, transform=False), 0.)
 
 def test_torus_solve_quartic():
-    '''solve_quartic helps to find point on the torus if two coordinates are fixed.'''
-    mytorus = RowlandTorus(2., 1.)
+    '''solve_quartic helps to find points on the torus.
+
+    This test could make use of the hypothesis testing package.
+    '''
+    mytorus = RowlandTorus(5., 4.)
     xyzw = mytorus.parametric([.34, 1.23], [.4, 4.5])
-    xyz = h2e(xyzw)
 
     for i in [0, 1]:
-        for j in range(3):
-            kwargs = {'x': xyz[i, 0], 'y': xyz[i, 1], 'z': xyz[i, 2],
-                      'interval' : np.array([-0.1, 0.1]) + xyz[i, j]}
-            kwargs['xyz'[j]] = None
-            assert np.allclose(xyz[i, j], mytorus.solve_quartic(**kwargs))
-
-    # Nothing to solve for
-    with pytest.raises(ValueError) as e:
-        out = mytorus.solve_quartic(x=1, y=1, z=1)
-    assert 'Exactly one of the input numbers' in str(e.value)
-
-    # Too many parameters to solve for
-    with pytest.raises(ValueError) as e:
-        out = mytorus.solve_quartic(x=1, y=None, z=None)
-    assert 'Exactly one of the input numbers' in str(e.value)
+        # generate random direction in homogeneous coordinates
+        direction = np.random.rand(4) - 0.5
+        direction[3] = 0
+        assert np.allclose(xyzw[i, :],
+                            mytorus.solve_quartic(origin=xyzw[i, :] + 0.1 * direction,
+                                                  v=direction))
+
 
 def test_rotated_torus():
     '''Test the torus equation for a set of points.
 
     Importantly, we use a parametric description of the torus here, which is
     different from the actual implementation.
     '''
@@ -207,26 +206,25 @@
 def test_GratingArrayStructure():
     '''Check a GAS for consistency
 
     The expected numbers for this one are hand-checked and plotted and thus
     can be taken as known-good to prevent regressions later.
     '''
     myrowland = RowlandTorus(10000., 10000.)
-    gas = GratingArrayStructure(myrowland, 30., [10000., 20000.], [300., 600.], phi=[-0.2*np.pi, 0.2*np.pi], elem_class=mock_facet)
+    gas = GratingArrayStructure(rowland=myrowland,
+                                d_element=[30., 30.],
+                                radius=[300., 600.],
+                                phi=[-0.2*np.pi, 0.2*np.pi], elem_class=mock_facet)
     assert gas.max_elements_on_arc(300.) == 12
     angles = gas.distribute_elements_on_arc(315.) % (2. * np.pi)
     # This is a wrap-around case. Hard to test in general, but here I know the numbers
     assert np.alltrue((angles < 0.2 * np.pi) | (angles > 1.8 * np.pi))
     assert gas.max_elements_on_radius(gas.radius) == 10
     assert np.all(gas.distribute_elements_on_radius() == np.arange(315., 600., 30.))
     assert len(gas.elem_pos) == 177
-    center = gas.calc_ideal_center()
-    assert center[2] == 0
-    assert center[1] == (300. + 600.) / 2.
-    assert 2e4 - center[0] < 20.  # R_rowland >> r_gas  -> center close to R_rowland
     # fig, axes = plt.subplots(2,2)
     # for elem in [[axes[0, 0], 0, 1], [axes[0, 1], 0, 2], [axes[1, 0], 1, 2]]:
     #     for f in gas.elem_pos:
     #         elem[0].plot(f[elem[1],3], f[elem[2],3], 's')
     # plt.show()  # or move mouse in window or something.
 
     # There is a test missing here that the rotational part works correctly.
@@ -235,79 +233,92 @@
     # Check that initially all uncertainties are 0
     for i in range(len(gas.elem_pos)):
         assert np.allclose(gas.elem_pos[i], gas.elements[i].pos4d)
 
 def test_GAS_multipleradii():
     '''Radius can be a list of many pairs.'''
     myrowland = RowlandTorus(1000., 1000.)
-    gas1 = GratingArrayStructure(myrowland, 60., [1000., 2000.], [300., 400.], elem_class=mock_facet)
-    gas2 = GratingArrayStructure(myrowland, 60., [1000., 2000.], [500., 540.], elem_class=mock_facet)
-    gas = GratingArrayStructure(myrowland, 60., [1000., 2000.], [300., 400., 500., 540.], elem_class=mock_facet)
+    gas1 = GratingArrayStructure(rowland=myrowland, d_element=[60., 60.],
+                                 radius=[300., 400.], elem_class=mock_facet)
+    gas2 = GratingArrayStructure(rowland=myrowland, d_element=[60., 60.],
+                                 radius=[500., 540.], elem_class=mock_facet)
+    gas = GratingArrayStructure(rowland=myrowland, d_element=[60., 60.],
+                                radius=[300., 400., 500., 540.],
+                                elem_class=mock_facet)
 
     r1 = gas1.distribute_elements_on_radius()
     r2 = gas2.distribute_elements_on_radius()
     r = gas.distribute_elements_on_radius()
     assert np.all(np.in1d(r, np.union1d(r1, r2)))
 
 
 def test_GratingArrayStructure_2pi():
     '''test that delta_phi = 2 pi means "full circle" and not 0
     '''
     myrowland = RowlandTorus(10000., 10000.)
-    gas = GratingArrayStructure(myrowland, 30., [10000., 20000.], [300., 600.], phi=[0, 2*np.pi], elem_class=mock_facet)
+    gas = GratingArrayStructure(rowland=myrowland, d_element=[30., 30.],
+                                radius=[300., 600.],
+                                phi=[0, 2*np.pi], elem_class=mock_facet)
     assert gas.max_elements_on_arc(300.) > 10
     n = len(gas.elem_pos)
     yz = np.empty((n, 2))
     for i, p in enumerate(gas.elem_pos):
         yz[i, :] = p[1:3, 3]
     phi = np.arctan2(yz[:, 1], yz[:, 0])
     ks, pvalue = kstest((phi + np.pi) / (2 * np.pi), 'uniform')
     assert pvalue > 0.3  # It's not exactly uniform because of finite size of elements.
 
 def test_GAS_facets_on_radius():
     '''test distribution of elements on radius for d_r is non-integer multiple of d_element.'''
     myrowland = RowlandTorus(1000., 1000.)
-    gas = GratingArrayStructure(myrowland, 60., [1000., 2000.], [300., 400.], elem_class=mock_facet)
+    gas = GratingArrayStructure(rowland=myrowland, d_element=[60., 60.],
+                                radius=[300., 400.], elem_class=mock_facet)
     assert np.all(gas.distribute_elements_on_radius() == [320., 380.])
     gas.radius = [300., 340.]
     assert gas.distribute_elements_on_radius() == [320.]
 
 def test_facet_rotation_via_facetargs():
     '''The numbers for the blaze are not realistic.'''
     gratingeff = OrderSelector(np.arange(-3, 4))
     mytorus = RowlandTorus(9e3/2, 9e3/2)
-    mygas = GratingArrayStructure(mytorus, d_element=60., x_range=[5e3,1e4], radius=[538., 550.], elem_class=FlatGrating, elem_args={'zoom': 30, 'd':0.0002, 'order_selector': gratingeff})
+    mygas = GratingArrayStructure(rowland=mytorus, d_element=[60., 60.],
+                                  radius=[538., 550.], elem_class=FlatGrating,
+                                  elem_args={'zoom': 30, 'd':0.0002, 'order_selector': gratingeff})
     blaze = transforms3d.axangles.axangle2mat(np.array([0,1,0]), np.deg2rad(15.))
-    mygascat = GratingArrayStructure(mytorus, d_element=60., x_range=[5e3,1e4], radius=[538., 550.], elem_class=FlatGrating, elem_args={'zoom': 30, 'orientation': blaze, 'd':0.0002, 'order_selector': gratingeff})
+    mygascat = GratingArrayStructure(rowland=mytorus, d_element=[60., 60.],
+                                     radius=[538., 550.], elem_class=FlatGrating,
+                                     elem_args={'zoom': 30, 'orientation': blaze, 'd':0.0002, 'order_selector': gratingeff})
     assert np.allclose(np.rad2deg(np.arccos(np.dot(mygas.elements[0].geometry['e_x'][:3], mygascat.elements[0].geometry['e_x'][:3]))), 15.)
 
 def test_persistent_facetargs():
     '''Make sure that facet_args is still intact after generating facets.
 
     This is important to allow tweaks of a single parameter and then to regenerate the facets.
     '''
     gratingeff = OrderSelector(np.arange(-3, 4))
     mytorus = RowlandTorus(9e4/2, 9e4/2)
     # id_col is automatically added in GAS is not present here.
     # So, pass in an id_col to make sure the comparison below will still work.
     facet_args = {'zoom': 30, 'd':0.0002, 'order_selector': gratingeff, 'id_col': 'facet'}
-    mygas = GratingArrayStructure(mytorus, d_element=60., x_range=[5e4,1e5], radius=[5380., 5500.], elem_class=FlatGrating, elem_args=facet_args)
+    mygas = GratingArrayStructure(rowland=mytorus, d_element=[60., 60.],
+                                  radius=[5380., 5500.], elem_class=FlatGrating,
+                                  elem_args=facet_args)
     assert mygas.elem_args == facet_args
 
 def test_run_photons_through_gas():
     '''And check that they have the expected labels.
 
-    No need to check here that the grating equation works - that's part of the grating tests/
+    No need to check here that the grating equation works - that's part of the grating tests.
     '''
     # Setup only.
     mysource = PointSource(coords=SkyCoord(30., 30., unit="deg"))
     photons = mysource.generate_photons(1. * u.ks)
     mypointing = FixedPointing(coords=SkyCoord(30, 30., unit='deg'))
     photons = mypointing.process_photons(photons)
-    marxm = MarxMirror('./marxs/optics/hrma.par', position=np.array([0., 0, 0]))
+    marxm = MarxMirror(get_pkg_data_filename('hrma.par', package='marxs.optics'), position=np.array([0., 0, 0]))
     photons = marxm(photons)
     gratingeff = OrderSelector([-1, 0, 1])
     facet_args = {'zoom': 30, 'd':0.0002, 'order_selector': gratingeff}
     mytorus = RowlandTorus(9e3/2, 9e3/2)
 
     # Now the real test with different input for facet_args
 
@@ -323,104 +334,183 @@
             f = 'ttt'
             kwargs = {}
         elif i == 4:
             facet_args['id_col'] = 'uuu'
             f = 'uuu'
             kwargs = {'id_col': 'yyy'}
 
-        mygas = GratingArrayStructure(mytorus, d_element=60., x_range=[5e3,1e4], radius=[538., 550.], elem_class=FlatGrating, elem_args=facet_args, **kwargs)
+        mygas = GratingArrayStructure(rowland=mytorus, d_element=[60., 60.],
+                                      radius=[538., 550.], elem_class=FlatGrating,
+                                      elem_args=facet_args, **kwargs)
 
         p = mygas(photons.copy())
         indorder = np.isfinite(p['order'])
         indfacet = p[f] >=0
         assert np.all(indorder == indfacet)
 
         assert set(p['order'][indorder]) == set([-1, 0, 1])
         # -1 means no hit - passing between facets
         allfacets = set([-1]).union(set(np.arange(len(mygas.elements))))
         assert set(p[f]).issubset(allfacets)
 
-def test_LinearCCDArray():
-    '''Test an array in default position'''
-    myrowland = RowlandTorus(10000., 10000.)
-    # Along the way we normally would orient the detector.
-    ccds = LinearCCDArray(myrowland, d_element=30., x_range=[0., 2000.],
-                          radius=[-100., 100.], phi=0., elem_class=mock_facet)
-    assert len(ccds.elements) == 7
-    for e in ccds.elements:
-        # For this test we don't care if z and e_z are parallel or antiparallel
-        assert np.isclose(np.abs(np.dot([0, 0, 1, 0], e.geometry['e_z'])), 1.)
-        assert (e.pos4d[0, 3] >= 0) and (e.pos4d[0, 3] < 1.)
-
-    # center ccd is on the optical axis
-    assert np.allclose(ccds.elements[3].geometry['e_y'], [0, 1, 0, 0])
 
-def test_LinearCCDArray_rotatated():
+def test_RectangularGrid_rotated():
     '''Test an array with different rotations.
 
     In this case, we rotate the Rowland torus by -30 deg and then
     check that the e_z vector is rotated 30 deg with respect to the
     coordinate system.
     '''
     pos4d = transforms3d.axangles.axangle2aff([1, 0, 0], np.deg2rad(-30))
     myrowland = RowlandTorus(10000., 10000., pos4d=pos4d)
     # Along the way we normally would orient the detector.
-    ccds = LinearCCDArray(myrowland, d_element=30., x_range=[0., 2000.],
-                          radius=[-100., 100.], phi=0., elem_class=mock_facet)
+    ccds = RectangularGrid(rowland=myrowland, d_element=[30., 30.],
+                           y_range=[-100, 100],
+                           elem_class=mock_facet,
+                           guess_distance=100)
     assert len(ccds.elements) == 7
     for e in ccds.elements:
         assert np.isclose(np.dot([0, -0.8660254, 0.5], e.geometry['e_z'][:3]), 0, atol=1e-4)
 
-def test_impossible_LinearCCDArray():
-    '''The rotation is chosen such that all requested detector positions are
-    INSIDE the rowland torus
-    '''
-    pos4d = transforms3d.axangles.axangle2aff([1, 0, 0], np.deg2rad(-30))
-    myrowland = RowlandTorus(10000., 10000., pos4d=pos4d)
-    with pytest.raises(ElementPlacementError) as e:
-        ccds = LinearCCDArray(myrowland, d_element=30., x_range=[0., 2000.],
-                              radius=[-100., 100.], phi=np.deg2rad(30.), elem_class=mock_facet)
-    assert 'No intersection with Rowland' in str(e.value)
 
-def test_RowlandCircleArrayone():
+def test_RectangularGridone():
     '''Test an array of one element in default position'''
     myrowland = RowlandTorus(10000., 10000.)
     # Along the way we normally would orient the detector.
-    ccds = RowlandCircleArray(myrowland, d_element=300., theta=[np.pi - 0.0001, np.pi + 0.0001],
-                              elem_class=mock_facet)
+    ccds = RectangularGrid(rowland=myrowland, d_element=[300., 300.],
+                           y_range=[-1, 1],
+                           elem_class=mock_facet,
+                           guess_distance=25)
     assert len(ccds.elements) == 1
     # multiply because of pointing inward vs. outward
-    assert np.allclose(ccds.elements[0].pos4d, np.eye(4) * np.array([-1,-1,1,1]))
+    assert np.allclose(ccds.elements[0].pos4d, np.eye(4))
+
+
+def test_RegtangularGrid_offcenter_unaffected():
+    '''Make sure the coordinate system of the xyz_range is in global coordinates.
+    In this test, we check the z position, which in unchanged because the torus
+    center is moved only in the y direction.'''
+    R, r, pos4d = design_tilted_torus(5000, 0.07, 0.15)
+    rowland = RowlandTorus(R, r, pos4d=pos4d)
+    ccds = RectangularGrid(rowland=rowland, d_element=[5., 5.],
+                           z_range=[10, 20],
+                           y_range=[600, 615],
+                           elem_class=mock_facet,
+                           guess_distance=25)
+
+    for e in ccds.elements:
+        assert (e.geometry['center'][2] > 10) and (e.geometry['center'][2] < 20)
+
+
+def test_RegtangularGrid_offcenter_affected():
+    '''Make sure the coordinate system of the xyz_range is in global coordinates.
+    In this test, we check the y position.'''
+    R, r, pos4d = design_tilted_torus(50000, 0.007, 0.015)
+    rowland = RowlandTorus(R, r, pos4d=pos4d)
+    ccds = RectangularGrid(rowland=rowland, d_element=[50., 50.],
+                           y_range=[600, 800],
+                           elem_class=mock_facet,
+                           guess_distance=25)
+    y_offset = rowland.geometry['center'][1]
+    for e in ccds.elements:
+        assert (e.geometry['center'][1] > 600 + y_offset) and \
+               (e.geometry['center'][1] < 800 + y_offset)
 
-def test_compareRowlandCircle2LinearCCD_rotatated():
-    '''Test an array with different rotations.
 
-    The RowlandCircleArray and the LinearCCDArray should be very similar
-    for phi = 0.
-    '''
-    myrowland = RowlandTorus(10000., 10000.)
-    ccd1 = RowlandCircleArray(myrowland, d_element=30., theta=[np.pi - 0.03, np.pi],
-                              elem_class=mock_facet)
-    ccd2 = LinearCCDArray(myrowland, d_element=30., x_range=[0., 2000.],
-                          radius=[0., 10000. * np.sin(0.03)], phi=0., elem_class=mock_facet)
-    # reversed because the one element orders it differently then the other.
-    # Should really compare sets here or standardize order in some way, I guess.
-    for e1, e2 in zip(ccd1.elements, reversed(ccd2.elements)):
-        t1, r1, z1, s1 = transforms3d.affines.decompose44(e1.pos4d)
-        t2, r2, z2, s2 = transforms3d.affines.decompose44(e2.pos4d)
-        assert np.allclose(t1, t2, rtol=1e-3, atol=0.01)
-        # orientation is not too important, so allow some -1 factors
-        assert np.allclose(np.abs(r1), np.abs(r2), rtol=1e-3, atol=0.01)
 
 def test_nojumpsinCCDorientation():
     '''Regression test: CCD orientation should change smoothly along the circle.'''
     R, r, pos4d = design_tilted_torus(12e3, 0.07, 0.15)
     rowland = RowlandTorus(R, r, pos4d=pos4d)
-    det = RowlandCircleArray(rowland=rowland,
+    det = RectangularGrid(rowland=rowland,
                              elem_class=mock_facet,
-                             d_element=49.652, #theta=[np.pi - 0.2, np.pi + 0.5])
-                             theta=[np.pi - 0.2, np.pi - 0.1])
+                             d_element=[49.652, 49.652],
+                             y_range=[-200, +200],
+                             guess_distance=25.)
 
     # If all is right, this will vary very smoothly along the circle.
     xcomponent = np.array([e.geometry['e_y'][0] for e in det.elements])
     xcompdiff = np.diff(xcomponent)
     assert (np.max(np.abs(xcompdiff)) / np.median(np.abs(xcompdiff))) < 1.1
+
+
+def test_circularMeshGrid():
+    '''Check MeshGrid against a hand-checked and thus known-good solution'''
+    myrowland = RowlandTorus(10000., 10000.)
+    gas = CircularMeshGrid(rowland=myrowland,
+                           radius=(100., 300.),
+                           d_element=(30., 50),
+                           elem_class=mock_facet,
+                           optimize_axis=np.array([1, 0, 0, 0]),
+                           parallel_spec=np.array([0., 1., 0., 0.]),
+                           normal_spec=np.array([1, 0, 0, 1]))
+    assert len(gas.elements) == 178
+    poslist = np.stack(gas.elem_pos)
+    assert np.all(poslist[:, 0, 3] > 19000)
+    assert np.all(poslist[:, 0, 3] < 20000)
+    assert np.all(np.abs(poslist[:, 1, 3] < 300))
+    assert np.all(np.abs(poslist[:, 2, 3] < 300))
+
+def test_circularMeshGrid_rotated():
+    '''Check MeshGrid against a hand-checked and thus known-good solution.
+    Repeats previous test but for a different axes'''
+    myrowland = RowlandTorus(10000., 10000.)
+    myrowland.pos4d = xyz2zxy @ myrowland.pos4d
+    gas = CircularMeshGrid(rowland=myrowland,
+                           radius=(100., 300.),
+                           d_element=(30., 50),
+                           elem_class=mock_facet,
+                           optimize_axis=np.array([0, 0, 1, 0]),
+                           parallel_spec=np.array([0., 1., 0., 0.]),
+                           normal_spec=np.array([0, 1, 0, 1]))
+    assert len(gas.elements) == 178
+    poslist = np.stack(gas.elem_pos)
+    assert np.all(poslist[:, 2, 3] > 19000)
+    assert np.all(poslist[:, 2, 3] < 20000)
+    assert np.all(np.abs(poslist[:, 0, 3] < 300))
+    assert np.all(np.abs(poslist[:, 1, 3] < 300))
+
+
+def test_double_rowland_from_channel_distance():
+    '''Check that the double torus is in the right position.
+    The numbers are hand-checked and thus known-good.
+    '''
+    geom = double_rowland_from_channel_distance(600., 6000, 12000)
+    assert geom['pos_opt_ax']['1'] == pytest.approx([0, -300, 0, 1])
+    assert geom['pos_opt_ax']['1m'] == pytest.approx([0, 300, 0, 1])
+
+    assert geom['rowland_detector'].R == pytest.approx(6000)
+    assert geom['rowland_detector'].r == pytest.approx(6007.495318350236)
+    assert geom['rowland_central'].geometry['center'] == pytest.approx([7.48596673, 599.62570166, 0.,  1.])
+
+
+def test_offset_double_rowland_channels():
+    '''Split the double torus into two and offset all four channels.
+
+    Checked against the version of the code that's been in use for years
+    for Arcus.
+    '''
+    geom = double_rowland_from_channel_distance(600., 6000, 12000)
+    add_offset_double_rowland_channels(geom,
+                                   offsets={'1': [0, -2.5, -7.5],
+                                            '1m': [0, -2.5, -2.5],
+                                            '2': [0, 2.5, 2.5],
+                                            '2m': [0, 2.5, 12.5],
+                                            })
+    assert geom['pos_opt_ax']['2m'] == pytest.approx([0, 302.5, 12.5, 1. ])
+    assert geom['rowland_1'].geometry['center'] == pytest.approx([7.48596673, 297.12570166, -7.5, 1.])
+
+
+def test_rowlands_are_oriented_the_same_way():
+    """When there are two rowland tori, they should be oriented the same way."""
+    double = double_rowland_from_channel_distance(100, 500, 1000.0)
+    add_offset_double_rowland_channels(
+        double, offsets={"1": [0, -5, 0], "1m": [0, +5, 0]}
+    )
+    assert_allclose(
+        double["rowland_central"].parametric(0, 0),
+        double["rowland_central_m"].parametric(0, 0),
+    )
+    # The "top" points in the same direction. Of course, they are offset from each other
+    # so the numbers are not exactly the same.
+    assert_allclose(double["rowland_1"].parametric(0, 0), [1000.0, -55.0, 0.0, 1.0])
+    assert_allclose(double["rowland_1m"].parametric(0, 0), [1000.0, 55.0, 0.0, 1.0])
```

### Comparing `marxs-1.2/marxs/design/tests/test_tolerancing.py` & `marxs-2.0/marxs/design/tests/test_tolerancing.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,44 +4,46 @@
 import numpy as np
 import pytest
 import astropy.units as u
 from astropy.table import Table
 from astropy.coordinates import SkyCoord
 from astropy.utils.data import get_pkg_data_filename
 
-from ..tolerancing import (oneormoreelements,
-                           wiggle, moveglobal, moveindividual,
+from marxs.design.tolerancing import (oneormoreelements,
+                           wiggle, moveglobal, moveindividual, moveelem,
                            varyperiod, varyorderselector, varyattribute,
-                           run_tolerances, CaptureResAeff,
+                           run_tolerances,
                            generate_6d_wigglelist,
                            select_1dof_changed,
-                           plot_wiggle, load_and_plot,
+                           DispersedWigglePlotter,
                            run_tolerances_for_energies,
+                           run_tolerances_for_energies2,
                            )
-from ...optics import (FlatGrating, OrderSelector, RadialMirrorScatter,
+from marxs.optics import (FlatGrating, OrderSelector, RadialMirrorScatter,
                        RectangleAperture, ThinLens, FlatDetector)
 
-from ...design import RowlandTorus, GratingArrayStructure
-from ...utils import generate_test_photons
-from ...source import PointSource, FixedPointing
-from ...simulator import Sequence
+from marxs.design import RowlandTorus, GratingArrayStructure
+from marxs.utils import generate_test_photons
+from marxs.source import PointSource, FixedPointing
+from marxs.simulator import Sequence
+from marxs.analysis.gratings import CaptureResAeff
 
 try:
     import matplotlib.pyplot as plt
     HAS_MPL = True
 except ImportError:
     HAS_MPL = False
 
-
 mytorus = RowlandTorus(0.5, 0.5, position=[1.5, 0, -3])
 
-def gsa():
+def gsa(elem_class=FlatGrating):
     '''make a parallel structure - fresh for every test'''
-    g = GratingArrayStructure(mytorus, d_element=0.1, x_range=[0.5, 1.], radius=[0.1,.2],
-                              elem_class=FlatGrating,
+    g = GratingArrayStructure(rowland=mytorus,
+                              d_element=[0.1, 0.1], radius=[0.1,.2],
+                              elem_class=elem_class,
                               elem_args={'zoom':0.2, 'd':0.002,
                                          'order_selector': OrderSelector([1])
                                      })
     return g
 
 elempos = np.stack([e.pos4d for e in gsa().elements])
 
@@ -86,20 +88,23 @@
         assert not np.all(np.stack([e.pos4d for e in g.elements]) == elempos)
 
 
 def test_moveelements_translate():
     '''Check that the element movers work. If the whole structure is translated
     or individual elements are translated by the same amount, the positions
     should be the same.'''
+    g0 = gsa()
     g1 = gsa()
     g2 = gsa()
     moveglobal(g1, dy=-20)
     moveindividual(g2, dy=-20)
     assert np.allclose(np.stack([e.pos4d for e in g1.elements]),
                        np.stack([e.pos4d for e in g2.elements]))
+    assert not np.allclose(np.stack([e.pos4d for e in g0.elements]),
+                           np.stack([e.pos4d for e in g2.elements]))
 
 
 def test_moveelements_rotate():
     '''Check that the element movers work.
     Unlike test_moveelements_translate we expect different results because
     there are different center of the rotation.
     This test does not check that the rotation is correct, only that its
@@ -110,21 +115,30 @@
     g2 = gsa()
     moveglobal(g1, rz=-1, ry=.2)
     moveindividual(g2, rz=-1, ry=.2)
     assert not np.allclose(np.stack([e.pos4d for e in g1.elements]),
                            np.stack([e.pos4d for e in g2.elements]))
 
 
+def test_moveelem():
+    '''Move an individual element'''
+    det = FlatDetector(zoom=[1, 100, 100])
+    assert det.geometry['center'][2] == 0
+    moveelem(det, dz=5)
+    assert det.geometry['center'][2] == 5
+    assert np.all(det.geometry.pos4d[:3, :3] == np.eye(3) * [1, 100, 100])
+
+
 def test_wiggle():
     '''Check wiggle function'''
     g = gsa()
     wiggle(g, dx=10, dy=.1)
     diff = elempos - np.stack([e.pos4d for e in g.elements])
     # Given the numbers, wiggle in x must be larger than y
-    # This also tests that not all diff number are the same
+    # This also tests that not all diff numbers are the same
     # (as they would be with move).
     assert np.std(diff[:, 0, 3]) > np.std(diff[:, 1, 3])
 
 
 @pytest.mark.parametrize('function', [varyperiod, varyorderselector])
 def test_errormessage(function):
     '''Check that check is performed for right type of object.
@@ -170,15 +184,14 @@
         # Error should be raised before they are used, so the value does not
         # matter
         varyattribute(gsa, attributenotpresent=1., notpresenteither=2.)
 
     assert 'does not have' in str(e.value)
 
 
-
 def test_orderselector():
     '''Test setting the order selector properties.'''
     photons = generate_test_photons(5)
     grat = FlatGrating(d=1., order_selector=OrderSelector([1]))
     p = grat(photons.copy())
     assert np.all(p['order'] == 1)
 
@@ -209,18 +222,19 @@
     assert out[1]['orderlist'] == [1, 2]
     # check original parameter is still intact and can be used again
     # Regression test: If results are inserted into the same dict
     # 'meanorder' will appear which is not valid for varyorderselector
     assert 'meanorder' not in parameters[0]
 
 def test_run_tolerances_for_energies():
-    '''For this test, we need to define an instrument. The instrument is not very
-    realistic (an X-ray mirror with r=0 won't work), but the point here is just to
-    check the tolerancing for several energies. To make that calculation reasonably
-    fast, we need to keep the number of elements in the optical system small.
+    '''For this test, we need to define an instrument. The instrument is not
+    very realistic (an X-ray mirror with r=0 won't work), but the
+    point here is just to check the tolerancing for several
+    energies. To make that calculation reasonably fast, we need to
+    keep the number of elements in the optical system small.
     '''
     coords = SkyCoord(12. * u.deg, -45 * u.deg)
     src = PointSource(coords=coords)
     pnt = FixedPointing(coords=coords)
     aper = RectangleAperture(position=[5000, 0, 0], zoom=[1, 10, 10])
     lens = ThinLens(position=[4900, 0, 0], zoom=[1, 10, 10], focallength=4900)
     grat = FlatGrating(d=.002, order_selector=OrderSelector([0, 1]),
@@ -247,55 +261,49 @@
     assert .1 in res['energy']
     assert len(res) == 4
     # check results are reasonable
     assert np.all(res['R'].data[:, 0] == 0)
     assert not np.any(np.isfinite(res['R'].data[:, 2]))
     assert res['R'].data[2, 1] > res['R'].data[0, 1]
 
-def test_capture_res_aeff():
-    '''Test the captures res/aeff class.
 
-    Similar to the previous test, this is not a complete functional test,
-    but it checks the interfaces.
-    The actual function to calculate the effective area is tested elsewhere.
+def test_run_tolerances_for_energies2():
+    '''Same, as above, but with different calling sequence
     '''
-    p = generate_test_photons(200)
-    p['order'] = 0
-    p['order'][50:] = 5
-    p['xpos'] = -100
-    p['xpos'][50:] = np.random.normal(scale=1, size=150)
-
-    resaeff = CaptureResAeff(A_geom=10., order_col='order',
-                             orders=[0, 2, 5], dispersion_coord='xpos')
-    out = resaeff(p)
-    assert np.allclose(out['Aeff'], [2.5, 0., 7.5])
-    assert np.isclose(out['Aeff0'], 2.5)
-    assert np.isclose(out['Aeffgrat'], 7.5)
-    assert len(out['R']) == 3
-    assert np.isnan(out['R'][1])
+    coords = SkyCoord(12. * u.deg, -45 * u.deg)
+    src = PointSource(coords=coords)
+    pnt = FixedPointing(coords=coords)
+    aper = RectangleAperture(position=[5000, 0, 0], zoom=[1, 10, 10])
+    lens = ThinLens(position=[4900, 0, 0], zoom=[1, 10, 10], focallength=4900)
+    grat = FlatGrating(d=.002, order_selector=OrderSelector([0, 1]),
+                       position=[4800, 0, 0], zoom=[1, 10, 10])
+    det = FlatDetector(zoom=[1, 100, 100])
+    instrum = Sequence(elements=[pnt, aper, lens, grat, det])
 
-def test_capture_res_aeff_filter():
-    '''Ensure that photons with probability 0 will be ignored.
-    '''
-    p = generate_test_photons(200)
-    p['probability'] = 0
-    p['order'] = 0
-    p['order'][50:] = 5
-    p['xpos'] = -100
-    p['xpos'][50:] = np.random.normal(scale=1, size=150)
-
-    resaeff = CaptureResAeff(A_geom=10., order_col='order',
-                             orders=[0, 2, 5], dispersion_coord='xpos')
-    out = resaeff(p)
-    assert np.all(out['Aeff'] == 0)
-    assert out['Aeff0'] == 0
-    assert out['Aeffgrat'] == 0
-    assert len(out['R']) == 3
-    assert np.isnan(out['R'][2])
+    parameters = [{'period_mean': 0.003, 'period_sigma': 0.},
+                  {'period_mean': 0.004, 'period_sigma': 0.}]
 
+    res = run_tolerances_for_energies2(src, [.1, 1] * u.keV,
+                                       instrum, FlatGrating,
+                                       varyperiod,
+                                       parameters,
+                                       CaptureResAeff(orders=[0, 1, 2]),
+                                       reset={'period_mean': 0.005,
+                                              'period_sigma': 0.},
+                                       t_source=1. * u.ks)
+    # Check the reset worked
+    assert grat._d == 0.005
+    # Check both energy have been calculated
+    assert 1 in res['energy']
+    assert .1 in res['energy']
+    assert len(res) == 4
+    # check results are reasonable
+    assert np.all(res['R'].data[:, 0] == 0)
+    assert not np.any(np.isfinite(res['R'].data[:, 2]))
+    assert res['R'].data[2, 1] > res['R'].data[0, 1]
 
 
 def test_6dlist():
     '''Check the list of dicts in 3 translations dof and 3 rotations'''
     cglob, cind = generate_6d_wigglelist([0, 1.] * u.cm, [0., 1.] * u.degree,
                             names=['x', 'y', 'z', 'rx', 'ry', 'rz'])
     assert len(cind) == 7
@@ -323,60 +331,51 @@
     '''Test that we find the row where only one parameter was changed.'''
     tab = Table({'par1': [-1, -1, 0, 0, 0, 1],
                  'par2': [-1,  0, 0, 3, 0, 0],
                  'id':   [ 0,  1, 2, 3, 4, 5]})
     t = select_1dof_changed(tab, 'par1', parlist=['par1', 'par2'])
     assert set(t['id']) == set([1, 2, 4, 5])
 
-@pytest.mark.skipif('not HAS_MPL')
+
 def test_plot_wiggle():
     '''Test that wiggle plot works. This does not test that the result
     looks correct, only that running through the plot function does not
     raise any errors.
     This is one of the few plotting functions in the entire package, so
     setting up the infrastructure to compare output pixel-by-pixel does not
     seem worth it as this point.
     '''
+    plt = pytest.importorskip("matplotlib.pyplot")
     fig, ax = plt.subplots()
 
     tab = Table({'wave': [1, 1],
                  'dd': [0, 1],
                  'Rgrat': [500, 500],
                  'Aeff': [20, 50]})
-    plot_wiggle(tab, 'dd', ['dd'], ax, Aeff_col='Aeff')
-
-@pytest.mark.skipif('not HAS_MPL')
-def test_plot_wiggle_exception():
-    '''Test that exception is raised for parameters not plotted.
-    '''
-    fig, ax = plt.subplots()
-
-    tab = Table({'wave': [1, 1],
-                 'qwe': [0, 1],
-                 'Rgrat': [500, 500],
-                 'Aeff': [20, 50]})
-    with pytest.raises(ValueError, match='Parameter names should start with'):
-        plot_wiggle(tab, 'qwe', ['qwe'], ax, Aeff_col='Aeff')
+    wiggle_plotter = DispersedWigglePlotter()
+    wiggle_plotter.plot_wiggle(tab, 'dd', ['dd'], ax, Aeff_col='Aeff')
 
 @pytest.mark.skipif('not HAS_MPL')
 def test_plot_6dof():
 
     tab = Table({'wave': [1, 1, 2, 2, 1, 1, 1, 1],
                  'dd': [0, 1, 0, 2, 0, 0, 0, 0],
                  'rr': [0, 0, 0, 0, 2, 4, 6, 8],
                  'R': np.random.rand(8),
                  'Aeffgrat': np.arange(8)})
 
+    wiggle_plotter = DispersedWigglePlotter()
     with tempfile.TemporaryDirectory() as tmpdirname:
         name = os.path.join(tmpdirname, 'var_global.fits')
         tab.write(name)
-        fig, ax = load_and_plot(name, ['dd', 'rr'], R_col='R')
+        fig, ax = wiggle_plotter.load_and_plot(name, ['dd', 'rr'], R_col='R')
 
 @pytest.mark.skipif('not HAS_MPL')
 def test_plot_6dof_real_file():
     '''Repeat previous test with static data file. This is a more realistic file
     but it takes too long to generate every time. This file is used in the docs
     in design/tolerancing (see docs/pyplot/chandra_tolerancing) so if this test
     breaks, the docs will likely have to be changed, too.
     '''
+    wiggle_plotter = DispersedWigglePlotter()
     filename = get_pkg_data_filename('data/wiggle_global.fits', 'marxs.design.tests')
-    fig, ax = load_and_plot(filename)
+    fig, ax = wiggle_plotter.load_and_plot(filename)
```

### Comparing `marxs-1.2/marxs/design/tests/test_uncertainties.py` & `marxs-2.0/marxs/design/tests/test_uncertainties.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     Also, generating the GAS is a fairly expensive operation, so I do not want to
     make too many elements unless there is a good reason for it.
     '''
 
     np.random.seed(10)
 
     rowland  = RowlandTorus(5e3, 5e3)
-    gas = GratingArrayStructure(rowland, d_element=2., x_range=[9e3, 1.1e4],
+    gas = GratingArrayStructure(rowland=rowland, d_element=[2., 2.],
                                 radius=[2, 15], phi=[0, np.pi],
                                 elem_class=FlatGrating,
                                 elem_args={'d': 2e-4,
                                            'order_selector': OrderSelector([1])},
     )
     oldgaspos = deepcopy(gas.elem_pos)
     for a, b in zip(oldgaspos, gas.elements):
```

### Comparing `marxs-1.2/marxs/design/tolerancing.py` & `marxs-2.0/marxs/design/tolerancing.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,45 +1,42 @@
 # Licensed under GPL version 3 - see LICENSE.rst
-import inspect
 from functools import wraps
 import collections
 from copy import copy
 import warnings
 
 import numpy as np
 from transforms3d import affines, euler
 from astropy.table import Table
 from astropy import table
 import astropy.units as u
-from ..simulator import Parallel
-from .uncertainties import generate_facet_uncertainty as genfacun
-from ..analysis.gratings import (resolvingpower_from_photonlist,
-                                 effectivearea_from_photonlist)
-from ..analysis.gratings import AnalysisError
+from marxs.simulator import Sequence
+from marxs.design.uncertainties import generate_facet_uncertainty as genfacun
 
 __all__ = ['oneormoreelements',
-           'wiggle', 'moveglobal', 'moveindividual',
+           'wiggle', 'moveglobal', 'moveindividual', 'moveelem',
            'varyperiod', 'varyorderselector', 'varyattribute',
            'run_tolerances', 'run_tolerances_for_energies',
-           'CaptureResAeff',
            'generate_6d_wigglelist', 'reset_6d',
            'select_1dof_changed',
-           'plot_wiggle', 'load_and_plot',
+           'WigglePlotter',
+           'DispersedWigglePlotter',
            ]
 
+
 def oneormoreelements(func):
     '''Decorator for functions that modify optical elements.
 
     The functions in this module are written to work on a single optical
     element. This decorator allows them to accept a list of elements or
     a single element.
     '''
     @wraps(func)
     def func_wrapper(elements, *args, **kwargs):
-        if isinstance(elements, collections.Iterable):
+        if isinstance(elements, collections.abc.Iterable):
             for e in elements:
                 func(e, *args, **kwargs)
         else:
             func(elements, *args, **kwargs)
 
     return func_wrapper
 
@@ -51,15 +48,16 @@
     Parameters
     ----------
     e : `marxs.simulator.Parallel` or list of those elements
         Elements where uncertainties will be set
     dx, dy, dz : float
         accuracy of positioning in x, y, z (in mm) - Gaussian sigma, not FWHM!
     rx, ry, rz : float
-        accuracy of positioning. Rotation around x, y, z (in rad) - Gaussian sigma, not FWHM!
+        accuracy of positioning. Rotation around x, y, z (in rad) - Gaussian
+        sigma, not FWHM!
     '''
     e.elem_uncertainty = genfacun(len(e.elements), [dx, dy, dz], [rx, ry, rz])
     e.generate_elements()
 
 
 @oneormoreelements
 def moveglobal(e, dx=0, dy=0, dz=0, rx=0., ry=0., rz=0.):
@@ -102,14 +100,43 @@
     e.elem_uncertainty = [affines.compose((dx, dy, dz),
                                           euler.euler2mat(rx, ry, rz, 'sxyz'),
                                           np.ones(3))] * len(e.elements)
     e.generate_elements()
 
 
 @oneormoreelements
+def moveelem(e, dx=0, dy=0, dz=0, rx=0., ry=0., rz=0.):
+    '''Move and rotate a marxs element around principal axes.
+
+    Unlike `~marxs.design.tolerancing.moveglobal` this does not work on a
+    `~marxs.simulator.Parallel` object, which is a container holding other
+    elements, but it moves just one specific element itself (e.g. a single
+    detector).
+
+    To make it easier to return the element to its original position,
+    the original ``pos4d`` matrix of the element is stored as ``pos4d_orig``.
+
+    Parameters
+    ----------
+    e :`marxs.optics.base.OpticalElement` or list of those elements
+        Elements where uncertainties will be set
+    dx, dy, dz : float
+        translation in x, y, z (in mm)
+    rx, ry, rz : float
+        Rotation around x, y, z (in rad)
+    '''
+    if not hasattr(e.geometry, 'pos4d_orig'):
+        e.geometry.pos4d_orig = e.geometry.pos4d.copy()
+    move = affines.compose([dx, dy, dz],
+                           euler.euler2mat(rx, ry, rz, 'sxyz'),
+                           np.ones(3))
+    e.geometry.pos4d = move @ e.geometry.pos4d_orig
+
+
+@oneormoreelements
 def varyattribute(element, **kwargs):
     '''Modify the attributes of an element.
 
     This function modifies the attributes of an object. The keyword arguments
     are name and value of the attributes to be changed. This can be used for
     a wide variety of MARXS objects where the value of a parameter is stored
     as an instance attribute.
@@ -225,15 +252,15 @@
         contain all the parts of the instrument that the photons need to run
         though up to the detector.
     parameters : list of dicts
         List of parameter values for calls to `wigglefunc`.
     analyzefunc : callable function or object
         This is called with a photon table and should return a dictionary
         of results. This could be, e.g. a
-        `marxs.design.tolerancing.CaptureResAeff` instance.
+        `marxs.analysis.gratings.CaptureResAeff` instance.
 
 
     Returns
     -------
     result : list of dicts
         Each dict contains parameters and results for one run.
 
@@ -251,111 +278,25 @@
         cpars = copy(pars)
         cpars.update(analyzefunc(photons))
         out.append(cpars)
 
     return out
 
 
-class CaptureResAeff():
-    '''Capture resolving power and effective area for a tolerancing simulation.
-
-    Instances of this class can be called with a photon list for a tolerancing
-    simulation. The photon list will be analysed for resolving power and
-    effective area in a number of relevant orders.
-
-    This is implemented as a class and not a simple function. When the class is
-    initialized a number of parameters that are true for any to the
-    analysis (e.g. the names of certain columns) are set and saved in the class
-    instance.
-
-    The implementation of this class is geared towards instruments with
-    gratings but can also serve as an example how a complex analysis that
-    derives several different parameters can be implemented.
-
-    Results for effective area and resolving power are reported on a per order
-    basis and also summarized for all grating orders combined and the zeroth
-    order separately.
-
-    Parameters
-    ----------
-    A_geom : number
-        Geometric area of aperture for the simulations that this instance
-        will analyze.
-    order_col : string
-        Column names for grating orders
-    orders : array
-        Order numbers to consider in the analysis
-    dispersion_coord : string
-        Dispersion coordinate for
-        `marxs.analysis.gratings.resolvingpower_from_photonlist`
-
-    '''
-    def __init__(self, A_geom=1, order_col='order',
-                 orders=np.arange(-10, 11), dispersion_coord='det_x'):
-        self.A_geom = A_geom
-        self.order_col = order_col
-        self.orders = np.asanyarray(orders)
-        self.dispersion_coord = dispersion_coord
-
-    def __call__(self, photons):
-        '''Calculate Aeff and R for an input photon list.
-
-        Parameters
-        ----------
-        photons : `astropy.table.Table`
-            Photon list.
-
-        Returns
-        -------
-        result : dict
-            Dictionary with per-order Aeff and R, as well as values
-            summed over all grating orders.
-        '''
-        aeff = effectivearea_from_photonlist(photons, self.orders, len(photons),
-                                             self.A_geom, self.order_col)
-        try:
-            ind = (np.isfinite(photons[self.dispersion_coord]) &
-                   (photons['probability'] > 0))
-            res, pos, std = resolvingpower_from_photonlist(photons[ind], self.orders,
-                                                           col=self.dispersion_coord,
-                                                           zeropos=None,
-                                                           ordercol=self.order_col)
-        except AnalysisError:
-            # Something did not work, e.g. too few photons to find zeroth order
-            res = np.nan * np.ones(len(self.orders))
-
-        disporders = self.orders != 0
-        # The following lines work for an empty photon list, too.
-        aeffgrat = np.sum(aeff[disporders])
-        aeff0 = np.sum(aeff[~disporders])
-
-        # Division by 0 causes more nans, so filter those out
-        # Also, res is nan if less than 20 photons are detected
-        # so we need to filter those out, too.
-        ind = disporders & (aeff > 0) & np.isfinite(res)
-        if ind.sum() == 0:  # Dispersed spectrum misses detector
-            avggratres = np.nan
-        else:
-            avggratres = np.average(res[ind],
-                                    weights=aeff[ind] / aeff[ind].sum())
-        return {'Aeff0': aeff0, 'Aeffgrat': aeffgrat, 'Aeff': aeff,
-                'Rgrat': avggratres, 'R': res}
-
-
 def run_tolerances_for_energies(source, energies,
                                 instrum_before, instrum_remaining,
                                 wigglefunc, wiggleparts,
                                 parameters, analyzefunc,
-                                reset=None, t_source=1):
+                                reset=None, t_source=1 / u.s):
     '''Run tolerancing for a grid of parameters and energies
 
     This function loops over `~marxs.design.tolerancing.run_tolerances` for
     different energies.
     This function takes an instrument configuration and a function to change
-    one aspect of it. For every change it runs a simulations and calculates a
+    one aspect of it. For every change it runs simulations and calculates a
     figure of merit. As the name indicates, this function is designed to derive
     alignment tolerances for certain instrument parts but it might be general
     enough for other parameter studies in instrument design.
 
     There are two nested loops here looping over energy and tolerancing
     parameters. In this case, the outer loop is over energies and then for
     every energy, `~marxs.design.tolerancing.run_tolerances` loops over the
@@ -393,15 +334,15 @@
         description of these parameters.
     reset : dict or ``None``
         A dictionary of values for the ``wigglefunc`` function that resets
         the positions or properties of the wiggled elements to their default.
         If ``reset=None``, then the elements affected by ``wigglefunc`` will
         be in the state corresponding to the last entry in ``parameters`` when
         this function exits.
-    t_source : int
+    t_source : `astropy.units.quantity.Quantity`
         parameter for ``source.generate_photons()``. If the source flux is set
         to one, then ``t_source`` determines the number of photons used in the
         tolerancing simulation.
 
     Returns
     -------
     result : `astropy.table.Table`
@@ -430,14 +371,89 @@
     # Reset so that same instance of instrum can be used again
     if reset is not None:
         wigglefunc(wiggleparts, **reset)
 
     return table.vstack(outtabs)
 
 
+def run_tolerances_for_energies2(source, energies, instrum, cls, wigglefunc,
+                                 parameters,
+                                 analyzefunc, reset=None, subclass_ok=False,
+                                 t_source=1 / u.s):
+    '''Run tolerancing for a grid of parameters and energies
+
+    This function loops over `~marxs.design.tolerancing.run_tolerances` for
+    different energies.
+    This function takes an instrument configuration and a function to change
+    one aspect of it. For every change it runs a simulations and calculates a
+    figure of merit. As the name indicates, this function is designed to derive
+    alignment tolerances for certain instrument parts but it might be general
+    enough for other parameter studies in instrument design.
+
+    There are two nested loops here looping over energy and tolerancing
+    parameters. In this case, the outer loop is over energies and then for
+    every energy, `~marxs.design.tolerancing.run_tolerances` loops over the
+    parameters. This works well where running the ``wigglefunc`` is relatively
+    fast, but propagating the photons through ``instrum_before`` is slow and
+    minimizes the memory footprint, because only one photon list is in memory
+    at any one time. It also implies that runs for the same wiggle parameters
+    but different energies are run on different realizations of any random
+    draws that are performed by ``wigglefunc``.
+
+
+    Parameters
+    ----------
+    source : `marxs.source.Source`
+        Source used to generate the photons for every energy. This function
+        changes the energy of the source, so the source should be set for
+        monoenergetic emission with a constant flux of 1.
+    energies : `astropy.units.quantity.Quantity`
+        An array of energy values.
+    instrum : `marxs.simulator.Sequence`
+        An instance of the instrument which contains all elements.
+    cls : class
+        Class of modified / wiggled / etc. element
+    wigglefunc, parameters, analyzefunc :
+        These parameters are passed to
+        `marxs.design.tolerancing.run_tolerances`. See that function for a
+        description of these parameters.
+    reset : dict or ``None``
+        A dictionary of values for the ``wigglefunc`` function that resets
+        the positions or properties of the wiggled elements to their default.
+        If ``reset=None``, then the elements affected by ``wigglefunc`` will
+        be in the state corresponding to the last entry in ``parameters`` when
+        this function exits.
+    t_source : `astropy.units.quantity.Quantity`
+        parameter for ``source.generate_photons()``. If the source flux is set
+        to one, then ``t_source`` determines the number of photons used in the
+        tolerancing simulation.
+
+    Returns
+    -------
+    result : `astropy.table.Table`
+        Each row in the table contains energy, wave, parameter values, and
+        results from ``analyzefunc`` for a single run.
+
+    '''
+    ind = instrum.first_of_class_top_level(cls, subclass_ok)
+    if ind is None:
+        raise Exception(f'{cls} nor part of {instrum}')
+
+    tab = run_tolerances_for_energies(source, energies,
+                                      Sequence(elements=instrum.elements[:ind]),
+                                      Sequence(elements=instrum.elements[ind:]),
+                                      wigglefunc,
+                                      instrum.elements_of_class(cls),
+                                      parameters,
+                                      analyzefunc,
+                                      reset,
+                                      t_source=t_source)
+    return tab
+
+
 def generate_6d_wigglelist(trans, rot,
                            names=['dx', 'dy', 'dz', 'rx', 'ry', 'rz']):
     '''Generate a list of parameters for the wiggle functions in this module.
 
     This modules contains several wiggle functions such as
     `~marxs.design.tolerances.moveglobal` or
     `~marxs.design.tolerances.wiggle` that expect input for 6 degrees of
@@ -529,129 +545,164 @@
     pars = set(parlist)
     ind = np.ones(len(table), dtype=bool)
     for p in pars - set([par]):
         ind *= table[p] == 0
     return table[ind]
 
 
-def plot_wiggle(tab, par, parlist, ax, axt=None,
-                R_col='Rgrat', Aeff_col='Aeffgrat',
-                axes_facecolor='w'):
-    '''Plotting function for overview plot wiggeling 1 dof at the time.
+class WigglePlotter():
+    '''Object to plot results of tolerancing simulations
 
-    For parameters starting with "d" (e.g. "dx", "dy", "dz"), the plot axes
-    will be labeled as a shift, for parameters tarting with "r" as rotation.
+    This class combines the `load_and_plot` and `plot_wiggle` functions
+    with reasonable defaults for the plot appearance.
+    '''
+
+    ylabel = 'left label (solid lines)'
+    'Label for the left axis of the plot'
+
+    y2label = 'right label (dotted lines)'
+    'Label for the right axis of the plot'
+
+    bg_colors = {'global': '0.9',
+                 'individual': (1.0, 0.9, 0.9)}
+    '''Default background colors for wiggle overview plots.
+
+    If the key of the dict matches part of the filename, the color listed in
+    the dict is applied.
+    '''
 
-    Parameters
-    ----------
-    table : `astropy.table.Table`
-        Table with wiggle results
-    par : string
-        Name of parameter to be plotted
-    parlist : list of strings
-        Name of all parameters in ``table``
-    ax : `matplotlib.axes.Axes`
-        Axis object to plot into.
-    axt : ``None`` or  `matplotlib.axes.Axes`
-        If this is ``None``, twin axis are created to show resolving power
-        and effective area in one plot. Alternatively, a second axes instance
-        can be given here.
-    R_col : string
-        Column name in ``tab`` that hold the resolving power to be plotted.
-        Default is set to work with `marxs.design.tolerancing.CaptureResAeff`.
-    Aeff_col : string
-        Column name in ``tab`` that hold the effective area to be plotted.
-        Default is set to work with `marxs.design.tolerancing.CaptureResAeff`.
-    axes_facecolor : any matplotlib color specification
-        Color for the background in the plot.
-    '''
-    import matplotlib.pyplot as plt
-
-    t = select_1dof_changed(tab, par, parlist)
-    t.sort(par)
-    t_wave = t.group_by('wave')
-    if axt is None:
-        axt = ax.twinx()
 
-    for key, g in zip(t_wave.groups.keys, t_wave.groups):
+    def plot_wiggle(self, tab, par, parlist, ax, axt=None,
+                    axes_facecolor='w', **kwargs):
+        '''Plotting function for overview plot wiggeling 1 dof at the time.
+
+        For parameters starting with "d" (e.g. "dx", "dy", "dz"), the plot axes
+        will be labeled as a shift, for parameters tarting with "r" as rotation.
+
+        Parameters
+        ----------
+        table : `astropy.table.Table`
+            Table with wiggle results
+        par : string
+            Name of parameter to be plotted
+        parlist : list of strings
+            Name of all parameters in ``table``
+        ax : `matplotlib.axes.Axes`
+            Axis object to plot into.
+        axt : ``None`` or  `matplotlib.axes.Axes`
+            If this is ``None``, twin axis are created to show resolving power
+            and effective area in one plot. Alternatively, a second axes instance
+            can be given here.
+        R_col : string
+            Column name in ``tab`` that hold the resolving power to be plotted.
+            Default is set to work with `marxs.design.tolerancing.CaptureResAeff`.
+        Aeff_col : string
+            Column name in ``tab`` that hold the effective area to be plotted.
+            Default is set to work with `marxs.design.tolerancing.CaptureResAeff`.
+        axes_facecolor : any matplotlib color specification
+            Color for the background in the plot.
+        '''
+        t = select_1dof_changed(tab, par, parlist)
+        t.sort(par)
+        t_wave = t.group_by('wave')
+        axlist = [ax]
+
+        import matplotlib
+
+        match axt:
+            case None if self.y2label is not None:
+               axt = ax.twinx()
+               axlist.append(axt)
+            case matplotlib.axes.SubplotBase():
+                axlist.append(axt)
+
+        for key, g in zip(t_wave.groups.keys, t_wave.groups):
+            if par[0] == 'r':
+                x = np.rad2deg(g[par].data)
+            else:
+                x = g[par]
+
+            self.plot_one_line(ax, axt, key, g, x, **kwargs)
+        ax.set_ylabel(self.ylabel)
+        if len(axlist) > 1:
+            axt.set_ylabel(self.y2label)
         if par[0] == 'd':
-            x = g[par]
+            ax.set_xlabel('shift [mm]')
+            ax.set_title('Shift along {}'.format(par[1]))
         elif par[0] == 'r':
-            x = np.rad2deg(g[par].data)
+            ax.set_xlabel('Rotation [degree]')
+            ax.set_title('Rotation around {}'.format(par[1]))
         else:
-            raise ValueError("Don't know how to plot {}. Parameter names should start with 'd' for shifts and 'r' for rotations.".format(par))
+            ax.set_xlabel(par)
 
-        ax.plot(x, g[R_col], label='{:3.1f} $\AA$'.format(key[0]), lw=1.5)
-        axt.plot(x, g[Aeff_col], ':', label='{:2.0f} $\AA$'.format(key[0]), lw=2)
-    ax.set_ylabel('Resolving power (solid lines)')
-    axt.set_ylabel('$A_{eff}$ [cm$^2$] (dotted lines)')
-    if par[0] == 'd':
-        ax.set_xlabel('shift [mm]')
-        ax.set_title('Shift along {}'.format(par[1]))
-    elif par[0] == 'r':
-        ax.set_xlabel('Rotation [degree]')
-        ax.set_title('Rotation around {}'.format(par[1]))
-
-    for a in [ax, axt]:
-        a.set_facecolor(axes_facecolor)
-        a.set_axisbelow(True)
-        a.grid(axis='x', c='1.0', lw=2, ls='solid')
+        for a in axlist:
+            a.set_facecolor(axes_facecolor)
+            a.set_axisbelow(True)
+            a.grid(axis='x', c='1.0', lw=2, ls='solid')
+
+    def plot_one_line(self, ax, axt, key, g, x):
+        raise NotImplementedError
+
+    def load_and_plot(self, filename,
+                      parlist=['dx', 'dy', 'dz', 'rx', 'ry', 'rz'],
+                    **kwargs):
+        '''Load a table with wiggle results and make default plot
+
+        This is a function to generate a quicklook image with many
+        hardcoded defaults for figure size, colors etc.
+        In particular, this function is written for the display of
+        6d plots which vary 6 degrees of freedom, one at a time.
+
+        The color for the background in the plot is set depending on the filename
+        using the ``string : color`` assignments in
+        `~marxs.design.tolerancing.wiggle_plot_facecolors`. No fancy regexp based
+        match is applied, this is simply a check with ``in``.
 
+        Parameters
+        ----------
+        filename : string
+            Path to a file with data that can be plotted by
+            `~marxs.design.tolerancing.plot_wiggle`.
+
+        parlist : list of strings
+            Name of all parameters in ``table``.
+            This function only plots six of them.
 
-wiggle_plot_facecolors = {'global': '0.9',
-                          'individual': (1.0, 0.9, 0.9)}
-'''Default background colors for wiggle overview plots.
+        Returns
+        -------
+        tab : `astropy.table.Table`
+            Table of data read from ``filename``
+        fig : `matplotlib.figure.Figure`
+            Figure with plot.
+        kwargs :
+            All other parameters are passed to
+            `~marxs.design.tolerancing.plot_wiggle`.
+        '''
+        import matplotlib.pyplot as plt
 
-If the key of the dict matches part of the filename, the color listed in
-the dict is applied.
-'''
+        tab = Table.read(filename)
 
+        if 'axis_facecolor' not in kwargs:
+            for n, c in self.bg_colors.items():
+                if n in filename:
+                    kwargs['axes_facecolor'] = c
 
-def load_and_plot(filename, parlist=['dx', 'dy', 'dz', 'rx', 'ry', 'rz'], **kwargs):
-    '''Load a table with wiggle results and make default plot
+        fig = plt.figure(figsize=(12, 8))
+        fig.subplots_adjust(wspace=.6, hspace=.3)
+        for i, par in enumerate(parlist):
+            ax = fig.add_subplot(2, 3, i + 1)
+            self.plot_wiggle(tab, par, parlist, ax, **kwargs)
 
-    This is a function to generate a quicklook image with many
-    hardcoded defaults for figure size, colors etc.
-    In particular, this function is written for the display of
-    6d plots which vary 6 degrees of freedom, one at a time.
+        return tab, fig
 
-    The color for the background in the plot is set depending on the filename
-    using the ``string : color`` assignments in
-    `~marxs.design.tolerancing.wiggle_plot_facecolors`. No fancy regexp based
-    match is applied, this is simply a check with ``in``.
 
-    Parameters
-    ----------
-    filename : string
-        Path to a file with data that can be plotted by
-        `~marxs.design.tolerancing.plot_wiggle`.
+class DispersedWigglePlotter(WigglePlotter):
+    '''A wiggle plotter for gratings'''
 
-    parlist : list of strings
-        Name of all parameters in ``table``.
-        This function only plots six of them.
+    ylabel ='Resolving power (solid lines)'
+    y2label ='$A_{eff}$ [cm$^2$] (dotted lines)'
 
-    Returns
-    -------
-    tab : `astropy.table.Table`
-        Table of data read from ``filename``
-    fig : `matplotlib.figure.Figure`
-        Figure with plot.
-    kwargs :
-        All other parameters are passed to
-        `~marxs.design.tolerancing.plot_wiggle`.
-    '''
-    import matplotlib.pyplot as plt
-
-    tab = Table.read(filename)
-
-    if 'axis_facecolor' not in kwargs:
-        for n, c in wiggle_plot_facecolors.items():
-            if n in filename:
-                kwargs['axes_facecolor'] = c
-
-    fig = plt.figure(figsize=(12, 8))
-    fig.subplots_adjust(wspace=.6, hspace=.3)
-    for i, par in enumerate(parlist):
-        ax = fig.add_subplot(2, 3, i + 1)
-        plot_wiggle(tab, par, parlist, ax, **kwargs)
+    def plot_one_line(self, ax, axt, key, g, x,
+                      R_col='Rgrat', Aeff_col='Aeffgrat'):
+        ax.plot(x, g[R_col], label='{:3.1f} $\AA$'.format(key[0]), lw=1.5)
+        axt.plot(x, g[Aeff_col], ':', label='{:2.0f} $\AA$'.format(key[0]), lw=2)
 
-    return tab, fig
```

### Comparing `marxs-1.2/marxs/design/uncertainties.py` & `marxs-2.0/marxs/design/uncertainties.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 from transforms3d import affines, euler
 
 __all__ = ['generate_facet_uncertainty']
 
-def generate_facet_uncertainty(n, xyz, angle_xyz):
+
+def generate_facet_uncertainty(n, xyz, angle_xyz,
+                               trans_offset=0, rot_offset=0):
     '''Generate 4d matrices that represent facet misalignment.
 
     Positional and rotational uncertainties are input to this function. It then
     draws randomnly from Gaussians centered on 0 (the correct position) for the displacement
     and rotation, where the :math:`\sigma` of the Gaussian is given by the numbers in the input.
     The linear displacements and angles are expressed as (4,4) matrixes suitable for use with
     homogeneous coordinates.
@@ -17,17 +19,21 @@
     ----------
     n : int
         Number of 4d matrixes to be calculated
     xyz : tuple of 3 floats
         accuracy of grating positioning in x, y, z (in mm) - Gaussian sigma, not FWHM!
     angle_xyz : tuple of 3 floats
         accuracy of grating positioning. Rotation around x, y, z (in rad) - Gaussian sigma, not FWHM!
+    trans_offset : array_like
+        will be passed to `numpy.random.normal` as the ``loc`` parameter when drawing translantions.
+    rot_offset : array_like
+        will be passed to `numpy.random.normal` as the ``loc`` parameter when drawing rotations.
 
     Returns
     -------
     pos_uncert : list of n (4,4) np.arrays
         Random realizations of the uncertainty
     '''
-    translation = np.random.normal(size=(n, 3)) * np.asanyarray(xyz)[np.newaxis, :]
-    rotation = np.random.normal(size=(n, 3)) * np.asanyarray(angle_xyz)[np.newaxis, :]
+    translation = np.random.normal(size=(n, 3), loc=trans_offset, scale=xyz)
+    rotation = np.random.normal(size=(n, 3), loc=rot_offset, scale=angle_xyz)
     return [affines.compose(t, euler.euler2mat(a[0], a[1], a[2], 'sxyz'), np.ones(3))
-            for t, a in zip(translation, rotation)]
+            for t, a in zip(translation, rotation)]
```

### Comparing `marxs-1.2/marxs/math/geometry.py` & `marxs-2.0/marxs/math/geometry.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,37 +38,40 @@
     box = h2e(g['center']) + r_factor * np.vstack([h2e( g['v_y']) + h2e(g['v_z']),
                                                    h2e(-g['v_y']) + h2e(g['v_z']),
                                                    h2e(-g['v_y']) - h2e(g['v_z']),
                                                    h2e( g['v_y']) - h2e(g['v_z'])
                                                ])
     return box
 
+
 def xyz_circle(geometry, r_factor=1, philim=[0, 2 * np.pi], n_vertices=90):
     '''Generate Eukledian positions along an ellipse.
 
-    The circle is centered on the center of the object and the semi-major
-    and minor axes are given by ``v_y`` and ``v_z``. Note that this function
-    is usually used to generate circle position, although ellipses are possible,
-    thus the name.
-
-    The circle (or ellipse) is approximated by a polygon with ``n_vertices``
-    vertices, where the value of ``n_vertices`` is taken from the ``self.display``
-    dictionary.
+    The circle is centered on the center of the object and the
+    semi-major and minor axes are given by ``v_y`` and ``v_z``. Note
+    that this function is usually used to generate circle position,
+    although ellipses are possible, thus the name.
+
+    The circle (or ellipse) is approximated by a polygon with
+    ``n_vertices`` vertices, where the value of ``n_vertices`` is
+    taken from the ``self.display`` dictionary.
 
     Parameters
     ----------
     r_factor : float
         Scaling factor for the square.
     phi_lim : list
-        Lower and upper limit for the angle phi to restrict the circle to a wedge.
+        Lower and upper limit for the angle phi to restrict the circle to a
+        wedge.
 
     Returns
     -------
     circle : np.array of shape (n, 3)
         Eukledian coordinates of the corners of the square in 3d space.
+
     '''
     n = n_vertices
     phi = np.linspace(0.5 * np.pi, 2.5 * np.pi, n, endpoint=False)
     v_y = r_factor * geometry['v_y']
     v_z = r_factor * geometry['v_z']
 
     x = np.cos(phi)
@@ -94,23 +97,24 @@
 
 class Geometry(NoGeometry):
 
     n_points = 50
 
     def __init__(self, kwargs={}):
         self.pos4d = _parse_position_keywords(kwargs)
-        #copy class attribute to instance attribute
+        # copy class attribute to instance attribute
         self._geometry = copy(self._geometry)
-        super(Geometry, self).__init__(kwargs=kwargs)
+        super().__init__(kwargs=kwargs)
 
     def __getitem__(self, key):
         '''This function wraps access to the pos4d matrix.
 
-        This is mostly a convenience method that gives access to vectors from the
-        ``pos4d`` matrix in familiar terms with string labels:
+        This is mostly a convenience method that gives access to
+        vectors from the ``pos4d`` matrix in familiar terms with
+        string labels:
 
         - ``center``: The ``center`` is the origin of the local coordiante system
           of the optical elemement. Typically, if will be the center of the
           active plane, e.g. the center of the mirror surface.
         - :math:`\hat v_{y,z}`: The box stretches in the y and z direction for
           :math:`\pm \hat v_y` and :math:`\pm \hat v_z`. In optics, the relevant
           interaction often happens on a surface, e.g. the surface of a mirror or
@@ -129,14 +133,15 @@
           as ``plane``.
         - Other labels get looked up in ``self._geometry`` and if the resulting
           value is a 4-d vector, it gets transformed with ``pos4d``.
 
         Not all these labels make sense for every optical element (e.g. a curved
         mirror does not really have a "plane").
         Access through this method is slower than direct indexing of ``self.pos4d``.
+
         '''
 
         if key == 'center':
             return self.pos4d[:, 3]
         elif key in ['v_x', 'e_x']:
             val = self.pos4d[:, 0]
         elif key in ['v_y', 'e_y']:
@@ -178,33 +183,34 @@
 
     def get_local_euklid_bases(self, interpos_local):
         '''Obtain a local eukledian base at a set of positions.
 
         Parameters
         ----------
         interpos_local : `numpy.ndarray` of shape (N, 2)
-            coordinates in the coordiante system of the geometry (e.g. (x, y), or
-            (r, phi)).
+            coordinates in the coordiante system of the geometry (e.g. (x, y),
+            or (r, phi)).
 
         Returns
         -------
         e_1, e_2, n : `numpy.ndarray` of shape (N, 4)
             Vectors pointing in direction 1, 2, and normal to the surface.
         '''
         raise NotImplementedError
 
+
 class FinitePlane(Geometry):
     '''Base class for geometrically flat optical elements.
 
     '''
 
     shape = 'box'
 
     loc_coos_name = ['y', 'z']
-    '''name for output columns that contain the interaction point in local coordinates.'''
+    '''name for output columns with interaction point in local coordinates.'''
 
     def intersect(self, dir, pos):
         '''Calculate the intersection point between a ray and the element
 
         Parameters
         ----------
         dir : `numpy.ndarray` of shape (N, 4)
@@ -256,16 +262,15 @@
 
     def get_local_euklid_bases(self, interpos_local):
         '''Obtain a local eukledian base at a set of positions.
 
         Parameters
         ----------
         interpos_local : `numpy.ndarray` of shape (N, 2)
-            coordinates in the coordiante system of the geometry (e.g. (x, y), or
-            (r, phi)).
+            coordinates in the coordiante system of the geometry (x, y)
 
         Returns
         -------
         e_1, e_2, n : `numpy.ndarray` of shape (N, 4)
             Vectors pointing in direction 1, 2, and normal to the surface.
         '''
 
@@ -274,27 +279,27 @@
         y = np.tile(self['e_y'], (n, 1))
         z = np.tile(self['e_z'], (n, 1))
         return y, z, x
 
 
 class PlaneWithHole(FinitePlane):
 
-    shape='triangulation'
+    shape = 'triangulation'
     outer_factor = 3
     inner_factor = 0
 
     def __init__(self, kwargs):
         self._geometry['r_inner'] = kwargs.pop('r_inner', 0.)
-        super(PlaneWithHole, self).__init__(kwargs)
+        super().__init__(kwargs)
 
     def triangulate(self, display={}):
         '''Return a triangulation of the aperture hole embedded in a square.
 
-        The size of the outer square is determined by the ``'outer_factor'`` element
-        in ``self.display``.
+        The size of the outer square is determined by the ``'outer_factor'``
+        element in ``self.display``.
 
         Returns
         -------
         xyz : np.array
             Numpy array of vertex positions in Eukeldian space
         triangles : np.array
             Array of index numbers that define triangles
@@ -344,34 +349,36 @@
             raise ValueError('Input angles >> 2 pi. Did you use degrees (radian expected)?')
         if phi[0] > phi[1]:
             raise ValueError('phi[1] must be greater than phi[0].')
         if (phi[1] - phi[0]) > (2 * np.pi + 1e-6):
             raise ValueError('phi[1] - phi[0] must be less than 2 pi.')
         self.phi = phi
 
-        super(CircularHole, self).__init__(kwargs)
+        super().__init__(kwargs)
 
     def outer_display(self, display):
         '''Return values in Eukledian space.'''
         return xyz_circle(self, r_factor=display['outer_factor'])
 
     def outer_shape(self, display):
         return xyz_circle(self, r_factor=1, philim=self.phi)
 
     def inner_shape(self, display):
         return xyz_circle(self,
                           r_factor=self['r_inner']/np.linalg.norm(self['v_y']),
                           philim=self.phi)
+
     def inner_display(self, display):
         # Inner edge of the display. If we have several stacked apertures,
         # we don't want to fill is all up to r=0.
         return xyz_circle(self,
                           r_factor=display['inner_factor'] * self['r_inner'] / np.linalg.norm(self['v_y']),
                           philim=self.phi)
 
+
 class Cylinder(Geometry):
     '''A Geometry shaped like a ring or tube.
 
     This object is shaped like a tube. The form is a circle in the xy plane
     and flat along the z-direction.  This can be used, for example to
     simulate a setup that can follow the Rowland circle
     geometry exactly which is useful, e.g. to study the resolution of a
@@ -407,22 +414,22 @@
     #         if (v < -np.pi) or (v > np.pi):
     #             raise ValueError('phi_lim must be in range -pi to +pi.')
     #     self.coos_limits[0] = value
 
     def __init__(self, kwargs={}):
         self.coos_limits = deepcopy(self.coos_limits)
         self.coos_limits[0] = np.asanyarray(kwargs.pop('phi_lim', [-np.pi, np.pi]))
-        super(Cylinder, self).__init__(kwargs)
+        super().__init__(kwargs)
 
     def __getitem__(self, value):
         if value == 'R':
             trans, rot, zoom, shear = decompose44(self.pos4d)
             return zoom[0]
         else:
-            return super(Cylinder, self).__getitem__(value)
+            return super().__getitem__(value)
 
     @classmethod
     def from_rowland(cls, rowland, width, rotation=0., kwargs={}):
         '''Generate a `Cylinder` from a `RowlandTorus`.
 
         According to the definition of the `marxs.design.rowland.RowlandTorus`
         the origin phi=0 is at the "top". When this class method is used to
@@ -442,61 +449,63 @@
             Rotation angle of the Cylinder around its z-axis compared to the
             phi=0 position of the Rowland torus.
 
         '''
         # Step 1: Rotate around z axis
         rot = axangle2mat(np.array([0, 0, 1.]), rotation)
         # Step 2: Get position and size from Rowland torus
-        pos4d_circ = compose([rowland.R, 0, 0], rot, [rowland.r, rowland.r, width])
+        pos4d_circ = compose([rowland.R, 0, 0], rot,
+                             [rowland.r, rowland.r, width])
         # Step 3: Transform to global coordinate system
         pos4d_circ = np.dot(rowland.pos4d, pos4d_circ)
         # Step 4: Make detector
         det_kwargs = {'pos4d': pos4d_circ}
         det_kwargs.update(kwargs)
         return cls(det_kwargs)
 
-
     def intersect(self, dir, pos, transform=True):
         '''Calculate the intersection point between a ray and the element
 
         Parameters
         ----------
         dir : `numpy.ndarray` of shape (N, 4)
             homogeneous coordinates of the direction of the ray
         pos : `numpy.ndarray` of shape (N, 4)
             homogeneous coordinates of a point on the ray
         transform : bool
-            If ``True``, input is in global coordinates and needs to be transformed
-            here for the calculations; if ``False`` input is in local coordinates.
+            If ``True``, input is in global coordinates and needs to be
+            transformed here for the calculations; if ``False`` input is in
+            local coordinates.
 
         Returns
         -------
         intersect :  boolean array of length N
             ``True`` if an intersection point is found.
         interpos : `numpy.ndarray` of shape (N, 4)
             homogeneous coordinates of the intersection point. Values are set
             to ``np.nan`` is no intersecton point is found.
         interpos_local : `numpy.ndarray` of shape (N, 2)
-            phi, z coordiantes (in the local frame) for one of the intersection points.
-            If both intersection points are required, reset ``self.inner`` and call this
-            function again.
+            phi, z coordiantes (in the local frame) for one of the intersection
+            points. If both intersection points are required, reset
+            ``self.inner`` and call this function again.
         '''
         # This could be moved to a general function
         if not np.all(dir[:, 3] == 0):
             raise ValueError('First input must be direction vectors.')
         # Could test pos, too...
         if transform:
             invpos4d = np.linalg.inv(self.pos4d)
             dir = np.dot(invpos4d, dir.T).T
             pos = np.dot(invpos4d, pos.T).T
 
         xyz = h2e(pos)
         dir_e = h2e(dir)
 
-        # Solve quadratic equation in steps. a12 = (-xr +- sqrt(xr - r**2(x**2 - R**2)))
+        # Solve quadratic equation in steps.
+        # a12 = (-xr +- sqrt(xr - r**2(x**2 - R**2)))
         xy = xyz[:, :2]
         r = dir[:, :2]
         c = np.sum(xy**2, axis=1) - 1.
         b = 2 * np.sum(xy * r, axis=1)
         a = np.sum(r**2, axis=1)
         underroot = b**2 - 4 * a * c
         # List of intersect in xy plane.
@@ -517,61 +526,64 @@
             phi_1 = np.arctan2(xy_1[:, 1], xy_1[:, 0])
             xy_2 = xy[i, :] + a2[:, np.newaxis] * r[i, :]
             phi_2 = np.arctan2(xy_2[:, 1], xy_2[:, 0])
             # 1, 2 look like hits in x,y but might still miss in z
             z_1 = xyz[i, 2] + a1 * dir[i, 2]
             z_2 = xyz[i, 2] + a2 * dir[i, 2]
             hit_1 = ((a1 >= 0) & (np.abs(z_1) <= 1.) &
-                     angle_between(phi_1, self.coos_limits[0][0], self.coos_limits[0][1]))
+                     angle_between(phi_1, self.coos_limits[0][0],
+                                   self.coos_limits[0][1]))
             hit_2 = ((a2 >= 0) & (np.abs(z_2) <= 1.) &
-                     angle_between(phi_2, self.coos_limits[0][0], self.coos_limits[0][1]))
+                     angle_between(phi_2, self.coos_limits[0][0],
+                                   self.coos_limits[0][1]))
             # If both 1 and 2 are hits, use the closer one
             hit_1[hit_2 & (a2 < a1)] = False
             hit_2[hit_1 & (a2 >= a1)] = False
             intersect[i_ind] = hit_1 | hit_2
             # Set values into array from either point 1 or 2
             interpos_local[i_ind[hit_1], 0] = phi_1[hit_1]
             interpos_local[i_ind[hit_1], 1] = z_1[hit_1]
 
             interpos_local[i_ind[hit_2], 0] = phi_2[hit_2]
             interpos_local[i_ind[hit_2], 1] = z_2[hit_2]
             # Calculate pos for point 1 or 2 in local xyz coord system
             interpos[i_ind[hit_1], :] = e2h(xyz[i_ind, :] + a1[:, None] * dir_e[i_ind, :], 1)[hit_1, :]
             interpos[i_ind[hit_2], :] = e2h(xyz[i_ind, :] + a2[:, None] * dir_e[i_ind, :], 1)[hit_2, :]
 
-
             trans, rot, zoom, shear = decompose44(self.pos4d)
             # interpos_local in z direction is in local coordinates, i.e.
             # the x coordiante is 0..1, but we want that in units of the
             # global coordinate system.
             interpos_local[:, 1] = interpos_local[:, 1] * zoom[2]
             interpos = np.dot(self.pos4d, interpos.T).T
 
         return intersect, interpos, interpos_local
 
-
     def parametric_surface(self, phi=None, z=None, display={}):
         '''Parametric description of the tube.
 
         This is just another way to obtain the shape of the tube, e.g.
         for visualization.
 
         Parameters
         ----------
         phi : np.array
-            ``phi`` is the angle around the tube profile. Set to ``None`` to use the
-            extend of the element itself.
+            ``phi`` is the angle around the tube profile. Set to ``None`` to
+            use the extend of the element itself.
         z : np.array
-            The coordiantes along the radius coordinate. Set to ``None`` to use the
-            extend of the element itself.
+            The coordiantes along the radius coordinate. Set to ``None`` to use
+            the extend of the element itself.
 
         Returns
         -------
         xyzw : np.array
             Ring coordinates in global homogeneous coordinate system.
+            The array has the following shape (npoints, 2, 4). 
+            `xyzw[:, 0, :]` describes one rim of the cylinder, `xyzw[:, 1, :]`
+            the other rim.
         '''
         phi = np.linspace(self.coos_limits[0][0], self.coos_limits[0][1], self.n_points) \
               if phi is None else np.asanyarray(phi)
         trans, rot, zoom, shear = decompose44(self.pos4d)
         z = self.coos_limits[1] if z is None else np.asanyarray(z) / zoom[2]
         if (phi.ndim != 1) or (z.ndim != 1):
             raise ValueError('input parameters have 1-dim shape.')
@@ -584,16 +596,16 @@
 
     def get_local_euklid_bases(self, interpos_local):
         '''Obtain a local eukledian base at a set of positions.
 
         Parameters
         ----------
         interpos_local : `numpy.ndarray` of shape (N, 2)
-            coordinates in the coordiante system of the geometry (e.g. (x, y), or
-            (r, phi)).
+            coordinates in the coordiante system of the geometry (e.g. (x, y),
+            or (r, phi)).
 
         Returns
         -------
         e_1, e_2, n : `numpy.ndarray` of shape (N, 4)
             Vectors pointing in direction 1, 2, and normal to the surface.
         '''
```

### Comparing `marxs-1.2/marxs/math/pluecker.py` & `marxs-2.0/marxs/math/pluecker.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/polarization.py` & `marxs-2.0/marxs/math/polarization.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 import astropy.units as u
-from numpy.core.umath_tests import inner1d
 
 from .utils import norm_vector, e2h
 
 
 __all__ = ['polarization_vectors', 'Q_reflection', 'paralleltransport_matrix',
            'parallel_transport']
```

### Comparing `marxs-1.2/marxs/math/random.py` & `marxs-2.0/marxs/math/random.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/rotations.py` & `marxs-2.0/marxs/math/rotations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 from transforms3d.utils import normalized_vector
 
 __all__ = ['ex2vec_fix', 'axangle2mat']
 
+
 def ex2vec_fix(e1, efix):
     '''Rotate x-axis to e1, use efix to break rotation ambiguity.
 
-    This function calcalates the rotation matrix that rotates the x-axis to
+    This function calculates the rotation matrix that rotates the x-axis to
     ``e1``, i.e. it rotates the normal of the y,z-plane to a new plane where
     ``e1`` is the normal. This still leaves the rotation angle of the plane
     free. This function breaks the degeneracy by keeping a vector that is
     coplanar with the normal and fix coplanar with fix and the new normal.
 
     The purpose of this function is best explained by an example:
     Imagine a plane in the y, z plane. We want to rotate the plane, such that ``e1``
```

### Comparing `marxs-1.2/marxs/math/tests/test_geometry.py` & `marxs-2.0/marxs/math/tests/test_geometry.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,97 +1,100 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
-from numpy.core.umath_tests import inner1d
 import transforms3d
 import transforms3d.euler
 import pytest
 
 from ..geometry import Cylinder, FinitePlane
 from ...math.utils import h2e
 
 
 def test_intersect_plane_forwards():
 
     pos = np.array([[20., 0., 0.8, 1.],  # start above
-                    [0., .0, 0.4, 1.],  # start inside
-                    [-5., .1, -.2, 1]]) # start below
+                    [0., .0, 0.4, 1.],   # start inside
+                    [-5., .1, -.2, 1]])  # start below
     dir = np.array([[-.1, 0., 0., 0],
                     [-1., 0, 0.02, 0.],
                     [-2., -0.02, 0.023, 0.]])
 
     plane = FinitePlane()
     intersect, interpos, inter_local = plane.intersect(dir, pos)
     assert np.all(intersect == [True, True, False])
     intersect, interpos, inter_local = plane.intersect(-dir, pos)
     assert np.all(intersect == [False, True, True])
 
+
 def test_intersect_plane_zoomed():
     pos = np.array([[1., 4., 0.8, 1.],
                     [1., -4., 8., 1.],
                     [1., -6., -8., 1]])
     dir = np.array([[-.1, 0., 0., 0],
                     [-1., 0, 0.02, 0.],
                     [-2., -0.02, 0.023, 0.]])
 
     plane = FinitePlane({'zoom': [1, 5, 10]})
     intersect, interpos, inter_local = plane.intersect(dir, pos)
     assert np.all(intersect == [True, True, False])
     assert np.all(interpos[0, :] == [0, 4, .8, 1])
     assert np.all(inter_local[0, ] == [4, .8])
 
+
 def test_intersect_plane_moved():
 
     pos = np.array([[4.1, 5.5, 6.8, 1.],
                     [5., 4.1, 4.99, 1.],
                     [4.1, 3., 6., 1]])
     dir = np.array([[-.1, 0., 0., 0],
                     [-1., 0, 0.02, 0.],
                     [-2., -0.02, 0.023, 0.]])
 
-    plane = FinitePlane({'position': [4,5,6]})
+    plane = FinitePlane({'position': [4, 5, 6]})
     intersect, interpos, inter_local = plane.intersect(dir, pos)
     assert np.all(intersect == [True, True, False])
     assert np.all(interpos[1, :] == [4, 4.1, 5.01, 1])
     assert np.allclose(inter_local[1, :], [-0.9, -.99])
 
+
 def test_intersect_tube_miss():
     '''Rays passing at larger radius or through the center miss the tube.'''
     circ = Cylinder()
     # Passing at larger radius
-    intersect, interpos, inter_local = circ.intersect(np.array([[1., 0., .1, 0],
-                                                                [-1., -1., 0., 0.]]),
-                                                         np.array([[0, -1.1, 0., 1.],
-                                                                   [2., 0., 0., 1.]]))
-    assert np.all(intersect == False)
-    assert np.all(np.isnan(interpos))
-    assert np.all(np.isnan(inter_local))
+    sect, pos, local = circ.intersect(np.array([[1., 0., .1, 0],
+                                                [-1., -1., 0., 0.]]),
+                                      np.array([[0, -1.1, 0., 1.],
+                                                [2., 0., 0., 1.]]))
+    assert np.all(~sect)
+    assert np.all(np.isnan(pos))
+    assert np.all(np.isnan(local))
 
     # Through the center almost parallel to z-axis
-    intersect, interpos, inter_local = circ.intersect(np.array([[0., 0.1, 1., 0]]),
-                                                         np.array([[0.5, 0.5, 0., 1.]]))
-    assert np.all(intersect == False)
-    assert np.all(np.isnan(interpos))
-    assert np.all(np.isnan(inter_local))
+    sect, pos, local = circ.intersect(np.array([[0., 0.1, 1., 0]]),
+                                      np.array([[0.5, 0.5, 0., 1.]]))
+    assert np.all(~sect)
+    assert np.all(np.isnan(pos))
+    assert np.all(np.isnan(local))
 
     # Repeat with a tube that's moved to make sure we did not mess up local and
     # global coordinates in the implementation
     circ = Cylinder({'position': [0.8, 0.8, 1.2]})
-    intersect, interpos, inter_local = circ.intersect(np.array([[1., 0., .0, 0],
-                                                                [1., 0., 0., 0.]]),
-                                                         np.array([[0., 0., 0., 1.],
-                                                                   [0., -0.3, 1., 1.]]))
-    assert np.all(intersect == False)
-    assert np.all(np.isnan(interpos))
-    assert np.all(np.isnan(inter_local))
+    sect, pos, local = circ.intersect(np.array([[1., 0., .0, 0],
+                                                [1., 0., 0., 0.]]),
+                                      np.array([[0., 0., 0., 1.],
+                                                [0., -0.3, 1., 1.]]))
+    assert np.all(~sect)
+    assert np.all(np.isnan(pos))
+    assert np.all(np.isnan(local))
+
 
 def test_intersect_tube_rays_forward():
     '''Rays only intersect if propagating them forward works'''
     pos = np.array([[20., 0., 0.8, 1.],  # start above
-                    [0., .0, 0.4, 1.],  # start inside
-                    [-5., .1, -.2, 1]]) # start below
+                    [0., .0, 0.4, 1.],   # start inside
+                    [-5., .1, -.2, 1]])  # start below
     dir = np.array([[-.1, 0., 0., 0],
                     [-1., 0, 0.02, 0.],
                     [-2., -0.02, 0.023, 0.]])
 
     circ = Cylinder({'zoom': [1, 1, 1]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
     assert np.all(intersect == [True, True, False])
@@ -102,143 +105,153 @@
 def test_intersect_tube_hitmiss_zoomed():
     '''Rays that hit one tube, but miss a shorter one'''
     dir = np.array([[-.1, 0., 0., 0], [-1., 0, 0.2, 0.]])
     pos = np.array([[20., 0., 0.8, 1.], [2., .0, 0.4, 1.]])
 
     circ = Cylinder({'zoom': [1, 1, 1]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == True)
+    assert np.all(intersect)
 
     circ = Cylinder({'zoom': [1, 1, .5]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == False)
+    assert np.all(~intersect)
     assert np.all(np.isnan(interpos))
     assert np.all(np.isnan(inter_local))
 
+
 def test_intersect_tube_2points():
     dir = np.array([[-.1, 0., 0., 0], [-0.5, 0, 0., 0.], [-1., 0., 0., 0.]])
     pos = np.array([[50., 0., 0., 1.], [10., .5, 0., 1.], [2, 0, .3, 1.]])
 
     circ = Cylinder()
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == True)
+    assert np.all(intersect)
     assert np.allclose(h2e(interpos), np.array([[1., 0., 0.],
                                                 [np.sqrt(0.75), 0.5, 0.],
                                                 [1, 0., .3]]))
     assert np.allclose(inter_local, np.array([[0., np.arcsin(0.5), 0.],
                                               [0., 0., 0.3]]).T)
 
+
 def test_intersect_tube_2points_transformed():
     '''inter_local should be the same as interpos,
     even if we make the tube longer in z'''
     pos = np.array([[50., 0., 0., 1.], [10., .5, 0., 1.], [2, 0, .3, 1.]])
     dir = np.array([[-.1, 0., 0., 0], [-0.5, 0, 0., 0.], [-1., 0., 0., 0.]])
 
     exp_inter_loc = np.array([[0., np.arcsin(0.5), 0.],
                               [0., 0., 0.3]]).T
     exp_interpos = np.array([[1., 0., 0.],
                              [np.sqrt(0.75), 0.5, 0.],
                              [1, 0., .3]])
     circ = Cylinder({'zoom': [1, 1., 5.]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == True)
+    assert np.all(intersect)
     assert np.allclose(h2e(interpos), exp_interpos)
     assert np.allclose(inter_local, exp_inter_loc)
     # Rotate: interpos should be the same as in the unrotated case.
     # Beware of rotation direction!
     orient = transforms3d.axangles.axangle2mat([0, 0, 1], -.3)
     circ = Cylinder({'orientation': orient})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == True)
+    assert np.all(intersect)
     assert np.allclose(h2e(interpos), exp_interpos)
     assert np.allclose(inter_local, np.array([[0.3, 0.3 + np.arcsin(0.5), 0.3],
                                               [0., 0., 0.3]]).T)
 
     # Shift: inter_local is the same, but interpos changes
     circ = Cylinder({'position': [-.3, 0, 0]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == True)
+    assert np.all(intersect)
     assert np.allclose(h2e(interpos), np.array([[.7, 0, 0],
-                                                [np.sqrt(0.75) -.3, 0.5, 0.],
+                                                [np.sqrt(0.75) - .3, 0.5, 0.],
                                                 [.7, 0., .3]]))
     assert np.allclose(inter_local, exp_inter_loc)
 
+
 def test_intersect_tube_2points_outside():
     '''Setting phi_lim
 
     These are the same numbers, but with the phi_lim set, all intersection are
     at the "bottom" of the cylinder.'''
     pos = np.array([[50., 0., 0., 1.], [10., .5, 0., 1.], [2, 0, .3, 1.]])
     dir = np.array([[-.1, 0., 0., 0], [-0.5, 0, 0., 0.], [-1., 0., 0., 0.]])
 
     circ = Cylinder({'phi_lim': [.6, np.pi]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == True)
+    assert np.all(intersect)
     assert np.allclose(h2e(interpos), np.array([[-1., 0., 0.],
                                                 [-np.sqrt(0.75), 0.5, 0.],
                                                 [-1, 0., .3]]))
-    assert np.allclose(inter_local, np.array([[np.pi, np.pi - np.arcsin(0.5), np.pi],
-                                              [0., 0., 0.3]]).T)
+    assert np.allclose(inter_local,
+                       np.array([[np.pi, np.pi - np.arcsin(0.5), np.pi],
+                                 [0., 0., 0.3]]).T)
     # phi_lims that guarantee a miss
     circ = Cylinder({'phi_lim': [-.4, -.3]})
     intersect, interpos, inter_local = circ.intersect(dir, pos)
-    assert np.all(intersect == False)
+    assert np.all(~intersect)
     assert np.all(np.isnan(interpos))
     assert np.all(np.isnan(inter_local))
 
+
 @pytest.mark.xfail
 def test_phi_lim_verification():
     '''Check Errors for wrong phi_lim format.'''
     with pytest.raises(ValueError) as e:
-        circ = Cylinder({'phi_lim': [-.4, -.3, .4]})
+        Cylinder({'phi_lim': [-.4, -.3, .4]})
     assert '[lower limit, upper limit]' in str(e.value)
 
     with pytest.raises(ValueError) as e:
-        circ = Cylinder({'phi_lim': [-.4, -.5]})
+        Cylinder({'phi_lim': [-.4, -.5]})
     assert '[lower limit, upper limit]' in str(e.value)
 
     with pytest.raises(ValueError) as e:
-        circ = Cylinder({'phi_lim': [-.4, 5]})
+        Cylinder({'phi_lim': [-.4, 5]})
     assert 'range -pi to +pi' in str(e.value)
 
 
 def test_intersect_tube_2points_translation():
     '''Repeat test above with a tube that's moved and zoomed to make sure we
     did not mess up local and global coordinates in the implementation
     '''
     circ = Cylinder({'position': [0.8, 0.8, 1.2], 'zoom': [1, 1, 2]})
-    intersect, interpos, inter_local = circ.intersect(np.array([[1., 0., .0, 0],
-                                                                [1., 0., 0., 0.]]),
-                                                         np.array([[0., 0., 0., 1.],
-                                                                   [0., 0., 1., 1.]]))
-    assert np.all(intersect == True)
-    assert np.allclose(h2e(interpos), np.array([[.2, 0., 0.],
-                                                [.2, 0., 1.]]))
+    sect, pos, local = circ.intersect(np.array([[1., 0., .0, 0],
+                                                [1., 0., 0., 0.]]),
+                                      np.array([[0., 0., 0., 1.],
+                                                [0., 0., 1., 1.]]))
+    assert np.all(sect)
+    assert np.allclose(h2e(pos), np.array([[.2, 0., 0.],
+                                           [.2, 0., 1.]]))
+
 
 def test_tube_parametric():
-    '''Generate points on surface using parametric. Then make rays for intersection
-    which should return those points as intersection points.'''
+    '''Generate points on surface using parametric.
+
+    Then make rays for intersection
+    which should return those points as intersection points.
+    '''
     circ = Cylinder({'zoom': [2., 3., 4.]})
     parametric = circ.parametric_surface(phi=[-.1, 0., 1.])
     parametric = parametric.reshape((6, 4))
     # select dir so that it's in the right direction to recover these points.
     dir = np.tile([1, 0, 0, 0], (6, 1))
     intersect, interpos, inter_local = circ.intersect(dir, parametric)
     assert np.allclose(parametric, interpos)
 
+
 @pytest.mark.parametrize("geom", [FinitePlane, Cylinder])
 def test_local_coordsys(geom):
-    '''Ensure local coordiante systems are orthonormal'''
+    '''Ensure local coordinate systems are orthonormal'''
     rot = transforms3d.euler.euler2mat(*(np.pi * 2 * np.random.rand(3)))
     g = geom({'rotation': rot,
               'position': np.random.rand(3)})
 
     x, y, z = g.get_local_euklid_bases(np.random.rand(5, 2))
 
-    assert np.allclose(inner1d(x, y), 0)
-    assert np.allclose(inner1d(x, z), 0)
+    assert np.allclose(np.einsum("ij,ij->i", x, y), 0)
+    assert np.allclose(np.einsum("ij,ij->i", x, z), 0)
 
     for vec in [x, y, z]:
         assert np.allclose(np.linalg.norm(vec, axis=1), 1.)
 
     # Check it's a right-handed coordinage system
     assert np.allclose(np.cross(x[:, :3], y[:, :3]), z[:, :3])
```

### Comparing `marxs-1.2/marxs/math/tests/test_math.py` & `marxs-2.0/marxs/math/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/tests/test_polarization.py` & `marxs-2.0/marxs/math/tests/test_polarization.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/tests/test_random.py` & `marxs-2.0/marxs/math/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/tests/test_rotation.py` & `marxs-2.0/marxs/math/tests/test_rotation.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/tests/test_utils.py` & `marxs-2.0/marxs/math/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/math/utils.py` & `marxs-2.0/marxs/math/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 
+xyz2zxy = np.array([[0.,  1.,  0.,  0.],
+                    [0.,  0.,  1.,  0.],
+                    [1.,  0.,  0.,  0.],
+                    [0.,  0.,  0.,  1.]])
+'''Array toi flip coordinates for mission where the z-axis matches the optical axis.'''
 
 def e2h(e, w):
     '''Convert Euclidean coordinates to homogeneous coordinates
 
     Parameters
     ----------
     e : np.array
```

### Comparing `marxs-1.2/marxs/missions/chandra/HESSdesign.rdb` & `marxs-2.0/marxs/missions/chandra/HESSdesign.rdb`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/missions/chandra/__init__.py` & `marxs-2.0/marxs/missions/chandra/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,12 +17,12 @@
 reference files in the CALDB (or the files shipped with `classic MARX`_).
 Properties that are very easy to define and that are very unlikely to ever change
 (e.g. the mapping of ACIS chip number to chip name) are set in this module.
 That makes is easier to see where the numbers come from and thus helps for users
 who look at this module as an example of how to build up complex marxs setups.
 '''
 from .hess import HETG
-from .chandra import Chandra
+from .chandra_global import Chandra
 from .dither import LissajousDither
-from .acis import ACIS
+from .det_acis import ACIS
 from .data import (NOMINAL_FOCALLENGTH, AIMPOINTS, PIXSIZE)
 from .hrma_py import Aperture, HRMA
```

### Comparing `marxs-1.2/marxs/missions/chandra/acis.py` & `marxs-2.0/marxs/missions/chandra/det_acis.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,26 @@
 from ...simulator import Parallel
 from ...math.utils import h2e
 
 from .data import (NOMINAL_FOCALLENGTH, AIMPOINTS, TDET, ODET, PIXSIZE,
                    PIX_CORNER_LSI_PAR, chip2tdet)
 
 
-
 ACIS_name = ['I0', 'I1', 'I2', 'I3', 'S0', 'S1', 'S2', 'S3', 'S4', 'S5']
 '''names of the 10 ACIS chips'''
 
 
 class ACISChip(FlatDetector):
     '''A class that defines one chip in the ACIS instrument.'''
     def __init__(self, **kwargs):
         self.TDET = TDET['ACIS']
         self.ODET = ODET['ACIS']
         self.pixsize_in_rad = np.deg2rad(PIXSIZE['ACIS'])
         kwargs['ignore_pixel_warning'] = True
-        super(ACISChip, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def chip_name(self):
         return 'ACIS-{0}'.format(ACIS_name[self.id_num])
 
     def specific_process_photons(self, photons, intersect, interpos, intercoos):
         # CHIP and TDET are based on pixel coordinates
@@ -52,15 +51,16 @@
         photons.meta['ACSYS1'] = ('CHIP:AXAF-ACIS-1.0', 'reference for chip coord system')
         photons.meta['ACSYS2'] = ('TDET:{0}'.format(self.TDET['version']), 'reference for tiled detector coord system')
         photons.meta['ACSYS3'] = ('DET:ASC-FP-1.1', 'reference for focal plane coord system')
         photons.meta['ACSYS4'] = ('SKY:ASC-FP-1.1', 'reference for sky coord system')
         return {'chipx': chip[:, 0], 'chipy': chip[:, 1],
                 'tdetx': tdet[:, 0], 'tdety': tdet[:, 1],
                 'detx': detx, 'dety': dety,
-                'x': skyx, 'y': skyy,}
+                'x': skyx, 'y': skyy}
+
 
 class ACIS(Parallel):
     '''The ACIS instrument
 
     Missing:
 
     - This currently only implements the ideal **detection**, no PHA, no read-out streaks,
@@ -88,15 +88,15 @@
                                     kwargs.pop(['DetOffsetY'], 0)])
         # Now the ACIS specific case
         kwargs['elem_pos'] = self.calculate_elempos()
         kwargs['elem_class'] = ACISChip
         # Use 0.024 because that's more consistent with 1024 pix
         kwargs['elem_args'] = {'pixsize': 0.024 } # {'pixsize': 0.023985 }
 
-        super(ACIS, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.chips = chips
         self.elements = [self.elements[i] for i in chips]
 
     def get_corners(self):
         '''Get the coordinates of the ACIS pixel corners.
 
         Currently, this method reads the datafile included with MARX, but alternatively if could also
@@ -112,15 +112,15 @@
         '''
         t = Table.read(PIX_CORNER_LSI_PAR, format='ascii')
         out = []
         for chip in ACIS_name:
             coos = {}
             for corner in ['LL', 'LR', 'UR', 'UL']:
                 ind = t['col1'] == 'ACIS-{0}-{1}'.format(chip, corner)
-                coos[corner] = np.array([np.float(v) for v in t[ind]['col4'][0][1:-1].split()])
+                coos[corner] = np.array([float(v) for v in t[ind]['col4'][0][1:-1].split()])
             out.append(coos)
         return out
 
     def calculate_elempos(self):
         # This stuff is true for HRC, too. Move to more general class, once HRC is implemened.
         corners = self.get_corners()
         pos4d = []
@@ -146,14 +146,14 @@
             A[:3, 3] += self.aimpoint
             # for the coordiante convention - Offset is opposite to direction of coordiante system
             A[:3, 3] -= self.detoffset
             pos4d.append(A)
         return pos4d
 
     def process_photons(self, photons, *args, **kwargs):
-        photons = super(ACIS, self).process_photons(photons, *args, **kwargs)
+        photons = super().process_photons(photons, *args, **kwargs)
         photons.meta['SIM_X'] = self.aimpoint[0] - self.detoffset[0]
         photons.meta['SIM_Y'] = self.aimpoint[1] - self.detoffset[1]
         photons.meta['SIM_Z'] = self.aimpoint[2] - self.detoffset[2]
         photons.meta['DETNAM'] = 'ACIS-' + ''.join([str(i) for i in self.chips])
         photons.meta['INSTRUME'] = ('ACIS', 'Instrument')
         return photons
```

### Comparing `marxs-1.2/marxs/missions/chandra/chandra.py` & `marxs-2.0/marxs/missions/chandra/chandra_global.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     '''Main class representing the Chandra X-ray observatory
 
 
     '''
     def process_photons(self, photons):
         photons.meta['MISSION'] = ('AXAF', 'Mission')
         photons.meta['TELESCOP'] = ('CHANDRA', 'Telescope')
-        return super(Chandra, self).process_photons(photons)
+        return super().process_photons(photons)
 
     def write_evt(self, photons, filename):
         '''Write a Chandra event level 1 file.
 
         As opposed to directly saving the photon list, this adds some Chandra
         specific meta data.
```

### Comparing `marxs-1.2/marxs/missions/chandra/data.py` & `marxs-2.0/marxs/missions/chandra/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,14 +161,15 @@
 #
 HRC-S3-LL,s,h,"(0.000  -49.622  -13.167 )",,,"LSI coords for HRC-S2 LL"
 HRC-S3-LR,s,h,"(0.000  -49.622   13.167 )",,,"LSI coords for HRC-S2 LR"
 HRC-S3-UR,s,h,"(2.253 -155.400   13.167 )",,,"LSI coords for HRC-S2 UR"
 HRC-S3-UL,s,h,"(2.253 -155.400  -13.167 )",,,"LSI coords for HRC-S2 UL"
 '''
 
+
 def chip2tdet(chip, tdet, id_num):
     '''Convert CHIP coordinates to TDET coordiantes.
 
     See eqn (5) in `the Chandra coordiante memo <http://cxc.harvard.edu/contrib/jcm/ncoords.ps>`_.
 
     Parameters
     ----------
```

### Comparing `marxs-1.2/marxs/missions/chandra/dither.py` & `marxs-2.0/marxs/missions/chandra/dither.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     DitherPhase : `astropy.units.Quantity`
         (pitch, yaw, roll) dither phase at ``time = 0`` in radian
     '''
     def __init__(self, **kwargs):
         self.DitherAmp = kwargs.pop('DitherAmp', np.array([8., 8., 0.]) * u.arcsec)
         self.DitherPeriod = kwargs.pop('DitherPeriod', np.array([1000., 707., 1e5]) * u.s)
         self.DitherPhase = kwargs.pop('DitherPhase', np.zeros(3) * u.radian)
-        super(LissajousDither, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def dither(self, time):
         '''Calculate the dither offset relative to pointing direction.
 
         Parameters
         ----------
         time : np.array
@@ -41,15 +41,14 @@
         Returns
         -------
         delta : np.array of shape (N, 3)
             dither motion offset in pitch, yaw, roll for N times in rad
         '''
         return self.DitherAmp * np.sin(2. * np.pi * u.radian * time[:, np.newaxis] * u.s / self.DitherPeriod + self.DitherPhase)  / np.array([np.cos(self.coords.icrs.dec), 1., 1.])
 
-
     def pointing(self, time):
         '''Calculate the pointing direction for a set of times
         There are the steps to convert the dither (which are offsets) to the total
         pointing direction with the roll properly taken care of.
         (See marxasp.c in the marx code for more details.)
         1.  Convert ra/dec offsets to absolute pointing.
         2.  Roll resulting vector about nominal pointing
@@ -128,53 +127,55 @@
                               - pointing[i, 1],
                               - pointing[i, 2], 'rzyx')
 
             photons_dir[i, :3] = np.dot(mat3d.T, photons_dir[i, :3])
 
         return photons_dir
 
-
     def write_asol(self, photons, asolfile, timestep=0.256):
         '''Write an aspect solution (asol) file
 
-        Chandra analysis scripts often require an aspect solution, which is essientiall
-        a list of pointing directions in the dither pattern vs. time.
-        This method write such a list to a file.
+        Chandra analysis scripts often require an aspect solution,
+        which is essientially a list of pointing directions in the
+        dither pattern vs. time.  This method write such a list to a
+        file.
 
         Parameters
         ----------
         photons :  `astropy.table.Table` or `astropy.table.Row`
-            Table with photon properties. Some meta data from the header of this table
-            is required (e.g. the length of the observation).
+            Table with photon properties. Some meta data from the header of
+            this table is required (e.g. the length of the observation).
         asolfile : string
             Path and file name where the asol file is saved.
         timestamp : float
             Time step between entries in the asol file in seconds.
+
         '''
         time = np.arange(0, photons.meta['EXPOSURE'][0], timestep)
         pointing = self.pointing(time).to(u.deg).value
         asol = Table([time, pointing[:, 0], pointing[:, 1], pointing[:, 2]],
                      names=['time', 'ra', 'dec', 'roll'],
                      )
         asol['time'].unit = 's'
         # The following columns represent measured offsets in Chandra
         # They are not part of this simulation. Simply set them to 0
-        for col in [ 'ra_err', 'dec_err', 'roll_err',
-                     'dy', 'dz', 'dtheta', 'dy_err', 'dz_err', 'dtheta_err',
-                      'roll_bias', 'pitch_bias', 'yaw_bias', 'roll_bias_err', 'pitch_bias_err', 'yaw_bias_err']:
+        for col in ['ra_err', 'dec_err', 'roll_err',
+                    'dy', 'dz', 'dtheta', 'dy_err', 'dz_err', 'dtheta_err',
+                    'roll_bias', 'pitch_bias', 'yaw_bias', 'roll_bias_err',
+                    'pitch_bias_err', 'yaw_bias_err']:
             asol[col] = np.zeros_like(time)
             if 'bias' in col:
                 asol[col].unit = 'deg / s'
             elif ('dy' in col) or ('dz' in col):
                 asol[col].unit = 'mm'
             else:
                 asol[col].unit = 'deg'
         asol['q_att'] = [mat2quat(euler2mat(np.deg2rad(p[0]),
-                                   np.deg2rad(-p[1]),
-                                   np.deg2rad(-p[2]), 'rzyx'))
+                                            np.deg2rad(-p[1]),
+                                            np.deg2rad(-p[2]), 'rzyx'))
                          for p in pointing]
         # Copy info like the exposure time from the photons list meta to asol,
         # but not column specific keywords like TTYPEn, TCTYPn, MTYPEn, MFORMn, etc:
         for k in photons.meta:
             if (('TYP' not in k) and ('FORM' not in k) and
                 ('TCR' not in k) and ('TCDEL' not in k) and (k not in asol.meta)):
                 asol.meta[k] = photons.meta[k]
```

### Comparing `marxs-1.2/marxs/missions/chandra/fitsheaders.py` & `marxs-2.0/marxs/missions/chandra/fitsheaders.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/missions/chandra/hess.py` & `marxs-2.0/marxs/missions/chandra/hess.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,57 +3,64 @@
 from astropy.table import Table
 from astropy.utils.data import get_pkg_data_filename
 from transforms3d.affines import compose
 
 from ...optics import FlatGrating, OrderSelector
 from ...simulator import Parallel
 
+
 class HETG(Parallel):
 
     id_col = 'facet'
 
     def __init__(self, **kwargs):
         self.hess = Table.read(get_pkg_data_filename('HESSdesign.rdb'))
         '''The HESS datafile is commented very well inside the rdb file.
-        Here, I just need to make a note about the relation of the coordinate systems:
-        The vectors that define the facet edges are called x and y in the rdb file.
-        In the MARXS global coordinate system these are y and z respectively, so
-        uxf -> y and uyg -> z.
+
+        Here, I just need to make a note about the relation of the
+        coordinate systems: The vectors that define the facet edges
+        are called x and y in the rdb file.  In the MARXS global
+        coordinate system these are y and z respectively, so uxf -> y
+        and uyg -> z.
 
         Datafile from: http://space.mit.edu/HETG/hess/basic.html
+
         '''
         kwargs['elem_pos'] = self.calculate_elempos()
         kwargs['elem_class'] = FlatGrating
         # Gratings are defined in order MEG, then HEG
         d = [4001.95 * 1e-7] * 192 + [2000.81 * 1e-7] * 144
         ul = np.vstack([self.hess[s+'ul'].data for s in 'xyz'])
         uyf = np.vstack([self.hess[s + 'uyf'].data for s in 'xyz'])
         uxf = np.vstack([self.hess[s + 'uxf'].data for s in 'xyz'])
         groove_ang = -np.arctan2(np.einsum('i...,i...->...', ul, uxf),
                                  np.einsum('i...,i...->...', ul, uyf))
         kwargs['elem_args'] = {'order_selector': OrderSelector(np.arange(-3, 4)),
                                'd': d, 'name': list(self.hess['hessloc']),
                                'groove_angle': groove_ang.tolist()}
-        super(HETG, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         # I would like to put the center of the HETG on its hinge point.
         # Unfortunately, I don't know that hinge point very well, so I'm guessing a little.
         move = np.eye(4)
-        move[:, 3] = [8600., 580 * np.cos(np.deg2rad(30)),
-                      580 * np.sin(np.deg2rad(30)), 1.]
+        move[:, 3] = [8618., -650 * np.sin(np.deg2rad(60)),
+                      650 * np.cos(np.deg2rad(60)), 1.]
+        self.move_center(move)
 
     def calculate_elempos(self):
         '''Read position of facets from file.
 
-        Based on the positions, other grating parameters are chosen that differ between
-        HEG and MEG, e.g. grating constant.
+        Based on the positions, other grating parameters are chosen
+        that differ between HEG and MEG, e.g. grating constant.
+
         '''
-        # take x,y,z components of various vectors and put in numpy arrays
-        # Note: This makes (3, N) arrays as opposed to (N, 3) arrays used in other parts of MARXS.
-        # Note: Sometimes an angle has a minus. Beware of active / passive rotations.
+        # take x,y,z components of various vectors and put in numpy
+        # arrays Note: This makes (3, N) arrays as opposed to (N, 3)
+        # arrays used in other parts of MARXS.  Note: Sometimes an
+        # angle has a minus. Beware of active / passive rotations.
         hess = self.hess
 
         cen = np.vstack([hess[s+'c'].data for s in 'xyz'])
         cen[0, :] += (339.909 - 1.7) * 25.4
 
         # All those vectors are already normalized
         facnorm = np.vstack([hess[s + 'u'].data for s in 'xyz'])
```

### Comparing `marxs-1.2/marxs/missions/chandra/hrma_py.py` & `marxs-2.0/marxs/missions/chandra/hrma_py.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,42 +5,46 @@
 '''
 import numpy as np
 import astropy.units as u
 
 from .data import NOMINAL_FOCALLENGTH
 from ...import optics
 
-mirror_radii = np.array([[598.,610.],[481, 491], [424, 433], [315,322]])
+
+mirror_radii = np.array([[598., 610.], [481, 491], [424, 433], [315, 322]])
+
 
 class Aperture(optics.MultiAperture):
     '''Chandra opening aperture of four rings above the mirror shells.
     '''
     def __init__(self, **kwargs):
-        if not 'id_col' in kwargs:
+        if 'id_col' not in kwargs:
             kwargs['id_col'] = 'mirror_shell'
-        if not 'elements' in kwargs:
+        if 'elements' not in kwargs:
             kwargs['elements'] = [optics.CircleAperture(position=[NOMINAL_FOCALLENGTH, 0, 0],
                               zoom=[1, r[1], r[1]], r_inner=r[0]) for r in mirror_radii]
-        super(Aperture, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class HRMA(optics.FlatStack):
     '''High-resolution mirror assembly in a pure Python implementation
 
-    This class delivers a rough approximation (a few percent for on-axis sources)
-    to the Chandra mirror. Many important effects are missing (e.g. the mirror
-    reflectivity in this module is not energy dependent, neither is the mirror scatter).
-    Use `marxs.optics.MarxMirror` if possible.
+    This class delivers a rough approximation (a few percent for
+    on-axis sources) to the Chandra mirror. Many important effects are
+    missing (e.g. the mirror reflectivity in this module is not energy
+    dependent, neither is the mirror scatter).  Use
+    `marxs.optics.MarxMirror` if possible.
+
     '''
     def __init__(self, **kwargs):
         'asf'
         kwargs['position'] = [NOMINAL_FOCALLENGTH, 0, 0]
         kwargs['zoom'] = [1, 650., 650]
         kwargs['elements'] = [optics.PerfectLens,
                               optics.RadialMirrorScatter,
                               optics.EnergyFilter]
         kwargs['keywords'] = [{'focallength': NOMINAL_FOCALLENGTH},
                               {'inplanescatter': 3.6e-6 * u.rad,
                                'perpplanescatter': 1.2e-6 * u.rad},
                               {'filterfunc': lambda x: np.ones_like(x) * 0.66,
                                'name': 'support spider, reflectivity, et al.'}]
-        super(HRMA, self).__init__(**kwargs)
+        super().__init__(**kwargs)
```

### Comparing `marxs-1.2/marxs/missions/chandra/tests/sim_asol.fits` & `marxs-2.0/marxs/missions/chandra/tests/sim_asol.fits`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/missions/chandra/tests/test_chandra.py` & `marxs-2.0/marxs/missions/chandra/tests/test_chandra.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,92 +14,116 @@
 CWD = os.getcwd()
 TEST_DIR = os.path.dirname(__file__)
 
 
 def setup_function(function):
     os.chdir(TEST_DIR)
 
+
 def teardown_function(function):
     os.chdir(CWD)
 
+
 def test_ditherpattern():
     '''check that the dither pattern generated with consistent with MARX.'''
-    mypointing = chandra.LissajousDither(coords=SkyCoord(212.5, -33., unit='deg'),
+    mypointing = chandra.LissajousDither(coords=SkyCoord(212.5, -33.,
+                                                         unit='deg'),
                                          roll=15. * u.deg)
     time = np.arange(1000)
     coords = np.rad2deg(mypointing.pointing(time))
     masol = Table.read('sim_asol.fits')
-    assert np.allclose(coords[:, 0], np.interp(time, masol['time']-masol['time'][0], masol['ra']))
-    assert np.allclose(coords[:, 1], np.interp(time, masol['time']-masol['time'][0], masol['dec']))
-    assert np.allclose(coords[:, 2], np.interp(time, masol['time']-masol['time'][0], masol['roll']))
+    assert np.allclose(coords[:, 0],
+                       np.interp(time, masol['time'] - masol['time'][0],
+                                 masol['ra']))
+    assert np.allclose(coords[:, 1],
+                       np.interp(time, masol['time'] - masol['time'][0],
+                                 masol['dec']))
+    assert np.allclose(coords[:, 2],
+                       np.interp(time, masol['time'] - masol['time'][0],
+                                 masol['roll']))
+
 
 def test_stationary_pointing():
     '''Constant pointing can also be realized through a Lissajous with amplitude=0.'''
     mysource = PointSource(coords=SkyCoord(30., 30., unit="deg"))
-    fixedpointing = FixedPointing(coords=SkyCoord(30., 30., unit=u.degree), roll=15. * u.degree)
-    lisspointing = chandra.LissajousDither(coords=SkyCoord(30., 30., unit=u.degree),
-                                           roll=15. * u.degree, DitherAmp=np.zeros(3)*u.degree)
+    fixedpointing = FixedPointing(coords=SkyCoord(30., 30., unit=u.degree),
+                                  roll=15. * u.degree)
+    lisspointing = chandra.LissajousDither(coords=SkyCoord(30., 30.,
+                                                           unit=u.degree),
+                                           roll=15. * u.degree,
+                                           DitherAmp=np.zeros(3)*u.degree)
 
     photons = mysource.generate_photons(2 * u.s)
     fixedphotons = fixedpointing(photons.copy())
     lissphotons = lisspointing(photons.copy())
 
     assert np.allclose(fixedphotons['dir'], lissphotons['dir'])
 
+
 def test_detector_coordsystems():
-    '''Compare detector coordinates for known photon direction with CIAO dmcoords.
+    '''Compare detector coordinates with CIAO dmcoords.
+
+    Currently, I don't aim to make this very precise - within a pixel
+    or so is fine.  To make this more precise, there are several
+    places to go: The most obvious one is the size of the pixel -
+    currently the number of pixels times the pixel size does now match
+    the length of the chip precisely.
 
-    Currently, I don't aim to make this very precise - within a pixel or so is fine.
-    To make this more precise, there are several places to go:
-    The most obvious one is the size of the pixel - currently the number of pixels times
-    the pixel size does now match the length of the chip precisely.
     '''
     mysource = PointSource(coords=SkyCoord(30., 30., unit="deg"))
-    mypointing = chandra.LissajousDither(coords=SkyCoord(30., 30., unit='deg'), roll=15. * u.degree)
+    mypointing = chandra.LissajousDither(coords=SkyCoord(30., 30., unit='deg'),
+                                         roll=15. * u.degree)
     # marxm = MarxMirror('./marxs/optics/hrma.par', position=np.array([0., 0,0]))
     acis = chandra.ACIS(chips=[0,1,2,3], aimpoint=chandra.AIMPOINTS['ACIS-I'])
 
     photons = mysource.generate_photons(5 * u.s)
     photons = mypointing(photons)
-    # We want reproducible direction, so don't use mirror, but set direction by hand
+    # We want reproducible direction, so don't use mirror,
+    # but set direction by hand
     # photons = marxm(photons)
     # photons = photons[photons['probability'] > 0]
-    photons['pos'] = np.array([[100., 0, 0, 1],[100, 10, 0, 1], [100, 0, 10, 1],
-                               [100, -10, 0, 1], [100, 0, -10, 1]])
+    photons['pos'] = np.array([[100., 0, 0, 1],
+                               [100, 10, 0, 1],
+                               [100, 0, 10, 1],
+                               [100, -10, 0, 1],
+                               [100, 0, -10, 1]])
 
     photons.meta['MISSION'] = ('AXAF', 'Mission')
     photons.meta['TELESCOP'] = ('CHANDRA', 'Telescope')
 
     photons = acis(photons)
     # We need the asol to run CIAO.
-    # I've done that already and the expected numbers are hard-coded in the assert statement.
+    # I've done that already and the expected numbers are hard-coded.
     # Here are commands I used:
     # mypointing.write_asol(photons, 'asol.fits')
     # chandra.Chandra.write_evt('photons.fits')
 
     atol = 1.
     # This is the starting point
     assert np.allclose(photons['detx'], [4096.5, 4513.2, 4096.5, 3679.8, 4096.5], atol=atol)
     assert np.allclose(photons['dety'], [4096.5, 4096.5, 3679.8, 4096.5, 4513.2], atol=atol)
-    # I took these numbers and types them into dmcoords.
-    # Thus, if these numbers change when increasing the accuracy of the pixel size or the
-    # position of the chip edges, ... then all the numbers below need to be changed, too.
+    # I took these numbers and types them into dmcoords.  Thus, if
+    # these numbers change when increasing the accuracy of the pixel
+    # size or the position of the chip edges, ... then all the numbers
+    # below need to be changed, too.
     assert np.all(photons['CCD_ID'] == [3, 3, 1, 2, 3])
     assert np.allclose(photons['chipx'], [984.34, 984.34, 355.7, 40.91, 566.56], atol=atol)
     assert np.allclose(photons['chipy'], [994.8, 577.02, 994.23, 658.95, 993.75], atol=atol)
     assert np.allclose(photons['x'], [4096.5, 4499., 3988.5, 3693.4, 4204.34], atol=atol)
     assert np.allclose(photons['y'], [4096.5, 3988.65, 3693.4, 4204.5, 4499.], atol=atol)
     assert np.allclose(photons['tdetx'], [4137.2, 4555, 4137.77, 3720, 4138.25], atol=atol)
 
 
 def test_ACIS_pixel_number():
     '''The pixel size and chip size given in the docs are not consistent.
 
     Make sure we end up with 1024*1024 chips.
     '''
-    acis = chandra.ACIS(chips=[0, 1, 2, 3], aimpoint=chandra.AIMPOINTS['ACIS-I'])
+    acis = chandra.ACIS(chips=[0, 1, 2, 3],
+                        aimpoint=chandra.AIMPOINTS['ACIS-I'])
     for i in range(3):
         assert acis.elements[i].npix == [1024, 1024]
 
-    acis = chandra.ACIS(chips=[4, 5, 6, 7, 8, 9], aimpoint=chandra.AIMPOINTS['ACIS-I'])
+    acis = chandra.ACIS(chips=[4, 5, 6, 7, 8, 9],
+                        aimpoint=chandra.AIMPOINTS['ACIS-I'])
     for i in range(5):
         assert acis.elements[i].npix == [1024, 1024]
```

### Comparing `marxs-1.2/marxs/missions/chandra/tests/test_hetg.py` & `marxs-2.0/marxs/missions/chandra/tests/test_hetg.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 
 from .. import HETG
 
+
 def test_orient():
     '''Check orientation of gratings.'''
     hetg = HETG()
     for i in range(len(hetg.elements)):
         ex = hetg.elements[i].geometry['e_x'][:3]
         ey = hetg.elements[i].geometry['e_y'][:3]
         ez = hetg.elements[i].geometry['e_z'][:3]
```

### Comparing `marxs-1.2/marxs/missions/chandra/tests/test_hrma.py` & `marxs-2.0/marxs/missions/chandra/tests/test_hrma.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/missions/mitsnl/SiTransmission.csv` & `marxs-2.0/marxs/missions/mitsnl/data/SiTransmission.csv`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/missions/mitsnl/catgrating.py` & `marxs-2.0/marxs/missions/mitsnl/catgrating.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,44 +6,43 @@
 instruments in space. One particular field of research are critical
 angle transmission (CAT) gratings, see e.g. `Heilmann et al. (2015)`_
 
 .. _Space Nanotechnology Laboratory: http://snl.mit.edu/
 .. _Heilmann et al. (2015): http://dx.doi.org/10.1117/12.2188525
 '''
 import numpy as np
-from numpy.core.umath_tests import inner1d
 from scipy.interpolate import RectBivariateSpline, interp1d
 import astropy.units as u
 from astropy.utils.data import get_pkg_data_filename
 from astropy.table import Table
 
 from marxs.optics import (CATGrating,
                           OrderSelector, FlatStack,
                           FlatOpticalElement)
 from marxs.math.utils import norm_vector
 from marxs.optics.scatter import RandomGaussianScatter
-
+from marxs.utils import tablerows_to_2d
 
 __all__ = ['l1transtab', 'l1_order_selector',
            'l1_dims', 'l2_dims',
            'qualityfactor', 'd',
-           'load_table2d',
            'InterpolateEfficiencyTable',
            'QualityFactor',
            'L1',
            'L2Abs',
            'L2Diffraction',
            'CATL1L2Stack',
            'NonParallelCATGrating',
+           'catsupportbars',
            ]
 
 d = 0.0002
 '''Spacing of grating bars'''
 
-l1transtab = Table.read(get_pkg_data_filename('SiTransmission.csv'), format='ascii.ecsv')
+l1transtab = Table.read(get_pkg_data_filename('data/SiTransmission.csv'), format='ascii.ecsv')
 '''Transmission through 1 mu of Si'''
 
 l1_order_selector = OrderSelector(orderlist=np.array([-4, -3, -2, -1, 0, 1, 2, 3, 4]),
                                   p=np.array([0.006, 0.0135, 0.022, 0.028, 0.861, 0.028, 0.022, 0.0135, 0.006]))
 '''Simple order selector for diffraction on L1.
 
 The numbers here are calculated for the 2018 Arcus gratings assuming the L1 structure
@@ -57,103 +56,57 @@
 l2_dims = {'bardepth': 0.5 * u.mm, 'period': 0.9622504 * u.mm, 'barwidth': 0.0962250 * u.mm}
 '''Dimensions of hexagonal L2 support'''
 
 qualityfactor = {'d': 200. * u.um, 'sigma': 1.75 * u.um}
 '''Scaling of grating efficiencies, parameterized as a Debye-Waller factor'''
 
 
-class DataFileFormatException(Exception):
-    '''Exception for grating efficiency files not matching expected format.'''
-    pass
-
-
-def load_table2d(filename):
-    '''Get a 2d array from an ecsv input file.
-
-    In the table file, the data is flattened to a 1d form.
-    The first two columns are x and y, like this:
-    The first column looks like this with many duplicates:
-    [1,1,1,1,1,1,2,2,2,2,2,2,3,3,3, ...].
-    Column B repeats like this: [1,2,3,4,5,6,1,2,3,4,5,6,1,2,3, ...].
-
-    All remaining columns are data on the same x-y grid, and the grid
-    has to be regular.
-
-
-    Parameters
-    ----------
-    filename : string
-        Name and path of data file
-
-    Returns
-    -------
-    tab : `astropy.table.Table`
-        Table as read in. Useful to access units or other meta data.
-    x, y : `astropy.table.Column`
-        Unique entries in first and second column
-    dat : np.array
-        The remaining outputs are np.arrays of shape (len(x), len(y))
-    '''
-    tab = Table.read(filename, format='ascii.ecsv')
-    x = tab.columns[0]
-    y = tab.columns[1]
-    n_x = len(set(x))
-    n_y = len(set(y))
-    if len(x) != (n_x * n_y):
-        raise DataFileFormatException('Data is not on regular grid.')
-
-    x = x[::n_y]
-    y = y[:n_y]
-    coldat = [tab[d].data.reshape(n_x, n_y) for d in tab.columns[2:]]
-
-    return tab, x, y, coldat
-
-
 class InterpolateEfficiencyTable(object):
     '''Order Selector for MARXS using a specific kind of data table.
 
     Ralf Heilmann from the SNL typically writes simulated grating efficiencies
     into Excel tables. Since Excel is hard to read in Python and not very
     suited to version control with git, those tables are converted to csv files
     of a certain format.
     A short summary of this format is given here, to help reading the code.
-    The table contains data in 3-dimenasional (wave, n_theta, order) space,
+    The table contains data in 3-dimensional (wave, n_theta, order) space,
     flattened into a 2d table.
 
     - Row 1 + 2: Column labels. Not used here.
     - Column A: wavelength in nm.
     - Column B: blaze angle in deg.
     - Rest: data
 
     For each wavelength there are multiple blaze angles listed, so Column A
     contains
-    many dublicates and looks like this: [1,1,1,1,1,1,2,2,2,2,2,2,3,3,3, ...].
+    many duplicates and looks like this: [1,1,1,1,1,1,2,2,2,2,2,2,3,3,3, ...].
     Column B repeats like this: [1,2,3,4,5,6,1,2,3,4,5,6,1,2,3, ...].
 
     Because the wave, theta grid is regular, this class can use the
     `scipy.interpolate.RectBivariateSpline` for interpolation in each 2-d slice
     (``order`` is an integer and not interpolated).
 
     Parameters
     ----------
-    filename : string
-        path and name of data file
+    tab : `astropy.table.Table`
+        Table as read in. Useful to access units or other meta data.
     k : int
         Degree of spline. See `scipy.interpolate.RectBivariateSpline`.
     '''
 
-    def __init__(self, filename, k=3):
-        tab, wave, theta, orders = load_table2d(filename)
+    def __init__(self, tab, k=1):
+        wave, theta, orders = tablerows_to_2d(tab)
+
         theta = theta.to(u.rad)
         # Order is int, we will never interpolate about order,
         self.orders = np.array([int(n) for n in tab.colnames[2:]])
         self.interpolators = [RectBivariateSpline(wave, theta, d, kx=k, ky=k) for d in orders]
 
     def probabilities(self, energies, pol, blaze):
-        '''Obtain the probabilties for photons to go into a particular order.
+        '''Obtain the probabilities for photons to go into a particular order.
 
         This has the same parameters as the ``__call__`` method, but it returns
         the raw probabilities, while ``__call__`` will draw from these
         probabilities and assign an order and a total survival probability to
         each photon.
 
         Parameters
@@ -188,15 +141,15 @@
         cumprob = np.cumsum(interpprobs, axis=0) / totalprob
         ind_orders = np.argmax(cumprob > np.random.rand(len(energies)), axis=0)
 
         return orders[ind_orders], totalprob
 
 
 class QualityFactor(FlatOpticalElement):
-    '''Scale probabilites of theoretical curves to measured values.
+    '''Scale probabilities of theoretical curves to measured values.
 
     All gratings look better in theory than in practice. This grating quality
     factor scales the calculated diffraction probabilities to the observed
     performance.
     '''
 
     def __init__(self, qualityfactor=qualityfactor, **kwargs):
@@ -231,15 +184,17 @@
     blaze_name = 'blaze_L1'
     order_name = 'order_L1'
 
     def __init__(self, l1_dims=l1_dims, **kwargs):
         check_lx_dims(l1_dims)
         self.openfraction = 1 - l1_dims['barwidth'] / l1_dims['period']
         energy = l1transtab['energy'].to(u.keV, equivalencies=u.spectral())
-        trans = np.exp(np.log(l1transtab['transmission']) * l1_dims['bardepth'] / (1 * u.micrometer))
+        with np.errstate(divide='ignore'):
+            logtranstab = np.log(l1transtab['transmission'])
+        trans = np.exp(logtranstab * l1_dims['bardepth'] / (1 * u.micrometer))
         self.transfunc = interp1d(energy, trans)
         kwargs['d'] = l1_dims['period'].to(u.mm).value
         super().__init__(**kwargs)
 
 
     def specific_process_photons(self, photons, intersect,
                                  interpos, intercoos):
@@ -283,15 +238,15 @@
         self.innerfree = self.period - self.barwidth
 
     def specific_process_photons(self, photons, intersect,
                                  interpos, intercoos):
 
         p3 = norm_vector(photons['dir'].data[intersect])
         ex, ey, en = self.geometry.get_local_euklid_bases(intercoos[intersect, :])
-        angle = np.arccos(np.abs(inner1d(p3, en)))
+        angle = np.arccos(np.abs(np.einsum("ij,ij->i", p3, en)))
 
         # fractional area NOT covered by the hexagon structure
         openfraction = (self.innerfree / self.period)**2
         # fractional area shadowed by inclined hexagon structure
         shadowarea = (self.bardepth * self.innerfree * np.sin(angle))
         totalarea = self.period**2 / 2 * np.sqrt(3)
         shadowfraction = shadowarea / totalarea
@@ -359,49 +314,52 @@
 
 def catsupportbars(photons):
     '''Metal structure that holds grating facets will absorb all photons
     that do not pass through a grating facet.
 
     We might want to call this L3 support ;-)
     '''
-    photons['probability'][photons['facet'] < 0] = 0.
+    if 'facet' in photons.colnames:
+        photons['probability'][photons['facet'] < 0] = 0.
+    else:
+        photons['probability'] = 0.
     return photons
 
 
 class CATL1L2Stack(FlatStack):
     '''SNL fabricated CAT grating
 
     This element combines all parts of a CAT grating into a single object.
     These include the grating membrane and the absorption and diffraction due
     to the L1 and L2 support.
-    Approximations are done for all those elements, see the individial classes
+    Approximations are done for all those elements, see the individual classes
     for more details. Except for `order_selector` all other parameters are set with
     defaults defined in module level variables.
 
     Parameters
     ----------
     order_selector : `marxs.optics.OrderSelector`
         Order selector for the grating membrane
     groove_angle : float
-        Goove angle of grating bars (in rad). Default: 0
+        Groove angle of grating bars (in rad). Default: 0
     l1_order_selector : `marxs.optics.OrderSelector`
         Order selector for L1 dispersion (cross-dispersion direction for grating)
     qualityfactor : dict
         Parameterization of grating quality scaling factor. See model level variable
         for format.
     l1_dims : dict
         Dimensions of L1 support. See module level variable for format.
     l2_dims : dict
         Dimensions of L2 support. See module level variable for format.
     '''
     def __init__(self, l1_dims=l1_dims, l2_dims=l2_dims,
                  l1_order_selector=l1_order_selector,
                  qualityfactor=qualityfactor,
                  **kwargs):
-        kwargs['elements'] = [CATGrating,
+        kwargs['elements'] = [NonParallelCATGrating,
                               QualityFactor,
                               L1,
                               L2Abs,
                               L2Diffraction,
                           ]
         groove_angle = kwargs.pop('groove_angle', 0.)
         kwargs['keywords'] = [{'order_selector': kwargs.pop('order_selector'),
```

### Comparing `marxs-1.2/marxs/missions/mitsnl/tests/grating_efficiency.csv` & `marxs-2.0/marxs/missions/mitsnl/tests/grating_efficiency.csv`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/missions/mitsnl/tests/test_cat.py` & `marxs-2.0/marxs/missions/mitsnl/tests/test_cat.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,112 +1,135 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import pytest
 import numpy as np
 import astropy.units as u
+from astropy.table import Table
 from astropy.utils.data import get_pkg_data_filename
 from transforms3d.euler import euler2mat
 
-from ..catgrating import *
-from ..catgrating import DataFileFormatException, check_lx_dims
+from .. import catgrating
+from ..catgrating import check_lx_dims
 from marxs.optics import CATGrating, OrderSelector, FlatDetector
 from marxs.optics.scatter import RandomGaussianScatter
-from marxs.utils import generate_test_photons
+from marxs.utils import generate_test_photons, DataFileFormatException
+
 
 def test_nonparallelCATGrating_simplifies_to_CATGrating():
     '''With all randomness parameters set to 0, the results
     should match a CAT grating exactly.'''
     photons = generate_test_photons(50)
     # Mix the photons up a little
     scat = RandomGaussianScatter(scatter=0.01 * u.rad)
     photons = scat(photons)
     order_selector = OrderSelector([2])
     cat = CATGrating(order_selector=order_selector, d=0.001)
-    npcat = NonParallelCATGrating(order_selector=order_selector, d=0.001)
+    npcat = catgrating.NonParallelCATGrating(order_selector=order_selector,
+                                             d=0.001)
     p1 = cat(photons.copy())
     p2 = npcat(photons)
     assert np.all(p1['dir'] == p2['dir'])
 
+
 def test_check():
     '''Make sure check raises Exception for unphysical parameters'''
     with pytest.raises(ValueError):
         check_lx_dims({'barwidth': 1, 'period': 1})
 
+
 def test_scalingSitransparancy():
     '''The module has data for 1 mu Si and scales that to the depth of the
     grating. Test against known-good coefficient from CXRO.'''
     photons = generate_test_photons(100)
-    cat = L1(order_selector=OrderSelector([-5]),
-             l1_dims = {'bardepth': 0.004 * u.mm,
-                        'period': 0.0001 * u.mm,
-                        'barwidth': 0.00009 * u.mm})
+    cat = catgrating.L1(order_selector=OrderSelector([-5]),
+                        l1_dims={'bardepth': 0.004 * u.mm,
+                                 'period': 0.0001 * u.mm,
+                                 'barwidth': 0.00009 * u.mm})
     photons = cat(photons)
     assert np.isclose(np.median(photons['probability']), 0.22458, rtol=1e-4)
 
 
 def test_L2_broadening():
     '''Compare calculated L2 broadening with the values calculated
     by Ralf Heilmann. Both calculation make simplications (e.g. assuming
     a circular hole), but should give the right order of magnitude for
     diffraction.'''
     photons = generate_test_photons(1000)
     photons['energy'] = 0.25  # 50 Ang
-    l2 = L2Diffraction(l2_dims={'period': 0.966 * u.mm,
-                                'barwidth': 0.1 * u.mm})
+    l2 = catgrating.L2Diffraction(l2_dims={'period': 0.966 * u.mm,
+                                           'barwidth': 0.1 * u.mm})
     photons = l2(photons)
     det = FlatDetector(position=[-1, 0, 0])
     photons = det(photons)
     sigma = np.std(photons['det_x'])
     # for small angles tan(alpha) = alpha
     # 1 arcsec = 4.8...e-6 rad
     # 0.5 is sigma calculated by Ralf Heilmann for a rectangular
     # aperture
     assert np.isclose(sigma, .5 * 4.8e-6, rtol=.5)
 
 
 def test_L2_Abs():
     '''Check L2 absorption against numbers calculated by Ralf Heilmann.'''
     photons = generate_test_photons(1)
-    l2 = L2Abs(l2_dims={'period': 0.966 * u.mm, 'bardepth': 0.5 * u.mm,
-                        'barwidth': 0.1 * u.mm})
+    l2 = catgrating.L2Abs(l2_dims={'period': 0.966 * u.mm,
+                                   'bardepth': 0.5 * u.mm,
+                                   'barwidth': 0.1 * u.mm})
     photons = l2(photons)
     assert np.isclose(photons['probability'], 0.81, rtol=0.02)
 
 
 def test_L2_Abs_angle():
     '''Test that that shadow area increases with angle.
     The comparison number was calculated by H. M. Guenther in response
     to Arcus DQ36.'''
     l2_dims = {'period': 0.966 * u.mm, 'bardepth': 0.5 * u.mm,
                'barwidth': 0.1 * u.mm}
 
-    l2 = L2Abs(l2_dims=l2_dims)
+    l2 = catgrating.L2Abs(l2_dims=l2_dims)
     p1 = l2(generate_test_photons(1))
 
-    l2 = L2Abs(l2_dims=l2_dims, orientation=euler2mat(np.deg2rad(1.8), 0, 0, 'szxy'))
+    l2 = catgrating.L2Abs(l2_dims=l2_dims,
+                          orientation=euler2mat(np.deg2rad(1.8), 0, 0, 'szxy'))
     p2 = l2(generate_test_photons(1))
 
-    assert np.isclose(p2['probability'][0] / p1['probability'][0], 0.979, rtol=1e-3)
+    assert np.isclose(p2['probability'][0] / p1['probability'][0], 0.979,
+                      rtol=1e-3)
 
 
 def test_efficiency_table():
     '''Test that the efficiency is read in in the right format.'''
-    efftab = InterpolateEfficiencyTable(get_pkg_data_filename('grating_efficiency.csv'), k=2)
+    tab = Table.read(get_pkg_data_filename('grating_efficiency.csv'), format='ascii.ecsv')
+    efftab = catgrating.InterpolateEfficiencyTable(tab, k=2)
     orders, interpprobs = efftab.probabilities(np.array([0.5, 0.5, 1, 1]),
                                                np.ones(4),
                                                np.deg2rad([1., 2., 1., 2.]))
     assert np.allclose(interpprobs.sum(axis=0), [.8, .8, 1., 1.], rtol=1e-4)
     assert np.allclose(interpprobs[:, 0], [.3, .3, .2], rtol=1e-4)
 
 
 def test_efficiency_table_in_use():
     '''Use table in a optical element'''
-    efftab = InterpolateEfficiencyTable(get_pkg_data_filename('grating_efficiency.csv'), k=2)
+    tab = Table.read(get_pkg_data_filename('grating_efficiency.csv'), format='ascii.ecsv')
+    efftab = catgrating.InterpolateEfficiencyTable(tab, k=2)
     cat = CATGrating(order_selector=efftab, d=0.001)
     photons = generate_test_photons(5000)
     photons = cat(photons)
-    assert np.isclose((photons['order']==0).sum(), len(photons) / 2, rtol=.05)
+    assert np.isclose((photons['order'] == 0).sum(), len(photons) / 2,
+                      rtol=.05)
 
 
 def test_efficiency_table_wrong_format():
     '''Try to load a datafile with mission rows.'''
+    tab = Table.read(get_pkg_data_filename('grating_efficiency_broken.csv'), format='ascii.ecsv')
     with pytest.raises(DataFileFormatException):
-        efftab = InterpolateEfficiencyTable(get_pkg_data_filename('grating_efficiency_broken.csv'), k=2)
+        catgrating.InterpolateEfficiencyTable(tab, k=2)
+
+
+def test_catsupportbars():
+    photons = generate_test_photons(5)
+    p = catgrating.catsupportbars(photons.copy())
+    assert np.all(p['probability'] == 0)
+
+    photons['facet'] = np.arange(-1, 4)
+    p = catgrating.catsupportbars(photons)
+    assert np.all(p['probability'][1:] == 1)
+    assert p['probability'][0] == 0
```

### Comparing `marxs-1.2/marxs/optics/__init__.py` & `marxs-2.0/marxs/optics/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,12 +2,12 @@
 from .aperture import RectangleAperture, CircleAperture, MultiAperture
 from .detector import FlatDetector, CircularDetector
 from .marx import MarxMirror
 from .grating import (FlatGrating, CATGrating,
                       OrderSelector, EfficiencyFile
                       )
 from .mirror import ThinLens, PerfectLens
-from .baffle import Baffle
+from .baffles import Baffle
 from .scatter import RadialMirrorScatter, RandomGaussianScatter
 from .filter import EnergyFilter, GlobalEnergyFilter
 from .base import OpticalElement, FlatOpticalElement, FlatStack
 from .multiLayerMirror import FlatBrewsterMirror
```

### Comparing `marxs-1.2/marxs/optics/aperture.py` & `marxs-2.0/marxs/optics/aperture.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,21 +118,20 @@
     r_inner : float
         Inner radius for ring-like apertures. Default is 0 (full circle). If
         `r_inner` is non-zero, plotting the aperture will fill in the inner
         region.  If this is not desired because several `CircleApertures` are
         stacked into each other, ``self.display['inner_factor']`` can be used
         to restrict the radius range where the inner disk is displayed in a
         plot.
-
     '''
 
     default_geometry = CircularHole
 
     def __init__(self, **kwargs):
-        super(CircleAperture, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         if self.geometry['r_inner'] > np.linalg.norm(self.geometry['v_y']):
             raise ValueError('r_inner must be less than size of full aperture.')
 
         if not np.isclose(np.linalg.norm(self.geometry['v_y']),
                           np.linalg.norm(self.geometry['v_z'])):
             raise GeometryError('Aperture does not have the same size in y, z direction.')
 
@@ -185,15 +184,15 @@
     '''
     display = {'shape': 'container'}
 
     def __init__(self, **kwargs):
         self.elements = kwargs.pop('elements')
         self.id_col = kwargs.pop('id_col', 'aperture')
         self.id_num_offset = kwargs.pop('id_num_offset', 0)
-        super(MultiAperture, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         for i, elem in enumerate(self.elements):
             elem.id_col = self.id_col
             elem.id_num = self.id_num_offset + i
 
     @property
     def area(self):
         '''Area covered by the aperture'''
```

### Comparing `marxs-1.2/marxs/optics/baffle.py` & `marxs-2.0/marxs/optics/baffles.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/base.py` & `marxs-2.0/marxs/optics/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,57 @@
 import numpy as np
 from astropy.table import Table, Row
 
 from ..math.geometry import Geometry, FinitePlane
 from ..base import SimulationSequenceElement
 from ..simulator import BaseContainer
 
+
+def _assign_col_value(photons, col, index, value):
+    '''Assign new values to a subset of photons in a photon list
+
+    The column 'probability' receives special treatment: Probability values
+    are not replaced by the new numbers, but multiplied by the new numbers.
+    That way, a function just need to generate the *change in probability* and,
+    as a photon propagates through an instrument, all those changes multiply
+    together.
+
+    The probability column is also subject to extra checks because we want to
+    maintain probabilities between 0 and 1. In particular negative
+    probabilities can really cause problems later. Thus, this methods will
+    raise an Exception if probabilities are outside of the 0..1 range.
+    This can happen, for example, when an interpolation of a table goes wrong
+    or when numerical errors accumulate. In this case, the function that
+    generates the numbers for the probabilities in the first place, should
+    clip them to the allowed range.
+
+    Parameters
+    ----------
+    photons: `astropy.table.Table`
+        Table with photon properties
+    col : string
+        name of column
+    index : int or array
+        index of the photons that are assigned new values. Can be a single
+        number or a boolean array.
+    value : scalar or array
+        New valuees to the assigned to column `col`. If this is an array, it
+        needs to match the shape selected by the index array ``index``.
+    '''
+    if col == 'probability':
+        # Fix numerics of a probability
+        if np.any(value < 0) or np.any(value > 1):
+            raise ValueError('Found probability outside of the 0..1 arange.')
+        photons[col][index] *= value
+    elif col is None:
+        pass
+    else:
+        photons[col][index] = value
+
+
 class OpticalElement(SimulationSequenceElement):
     '''Base class for all optical elements in marxs.
 
     This class cannot be used to instanciate an optical element directly,
     rather it serves as a base class from with other optical elements will be
     derived.
 
@@ -39,15 +82,15 @@
 
         geometry = kwargs.pop('geometry', self.default_geometry)
         if isinstance(geometry, Geometry):
             self.geometry = geometry
         elif issubclass(geometry, Geometry):
             self.geometry = geometry(kwargs)
 
-        super(OpticalElement, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         if not hasattr(self, "loc_coos_name"):
             self.loc_coos_name = self.geometry.loc_coos_name
 
     @property
     def pos4d(self):
         return self.geometry.pos4d
@@ -126,49 +169,48 @@
             Table with photon properties.
             If possible, the input table is modified in place, but in some
             cases this might not be possible and the returned Table may be
             a copy. Do not rely on either - use ``photons.copy()`` if you want
             to ensure you are working with an independent copy.
 
         '''
-        if intersect.sum() > 0:
-            if hasattr(self, "specific_process_photons"):
-                outcols = self.specific_process_photons(photons, intersect, interpos, intercoos)
-                self.add_output_cols(photons, list(outcols.keys()))
-                for col in outcols:
-                    if col == 'probability':
-                        photons[col][intersect] *= np.asarray(outcols[col])
-                    else:
-                        photons[col][intersect] = outcols[col]
-
-            elif hasattr(self, "process_photon"):
-                if isinstance(photons, Row):
-                    photons = Table(photons)
-                outcols = ['dir', 'pos', 'energy', 'polarization', 'probability'] + self.output_columns
-                n_intersect = intersect.nonzero()[0]
-                for photon, i in zip(photons[intersect], n_intersect):
-                    outs = self.process_photon(photon['dir'], photon['pos'],
-                                               photon['energy'],
-                                               photon['polarization'])
-                    for a, b in zip(outcols, outs):
-                        if a == 'probability':
-                            photons['probability'][i] *= b
-                        else:
-                            photons[a][i] = b
-            else:
-                raise AttributeError('Optical element must have one of three: specific_process_photons, process_photon, or override process_photons.')
+        if intersect.sum() == 0:
+            return photons
+        if hasattr(self, "specific_process_photons"):
+            outcols = self.specific_process_photons(photons, intersect,
+                                                    interpos, intercoos)
+            self.add_output_cols(photons, list(outcols.keys()))
+            for col in outcols:
+                _assign_col_value(photons, col, intersect,
+                                  np.asarray(outcols[col]))
+
+        elif hasattr(self, "process_photon"):
+            if isinstance(photons, Row):
+                photons = Table(photons)
+            outcols = ['dir', 'pos', 'energy', 'polarization',
+                       'probability'] + self.output_columns
+            n_intersect = intersect.nonzero()[0]
+            for photon, i in zip(photons[intersect], n_intersect):
+                outs = self.process_photon(photon['dir'], photon['pos'],
+                                           photon['energy'],
+                                           photon['polarization'])
+                for col, b in zip(outcols, outs):
+                    _assign_col_value(photons, col, i, b)
+        else:
+            raise AttributeError('Optical element must have one of three: specific_process_photons, process_photon, or override process_photons.')
 
+        if self.loc_coos_name is not None:
             self.add_output_cols(photons, self.loc_coos_name)
-            # Add ID number to ID col, if requested
-            if self.id_col is not None:
-                photons[self.id_col][intersect] = self.id_num
-            # Set position in different coordinate systems
-            photons['pos'][intersect] = interpos[intersect]
             photons[self.loc_coos_name[0]][intersect] = intercoos[intersect, 0]
             photons[self.loc_coos_name[1]][intersect] = intercoos[intersect, 1]
+        # Add ID number to ID col, if requested
+        if self.id_col is not None:
+            photons[self.id_col][intersect] = self.id_num
+        # Set position in different coordinate systems
+        photons['pos'][intersect] = interpos[intersect]
 
         return photons
 
 
 class FlatOpticalElement(OpticalElement):
     pass
 
@@ -204,36 +246,39 @@
     ...     keywords=[{'filterfunc': lambda x: 0.5}, {'pixsize': 0.05}])
 
     '''
 
     def __init__(self, **kwargs):
         elements = kwargs.pop('elements')
         keywords = kwargs.pop('keywords')
-        super(FlatStack, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.elements = []
         for elem, k in zip(elements, keywords):
             self.elements.append(elem(pos4d=self.pos4d, **k))
 
     def specific_process_photons(self, *args, **kwargs):
         return {}
 
-    def process_photons(self, photons, intersect=None, interpos=None, intercoos=None):
-        '''
-        Parameters
+    def process_photons(self, photons, intersect=None, interpos=None,
+                        intercoos=None):
+        '''Parameters
         ----------
         intersect, interpos, intercoos : array (N, 4)
-            The array ``interpos`` contains the intersection points in the global
-            coordinate system, ``intercoos`` in the local (y,z) system of the grating.
+            The array ``interpos`` contains the intersection points in
+            the global coordinate system, ``intercoos`` in the local
+            (y,z) system of the grating.
+
         '''
         if intersect.sum() > 0:
             # This line calls FlatOpticalElement.process_photons to add ID cols
             # and local coos if requested (this could also be done by any of
             # the contained sequence elements, but we want the user to be able
             # to specify that for either of them).
-            photons = super(FlatStack, self).process_photons(photons, intersect, interpos, intercoos)
+            photons = super().process_photons(photons, intersect, interpos,
+                                              intercoos)
             for e in self.elements:
                 photons = e.process_photons(photons, intersect, interpos, intercoos)
 
         return photons
 
 
 def photonlocalcoords(f, colnames=['pos', 'dir']):
```

### Comparing `marxs-1.2/marxs/optics/cdef.txt` & `marxs-2.0/marxs/optics/cdef.txt`

 * *Files 1% similar despite different names*

```diff
@@ -100,12 +100,11 @@
 #define MARX_ORDER3_OK                0x00800000
 #define MARX_ORDER4_OK                0x01000000
 
    unsigned int tag_start;               /* start tag for this group */
 }
 Marx_Photon_Type;
 
-double Marx_Mirror_Geometric_Area = 1;
+extern double Marx_Mirror_Geometric_Area = 1;
 
 int marx_mirror_init (Param_File_Type *pf);
 int marx_mirror_reflect (Marx_Photon_Type *p, int verbose);
-
```

### Comparing `marxs-1.2/marxs/optics/data/A12113.txt` & `marxs-2.0/marxs/optics/data/A12113.txt`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/data/A13164.txt` & `marxs-2.0/marxs/optics/data/A13164.txt`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/data/A14070B.txt` & `marxs-2.0/marxs/optics/data/A14070B.txt`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/data/A14080B.txt` & `marxs-2.0/marxs/optics/data/A14080B.txt`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/data/ALSpolarization.txt` & `marxs-2.0/marxs/optics/data/ALSpolarization.txt`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/data/ALSpolarization2.txt` & `marxs-2.0/marxs/optics/data/ALSpolarization2.txt`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/filter.py` & `marxs-2.0/marxs/optics/filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 '''This module contains filters, e.g. an optical blocking filter or CCD contamination.
 '''
 import numpy as np
 
-from .base import OpticalElement, FlatOpticalElement
+from .base import FlatOpticalElement
 from ..base import MarxsElement
-from ..math.geometry import NoGeometry
+
 
 class GlobalEnergyFilter(MarxsElement):
     '''Energy dependent filter that globally affects all photons.
 
-    This element is used on all photons in the list, there is no geometrical
-    position associated with it. Consequently, there is no update of the position
-    or direction for each photon.
-    Use this element for global filters, that are not directly associated with any particular
-    physical object, e.g. to apply a energy based mirror efficiency after
-    passing the photons through one of the perfect efficiency mirror models.
+    This element is used on all photons in the list, there is no
+    geometrical position associated with it. Consequently, there is no
+    update of the position or direction for each photon.  Use this
+    element for global filters, that are not directly associated with
+    any particular physical object, e.g. to apply a energy based
+    mirror efficiency after passing the photons through one of the
+    perfect efficiency mirror models.
 
     Parameters
     ----------
     filterfunc : callable
         A function that calculates the probability for each photon to pass
         through the filter based on the photon energy in keV. The function
         signature should be ``p = func(en)``, where ``p, en`` are 1-d arrays
@@ -33,22 +34,23 @@
     >>> filtercurve = [.1, .5, .9, .9, .5]
     >>> f = interp1d(energygrid, filtercurve)
     >>> blockingfilter = GlobalEnergyFilter(filterfunc=f)
 
     See Also
     --------
     marxs.optics.filter.EnergyFilter
+
     '''
 
     def __init__(self, **kwargs):
         self.filterfunc = kwargs.pop('filterfunc')
-        super(GlobalEnergyFilter, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __call__(self, photons):
-        p =  self.filterfunc(photons['energy'])
+        p = self.filterfunc(photons['energy'])
         if np.any(p < 0.) or np.any(p > 1.):
             raise ValueError('Probabilities returned by filterfunc must be in interval [0, 1].')
         photons['probability'] *= p
         return photons
 
 
 class EnergyFilter(FlatOpticalElement):
@@ -75,17 +77,18 @@
     --------
     marxs.optics.filter.GlobalEnergyFilter
     '''
 
     display = {'color': (1.0, 0., 0.),
                'opacity': 0.5,
                'shape': 'box',
-    }
+               }
+
     def __init__(self, **kwargs):
         self.filterfunc = kwargs.pop('filterfunc')
-        super(EnergyFilter, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def specific_process_photons(self, photons, intersect, interpos, intercoos):
         p =  self.filterfunc(photons['energy'][intersect])
         if np.any(p < 0.) or np.any(p > 1.):
             raise ValueError('Probabilities returned by filterfunc must be in interval [0, 1].')
         return {'probability': p}
```

### Comparing `marxs-1.2/marxs/optics/grating.py` & `marxs-2.0/marxs/visualization/utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,290 +1,331 @@
 # Licensed under GPL version 3 - see LICENSE.rst
-'''Gratings and efficiency files'''
-import math
+'''This module collects helper functions for visualization backends.
+
+The functions here are not intended to be called directly by the
+user. Instead, they refractor common tasks that are used in several
+visualization backends.
+'''
+import warnings
 import numpy as np
-from numpy.core.umath_tests import inner1d
 
-from ..math.utils import norm_vector, h2e, e2h
-from ..math.polarization import parallel_transport
-from .. import energy2wave
-from .base import FlatOpticalElement
+from marxs.math import utils as mutils
 
 
-class OrderSelector(object):
-    '''Select from a list of order numbers independent of energy.
+class MARXSVisualizationWarning(Warning):
+    '''Warning class for MARXS objects missing from plotting'''
+    pass
+
+
+def get_obj_name(obj):
+    '''Return printable name for objects or functions.'''
+    if hasattr(obj, 'name'):
+        return obj.name
+    elif hasattr(obj, 'func_name'):
+        return obj.func_name
+    else:
+        return str(obj)
+
+
+class DisplayDict(dict):
+    '''A dictionary to store how an element is displayed in plotting.
+
+    A dictionary of this type works just like a normal dictionary,
+    except for an additional look-up step for keys that are not found
+    in the dictionary itself.  A ``DisplayDict`` is initialized with a
+    reference to the object it describes and any parameter accessed
+    from ``DisplayDict`` that is not found in the dictionary will be
+    searched for in the object's geometry. This allows us to set any
+    and all display settings in the ``DisplayDict`` to customize
+    plotting in any way without affecting how the ray-trace is run
+    (which uses only the parameters set in the geoemtry), but for
+    those values that are not set, fall back to the settings of the
+    geometry (e.g. the shape of an object is typically taken from the
+    geometry, while the color is not).
 
     Parameters
     ----------
-    orderlist : array
-        This are the order numbers to chose from. They must be integers.
-    p : None or array
-        Probability for a photon to end up in each order. The sum of all probabilities
-        can be smaller than 1, if a certain fraction of photons is absorbed by
-        the grating. If this is ``None``, equal probability is assigned to all orders.
-
-    Examples
-    --------
-    Two common use cases for testing are a grating where every photon gets
-    diffracted into the same order or where all photons get distributed with
-    equal probability into a set of orders.
+    parent : `marxs.base.MarxsElement`
+        Reference to the object that is described by this ``DisplayDict``
+    args, kwargs: see `dict`
 
-    >>> import numpy as np
-    >>> from marxs.optics import FlatGrating, OrderSelector
-    >>> singleordergrating = FlatGrating(d=1e-4, order_selector=OrderSelector([3]))
-    >>> setofordersgrating = FlatGrating(d=1e-4, order_selector=OrderSelector(np.arange(-3, 4)))
     '''
-    def __init__(self, orderlist, p=None):
-        self.orderlist = orderlist
-        if p is None:
-            self.p = np.ones(len(orderlist)) / len(orderlist)
-        else:
-            p = np.asanyarray(p)
-            if len(p) != len(orderlist):
-                raise ValueError('Number of elements in orderlist and probabilities does not match.')
-            if p.sum() > 1.:
-                raise ValueError('Sum of all probabilities must be <= 1.')
-            if np.any(p < 0):
-                raise ValueError('Probabilities cannot be negative')
-            self.p = p
-
-    def __call__(self, energy, *args):
-        p_sum = self.p.sum()
-        p = self.p / p_sum
-        if np.isscalar(energy):
-            return np.random.choice(self.orderlist, p=p), self.p.sum()
+    def __init__(self, parent, *args, **kwargs):
+        self.parent = parent
+        super().__init__(*args, **kwargs)
+
+    def __getitem__(self, key):
+        if (key not in self) and hasattr(self.parent, 'geometry'):
+            try:
+                return getattr(self.parent.geometry, key)
+            except AttributeError:
+                raise KeyError(key)
         else:
-            return np.random.choice(self.orderlist, size=len(energy), p=p), p_sum * np.ones_like(energy)
+            return super().__getitem__(key)
 
+    def get(self, k, d=None):
+        '''D.get(k[,d]) -> D[k] if k in D, else d.  d defaults to None.'''
+        try:
+            return self[k]
+        except KeyError:
+            return d
 
-class EfficiencyFile(object):
-    '''Select grating order from a probability distribution in a data file.
 
-    The file format supported by this class is as follows:
-    The first colum contains energy values in keV, all remaining columns have the probability
-    that a photons with this energy is diffracted into the respective order. The probabilities
-    for each order do not have to add up to 1.
+def plot_object_general(plot_registry, obj, display=None, **kwargs):
+    '''Look up a plotting routine for an object and execute it.
+
+    This function is not meant to be called directly by the user, instead, it
+    is designed to simplify the implementation of new plotting backends.
 
     Parameters
     ----------
-    filename : string
-        Path to the efficiency file.
-    orders : list
-        List of orders in the file. Must match the number of columns with probabilities.
+    plot_registry : dict
+        Keys are the names of the shape of an object and values in this
+        dictionary are functions that know how to plot this type of shape. The
+        appropriate plotting function is then called with the input `obj`,
+        `display` and any other keyword arguments.
+        If the shape is ``"None"`` (as a string), no plotting function is
+        called.
+    obj : `marxs.base.MarxsElement`
+        The element that should be plotted.
+    display : dict of None
+        Dictionary with display settings. If this is ``None``, ``obj.display``
+        is used. If that is also ``None`` then the objects is skipped.
+    kwargs : other keyword arguments
+        These arguments are just passed through to the plotting function.
+
+    Returns
+    -------
+    out : backend-dependent
+        The output from the plotting function that was executed is passed
+        through.  Different plotting backends return different kinds of output.
     '''
-    def __init__(self, filename, orders):
-        dat = np.loadtxt(filename)
-        self.energy = dat[:, 0]
-        if len(orders) != (dat.shape[1] - 1):
-            raise ValueError('orders has len={0}, but data files has {1} order columns.'.format(len(orders), dat.shape[1] - 1))
-        self.orders = np.array(orders)
-        self.prob = dat[:, 1:]
-        # Probability to end up in any order
-        self.totalprob = np.sum(self.prob, axis=1)
-        # Cumulative probability for orders, normalized to 1.
-        self.cumprob = np.cumsum(self.prob, axis=1) / self.totalprob[:, None]
-
-    def __call__(self, energies, *args):
-        orderind = np.empty(len(energies), dtype=int)
-        ind = np.empty(len(energies), dtype=int)
-        for i, e in enumerate(energies):
-            ind[i] = np.argmin(np.abs(self.energy - e))
-            orderind[i] = np.min(np.nonzero(self.cumprob[ind[i]] > np.random.rand()))
-        return self.orders[orderind], self.totalprob[ind]
+    if display is None:
+        if hasattr(obj, 'display') and (obj.display is not None):
+            display = obj.display
+        else:
+            warnings.warn('Skipping {0}: No display dictionary found.'.format(
+                get_obj_name(obj)),
+                          MARXSVisualizationWarning)
+            return None
+
+    try:
+        shape = display['shape']
+    except KeyError:
+        warnings.warn('Skipping {0}: "shape" not set in display dict.'.format(
+            get_obj_name(obj)),
+                      MARXSVisualizationWarning)
+        return None
+
+    shapes = [s.strip() for s in shape.split(';')]
+    for s in shapes:
+        if s == 'None':
+            return None
+        elif s in plot_registry:
+            # turn into valid color tuple
+            display['color'] = get_color(display)
+            return plot_registry[s](obj, display,  **kwargs)
+    else:
+        warnings.warn('Skipping {0}: No function to plot {1}.'.format(
+            get_obj_name(obj), shape),
+                      MARXSVisualizationWarning)
+        return None
+
+
+def get_color(d):
+    '''Look for color information in dictionary.
+
+    If missing, return white.
+    This function checks if the `d['color']` is a valid RGB tuple and if
+    not it imports a `matplotlib.colors.ColorConverter` to convert any
+    matplotlib compatible string to an RGB tuple.
 
+    Parameters
+    ----------
+    d : dict
+        Color information should be present in ``d['color']``.
 
+    Returns
+    -------
+    color : tuple
+        RGB tuple with each element in the range 0..1
+    '''
+    if 'color' not in d:
+        return (1., 1., 1.)
+    else:
+        c = d['color']
+        # check if this is a tuple of three floats n the range 0..1
+        # or can be converted to one
+        try:
+            cout = tuple(c)
+            if len(cout) != 3:
+                raise TypeError
+            for a in cout:
+                if not isinstance(a, float) or (a < 0.) or (a > 1.):
+                    raise TypeError
+            return cout
+        except TypeError:
+            # It's a hex or string. Let matplotlib deal with that.
+            import matplotlib.colors
+            return matplotlib.colors.colorConverter.to_rgb(c)
 
-class FlatGrating(FlatOpticalElement):
-    '''Flat grating
 
-    The grating is assumed to be geometrically thin, i.e. all photons enter on
-    the face of the grating, not through the sides.
+def color_tuple_to_hex(color):
+    '''Convert color tuple to hex string.
 
     Parameters
     ----------
-    d : float or callable
-        grating constant in mm. If ``d`` is callable, then it will be called as
-        ``d(intercoos)``, where ``intercoos`` is a (N, 2) array holding the
-        positions where photons hit the gratings in the local coordinate system.
-        This can be used to simulate manufacturing uncertainties or intentional
-        grating period variation. The callable has to return a vector of lengths N
-        that contains the grating constant for each photon in mm.
-    order_selector : callable
-        A function or callable object that accepts arrays of photon
-        energy, polarization and the blaze angle as input and returns
-        arrays for grating order (integer) and probability
-        (float). The probabiliy expresses the chance that the photon
-        passes the grating and is not absorbed, e.g. if the
-        probability that a photon at energy E ends up in order=[-2,
-        -1, 0, 1, 2] is [0, 0, .5, .3, .0] , then the returned
-        probability for all photons should be 0.8.
-    transmission : bool
-        Set to ``True`` for a transmission grating and to ``False`` for a
-        reflection grating. (*Default*: ``True`` ) **Warning: Reflection
-        gratings have not yet been tested**
-    groove_angle : float
-        Angle between the local z axis and the direction of the
-        grooves in radian.  (*Default*: ``0.``)
+    color : tuple
+        tuple has three elements (rgb) that are floats between 0 and 1
+        or ints between 0 and 255.
+
+    Returns
+    -------
+    hexstring : string
+        string encoding that number as hex
     '''
+    if all([isinstance(a, float) for a in color]):
+        if any(i < 0. for i in color) or any(i > 1. for i in color):
+            raise ValueError('Float values in color tuple must be between 0 and 1.')
+        out = hex(int(color[0] * 256**2 * 255 +
+                      color[1] * 256 * 255 +
+                      color[2] * 255))
+    elif all([isinstance(a, int) for a in color]):
+        if any(i < 0 for i in color) or any(i > 255 for i in color):
+            raise ValueError('Int values in color tuple must be between 0 and 255.')
+        out = hex(color[0] * 256**2 + color[1] * 256 + color[2])
+    else:
+        raise ValueError('Input tuple must be all float or all int.')
+    # Now pad with zeros if required
+    return out[:2] + out[2:].zfill(6)
 
-    loc_coos_name = ['grat_y', 'grat_z']
-    '''name for output columns that contain the interaction point in local coordinates.'''
 
-    order_name = 'order'
-    '''Column name for diffraction order. If set to ``None`` this is not added to the photon list.'''
+def plane_with_hole(outer, inner):
+    '''Triangulation of a plane with an inner hole
 
-    blaze_name = 'blaze'
-    '''Column name for blaze angle. If set to ``None`` this is not added to the photon list.'''
+    This function constructs a triangulation for a plane with an inner
+    hole, e.g. a rectangular plane where an inner circle is cut out.
 
-    def order_sign_convention(self, p, e_perp_groove):
-        '''Set sign convention for grating orders.
-
-        This sets the following, somewhat arbitrary convention:
-        Positive grating orders will are displaced along the local
-        :math:`\hat e_z` vector, negative orders in the opposite
-        direction. If the grating is rotated by :math:`-\pi` the
-        physical situation is the same, but the sign of the grating
-        order will be reversed.  In this sense, the convention chosen
-        is arbitrarily. However, it has some practical advantages: The
-        implementation is fast and all photons passing through the
-        grating in the same diffraction order are displaced in the
-        same way. (Contrary to the convention in :class:`CATGrating`.)
-        ``order_sign_convention`` has to be a callable that accepts an
-        array of eukledian direction vectors as input and returns
-        ``+1``, ``-1``, or an array filled with ``-1`` or ``+1``.
-
-        Parameters
-        ----------
-        p : np.array
-            Array of Eucleadian direction vectors
-        e_perp_groove : np.array
-            Array of local groove directions at the positions where the photons hit
-        '''
-        # -1 because n, l, d should be right-handed coordinate system
-        # while n = e_x, l = e_x, and d = e_y would be left-handed.
-        return -1
-
-    def __init__(self, **kwargs):
-        self.order_selector = kwargs.pop('order_selector')
-        self.transmission = kwargs.pop('transmission', True)
-        if 'd' not in kwargs:
-            raise ValueError('Input parameter "d" (Grating constant) is required.')
-        self._d = kwargs.pop('d')
-        groove_angle = kwargs.pop('groove_angle', 0.)
-
-        super(FlatGrating, self).__init__(**kwargs)
-
-        self.geometry._geometry['groove_angle'] = groove_angle
-
-    def e_groove_coos(self, intercoos):
-        '''Get coordiante orthonormal coordinate system along groove direction.
-
-        Parameters
-        ----------
-         intercoos : `numpy.ndarray` of shape (N, 2)
-            coordinates in the coordiante system of the geometry (e.g. (x, y), or
-            (r, phi)).
-
-        Returns
-        -------
-        e_groove, e_perp_groove, n : `numpy.ndarray` of shape (N, 4)
-            Vectors pointing along the groove direction (parallel to the surface),
-            perpendicular to the groove direction (parallel to surface),
-            and normal to surface.
-        '''
-
-        groove = self.geometry['groove_angle']
-        ex, ey, en = self.geometry.get_local_euklid_bases(intercoos)
-        e_groove = math.sin(-groove) * ex + math.cos(-groove) * ey
-        e_perp_groove = math.cos(-groove) * ex - math.sin(-groove) * ey
-        return e_groove, e_perp_groove, en
-
-    def d(self, intercoos):
-        '''Method that returns the grating constant at given positions.
-
-        For a grating with constant grating constant, this will just return the
-        number input as ``d`` when the element was initialized. For gratings
-        where the grating constant varies with position on the facet, this
-        calculates the appropriate number for every position.
-        '''
-        if not callable(self._d):
-            return self._d
-        else:
-            return self._d(intercoos)
+    Parameters
+    ----------
+    outer, inner : np.ndarray of shape (n, 3)
+        Coordinates in x,y,z of points that define the inner and outer
+        boundary.  ``outer`` and ``inner`` can have a different number of
+        points, but points need to be listed in the same orientation
+        (e.g. clockwise) for both and the starting points need to have a
+        similar angle as seen from the center (e.g. for a plane with z=0, both
+        ``outer`` and ``inner`` could list a point close to the y-axis first.
+
+    Returns
+    -------
+    xyz : nd.array
+        stacked ``outer`` and ``inner``.
+    triangles : nd.array
+        List of the indices. Each row has the index of three points in ``xyz``.
+
+    Examples
+    --------
+    In this example, we make a square and cut out a smaller square in the
+    middle.
 
-    def blaze_angle_modifier(self, intercoos):
-        '''Modify blaze angle
+    >>> import numpy as np
+    >>> from marxs.visualization.utils import plane_with_hole
+    >>> outer = np.array([[-1, -1, 1, 1], [-1, 1, 1, -1], [0,0,0,0]]).T
+    >>> inner = 0.5 * outer
+    >>> xyz, triangles = plane_with_hole(outer, inner)
+    >>> triangles
+    array([[0, 4, 5],
+       [0, 1, 5],
+       [1, 5, 6],
+       [1, 2, 6],
+       [2, 6, 7],
+       [2, 3, 7],
+       [3, 7, 4],
+       [3, 0, 4]])
 
-        In `diffract_photons` the blaze angle is calculated relative to the surface
-        of the grating. In cases where that number has to be modified (e.g. when the grating
-        bars are not perpendicualr to the surface) the blaze angle can be modified by
-        overriding this function.
-        '''
-        return np.zeros(intercoos.shape[0])
-
-    def diffract_photons(self, photons, intersect, interpos, intercoos):
-        '''Vectorized implementation'''
-        p = norm_vector(photons['dir'].data[intersect])
-        l, d, n = self.e_groove_coos(intercoos[intersect])
-        # Minus sign here because we want n, l, d to be a right-handed coordinate system
-        d = - d
-
-        wave = energy2wave / photons['energy'].data[intersect]
-        # calculate angle between normal and (ray projected in plane perpendicular to groove)
-        # -> this is the blaze angle
-        p_perp_to_grooves = norm_vector(p - inner1d(p, l)[:, None] * l)
-        # Use abs here so that blaze angle is always in 0..pi/2
-        # independent of the relative orientation of p and n.
-        blazeangle = np.arccos(np.abs(inner1d(p_perp_to_grooves, n)))
-        blazeangle += self.blaze_angle_modifier(intercoos[intersect, :])
-        m, prob = self.order_selector(photons['energy'].data[intersect],
-                                      photons['polarization'].data[intersect],
-                                      blazeangle)
-
-        # The idea to calculate the components in the (d,l,n) system separately
-        # is taken from MARX
-        sign = self.order_sign_convention(p, d)
-        p_d = inner1d(p, d) + sign * m * wave / self.d(intercoos[intersect, :])
-        p_l = inner1d(p, l)
-        # The norm for p_n can be derived, but the direction needs to be chosen.
-        p_n = np.sqrt(1. - p_d**2 - p_l**2)
-        # Check if the photons have same direction compared to normal before
-        direction = np.sign(inner1d(p, n), dtype=np.float)
-        if not self.transmission:
-            direction *= -1
-        dir = p_d[:, None] * d + p_l[:, None] * l + (direction * p_n)[:, None] * n
-        return dir, m, prob, blazeangle
-
-    def specific_process_photons(self, photons, intersect, interpos, intercoos):
-
-        dir, m, p, blaze = self.diffract_photons(photons, intersect, interpos, intercoos)
-        pol = parallel_transport(photons['dir'].data[intersect, :], dir,
-                                 photons['polarization'].data[intersect, :])
-        out = {'dir': dir, 'probability': p, 'polarization': pol}
-        if self.order_name is not None:
-            out[self.order_name] = m
-        if self.blaze_name is not None:
-            out[self.blaze_name] = blaze
-        return out
-
-
-class CATGrating(FlatGrating):
-    '''Critical-Angle-Transmission Grating
-
-    CAT gratings are a special case of :class:`FlatGrating` and accept the same arguments.
-
-    They differ from a :class:`FlatGrating` in the sign convention of the
-    grating orders: Blazing happens on the side of the negative orders. Obviously, this
-    convention is only meaningful if the photons do not arrive perpendicular to the grating.
     '''
+    n_out = outer.shape[0]
+    n_in = inner.shape[0]
+    n = n_out + n_in
+
+    triangles = np.zeros((n, 3), dtype=int)
+    xyz = np.vstack([outer, inner])
+
+    i_in = 0
+    i_out = 0
+    for i in range(n_out + n_in):
+        if i/n >= i_in/n_in:
+            triangles[i, :] = [i_out, n_out + i_in,
+                               n_out + ((i_in + 1) % n_in)]
+            i_in += 1
+        else:
+            triangles[i, :] = [i_out, (i_out + 1) % n_out,
+                               n_out + (i_in % n_in)]
+            i_out = (i_out + 1) % n_out
+    return xyz, triangles
 
 
-    def order_sign_convention(self, p, e_perp_groove):
-        '''Convention to chose the sign for CAT grating orders
+def combine_disjoint_triangulations(list_xyz, list_triangles):
+    '''Combine two disjoint triangulations into one set of points
+
+    This function combines two entirely separate triangulations into
+    one set of point and triangles. Plotting the combined
+    triangulation should have the same effect as plotting each
+    triangulation separately. This function is used for plotting
+    apertures where we have e.g. an open ring. This can be plotted as
+    an inner circle plus an outer shape with a hole in it.
 
-        Blazing happens on the side of the negative orders. Obviously, this
-        convention is only meaningful if the photons do not arrive perpendicular to the grating.
-        '''
-        dotproduct = inner1d(p, e_perp_groove)
-        sign = np.sign(dotproduct)
-        sign[sign == 0] = 1
-        return sign
+    Parameters
+    ----------
+    list_xyz : list of `np.array`
+        Each array holds xyz values for one triangulation
+    list_triangles : list of nd.array
+        Each array holds the list of the indices for one triangulation.
+
+    Returns
+    -------
+    xyz : nd.array
+        stacked ``outer`` and ``inner``.
+    triangles : nd.array
+        List of the indices. Each row has the index of three points in ``xyz``.
+
+    '''
+    xyz = np.vstack(list_xyz)
+    n_offset = np.cumsum([a.shape[0] for a in list_xyz])
+    n_offset -= n_offset[0]
+    triangles = np.vstack([list_triangles[i] + n_offset[i] for i in
+                           range(len(n_offset))])
+    return xyz, triangles
+
+
+def triangulate_parametricsurface(xyz):
+    xyz = mutils.h2e(xyz)
+    xyz = xyz.reshape(-1, 3)
+    index = np.arange(xyz.shape[0] - 2)
+    indarr = np.vstack([index, index + 1, index + 2]).T
+    return xyz, indarr
+
+
+def halfbox_corners(obj, display):
+    corners = np.array([[-1, -1, -1], [-1,+1, -1],
+                        [-1, -1,  1], [-1, 1,  1],
+                        [ 1, -1, -1], [ 1, 1, -1],
+                        [ 1, -1, +1], [ 1, 1, +1]])
+    if 'box-half' in display:
+        # write in a way that it works with any value for that keyword
+        try:
+            if display['box-half'][0] == '+':
+                factor = +1
+            elif display['box-half'][0] == '-':
+                factor = -1
+            else:
+                factor = 0
+            xyz = {'x': 0, 'y': 1, 'z': 2}
+            if display['box-half'][1] in xyz:
+                j = xyz[display['box-half'][1]]
+                corners[corners[:, j] == factor, j] = 0
+        except:
+            pass
+
+    corners = np.einsum('ij,...j->...i', obj.pos4d, mutils.e2h(corners, 1))
+    corners = mutils.h2e(corners)
+    return corners
```

### Comparing `marxs-1.2/marxs/optics/hrma.par` & `marxs-2.0/marxs/optics/hrma.par`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/marx.py` & `marxs-2.0/marxs/optics/marx.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,16 +25,16 @@
     '''Error in the compiled Marx C module'''
     pass
 
 
 class MarxMirror(OpticalElement, BaseAperture):
     '''Interface to MARX mirror module
 
-    This class provides an interface to the `MARX <http://space.mit.edu/ASC/marx/>`_
-    mirror module. It requires
+    This class provides an interface to the
+    `MARX <http://space.mit.edu/ASC/marx/>`_  mirror module. It requires
     both the MARX source code and compiled MARX binaries as explained in the
     :ref:`Installation instructions for MARXS <sect-installmarxccode>`
     When this model
     is initialized, it requires the path and filename to a MARX setup file.
 
     The default geometry is such that the focal point is at the origin of the
     coordinate system and the optical axis is along the x-axis, such that
@@ -71,15 +71,15 @@
         else:
             self.parfile = parfile
         self.cparfile = marx.pf_open_parameter_file(bytes(parfile, 'utf8'), bytes('r', 'utf8'))
         out = marx.marx_mirror_init(self.cparfile)
         if out < 0:
             raise MarxError('Mirror cannot be initialized. Probably missing parameters or syntax error in {0}.'.format(parfile))
 
-        super(MarxMirror, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @staticmethod
     def _table2c(photons):
         # Arrays assigned here in python need to keep a reference
         # somewhere, otherwise they would be garbage collected
         # and the pointer would suddenly be invalid.
         # To do so, this function adds them to the photons table header.
@@ -114,15 +114,15 @@
 
         sorted_index = np.argsort(photons['energy'].data)
         sorted_index = np.ascontiguousarray(sorted_index, dtype=np.uintc)
         keep_cffi_pointers['sorted_index'] = sorted_index  # keep alive
         c_photon_list.sorted_index = ffi.cast('unsigned int*', sorted_index.ctypes.data)
 
         sorted_energies = np.sort(photons['energy'].data)
-        sorted_energies = np.ascontiguousarray(sorted_energies, dtype=np.float)
+        sorted_energies = np.ascontiguousarray(sorted_energies, dtype=float)
         keep_cffi_pointers['sorted_energies'] = sorted_energies  # keep alive
         c_photon_list.sorted_energies = ffi.cast('double*', sorted_energies.ctypes.data)
 
         c_photon_list.num_sorted = n  # all photons in list are valid
         # Fields not mentioned here are irrelevant for the mirror
         # module and can have any value they are initialized to.
```

### Comparing `marxs-1.2/marxs/optics/marx_build.py` & `marxs-2.0/marxs/optics/marx_build.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 from os import path
 from configparser import ConfigParser
 from cffi import FFI
 
-with open ("marxs/optics/cdef.txt", "r") as myfile:
+with open (path.join(path.dirname(__file__), "cdef.txt"), "r") as myfile:
     cdeftxt=myfile.read()
 
 ffi = FFI()
 ffi.cdef(cdeftxt)
 
 
 conf = ConfigParser()
 # When setup.py is run, then setup.cfg is in the current directory
 # However, when runngin this in pytest, it's in ../
 # So offer both options here (files not found are silently ignored).
-conf.read(['setup.cfg', '../setup.cfg'])
+conf.read(['setup.cfg', '../setup.cfg', '../../setup.cfg'])
 marxscr = conf.get('MARX', 'srcdir')
 marxlib = conf.get('MARX', 'libdir')
 
 sources = [('pfile', 'src', 'pfile.c'), ('marx', 'libsrc', 'mirror.c')]
 headers = [('pfile', 'src'), ('jdmath', 'src') , ('jdfits', 'src'),
            ('marx', 'src',), ('marx', 'libsrc',), ('src',), ('libsrc',)]
```

### Comparing `marxs-1.2/marxs/optics/multiLayerMirror.py` & `marxs-2.0/marxs/optics/multiLayerMirror.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,49 +5,54 @@
 from .base import FlatOpticalElement, FlatStack
 from ..math.utils import norm_vector, e2h, h2e
 
 
 class FlatBrewsterMirror(FlatOpticalElement):
     '''Flat mirror operated at the Brewster angle.
 
-    Calculation of the Fresnel coefficients can be computationally intense
-    and also requires knowledge of the refractive index for the appropriate material.
-    The ``FlatBrewsterMirror`` simplifies this for a mirror that is known to be
-    operated at the Brewster angle.
+    Calculation of the Fresnel coefficients can be computationally
+    intense and also requires knowledge of the refractive index for
+    the appropriate material.  The ``FlatBrewsterMirror`` simplifies
+    this for a mirror that is known to be operated at the Brewster
+    angle.
 
     This mirror assumes that all photons arrive at the Brewster angle
-    where only s (senkrecht = direction perpendicular to plane of incidence)
-    polarisation is reflected.
-    It also assumes that all photons that are not reflected (i.e. those that
-    are transmitted) are lost. No transmitted photons are returned, instead the
-    probability of the reflected photons is adjusted to account for this overall loss.
+    where only s (senkrecht = direction perpendicular to plane of
+    incidence) polarisation is reflected.  It also assumes that all
+    photons that are not reflected (i.e. those that are transmitted)
+    are lost. No transmitted photons are returned, instead the
+    probability of the reflected photons is adjusted to account for
+    this overall loss.
+
     '''
     display = {'color': (0., 1., 0.),
                'shape': 'box',
                'box-half': '+x',
-    }
+               }
 
     def fresnel(self, photons, intersect, intersection, local):
         '''The incident angle can easily be calculated from e_x and photons['dir'].
 
         Returns
         -------
         refl_s, refl_p : np.array or float
             Reflection probability for s and p polarized photons.
             Typically, the number will depend on the incident angle and energy
             of each photon and thus the return value will be a vector.
         '''
         return 1., 0.
 
-    def specific_process_photons(self, photons, intersect, intersection, local):
+    def specific_process_photons(self, photons, intersect, intersection,
+                                 local):
         directions = norm_vector(photons['dir'].data[intersect])
         # save the direction of the incoming photons as beam_dir
         beam_dir = h2e(directions)
 
-        # reflect the photons (change direction) by transforming to local coordinates
+        # reflect the photons (change direction) by transforming to
+        # local coordinates
         pos4d_inv = np.linalg.inv(self.pos4d)
         directions = directions.T
         directions = np.dot(pos4d_inv, directions)
         directions[0, :] *= -1
         directions = np.dot(self.pos4d, directions)
         new_beam_dir = directions.T
 
@@ -60,27 +65,33 @@
         v_s /= np.linalg.norm(v_s, axis=1)[:, np.newaxis]
         v_p = np.cross(beam_dir, v_s)
 
         polarization = h2e(photons['polarization'].data[intersect])
         p_v_s = np.einsum('ij,ij->i', polarization, v_s)
         p_v_p = np.einsum('ij,ij->i', polarization, v_p)
 
-        fresnel_refl_s, fresnel_refl_p = self.fresnel(photons, intersect, intersection, local)
+        fresnel_refl_s, fresnel_refl_p = self.fresnel(photons, intersect,
+                                                      intersection, local)
         # Calculate new intensity ~ (E_x)^2 + (E_y)^2
         Es2 = fresnel_refl_s * p_v_s ** 2
         Ep2 = fresnel_refl_p * p_v_p ** 2
+        intensity = Es2 + Ep2
+        # Sometimes, the numerics in the square make probabilities > 1
+        # So, we clip, but raise an error is it's >> 1
+        if np.any(intensity > 1.001):
+            raise ValueError('Intensity cannot be > 1')
 
         # parallel transport of polarization vector
         # v_s stays the same by definition
         new_v_p = np.cross(h2e(new_beam_dir), v_s)
-        new_pol = norm_vector(-Es2[:, np.newaxis] * v_s  + Ep2[:, np.newaxis] * new_v_p)
-
+        new_pol = norm_vector(-Es2[:, np.newaxis] * v_s +
+                              Ep2[:, np.newaxis] * new_v_p)
 
         return {'dir': new_beam_dir,
-                'probability': Es2 + Ep2,
+                'probability': np.clip(intensity, 0, 1),
                 'polarization': e2h(new_pol, 0)}
 
 
 class MultiLayerEfficiency(FlatOpticalElement):
     '''The Multilayer mirror with varying layer thickness along one axis
 
     The distance between layers (and thus best reflected energy) changes along
@@ -90,67 +101,79 @@
     of incidence.
 
     Provide reflectivity data in a file with columns:
 
     - 'X(mm)' - position along the "changing" axis (local y axis)
     - 'Peak lambda' - wavelength with maximum reflection at a given position
     - 'Peak' - maximum reflection at a given position
-    - 'FWHM(nm)' - full width half max, measure of width of reflection Gaussian peaks
+    - 'FWHM(nm)' - full width half max, measure of width of reflection
+      Gaussian peaks
 
     Provide polarization data in a file with columns:
 
     - 'Photon energy' - energy of the photon in keV
-    - 'Polarization' - Fraction polarized in the more reflective direction, so that
-      randomly polarized light would have a value of 0.5.
+    - 'Polarization' - Fraction polarized in the more reflective direction, so
+      that randomly polarized light would have a value of 0.5.
 
     Parameters
     ----------
     reflFile: string
         path, filename, and .txt extension for reflection data file
     testedPolarization: string
-        path, filename, and .txt to a text file containing a table with photon energy
-        and fraction polarization for the light used to test the mirrors and create the
-        reflectivity file
+        path, filename, and .txt to a text file containing a table
+        with photon energy and fraction polarization for the light
+        used to test the mirrors and create the reflectivity file
+
     '''
     def __init__(self, **kwargs):
         self.fileName = kwargs.pop('reflFile')
         self.polFile = kwargs.pop('testedPolarization')
-        super(MultiLayerEfficiency, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def interp_files(self, photons, local):
         # read in correct reflecting probability file, now in table format
         reflectFile = ascii.read(self.fileName)
 
-        # find reflectivity adjustment due to polarization of light in reflectivity testing
+        # find reflectivity adjustment due to polarization of light in
+        # reflectivity testing
         polarizedFile = ascii.read(self.polFile)
         tested_polarized_fraction = np.interp(photons['energy'], polarizedFile['Photon energy'] / 1000, polarizedFile['Polarization'])
 
         # find probability of being reflected due to position
         local_x = local[:, 0] / np.linalg.norm(self.geometry['v_y'])
         local_coords_in_file = reflectFile['X(mm)'] / np.linalg.norm(self.geometry['v_y']) - 1
-        # interpolate 'Peak lambda', 'Peak' [reflectivity], and 'FWHM(nm)' to the actual photon positions
-        peak_wavelength = np.interp(local_x, local_coords_in_file, reflectFile['Peak lambda'])
-        max_refl = np.interp(local_x, local_coords_in_file, reflectFile['Peak']) / tested_polarized_fraction
-        spread_refl = np.interp(local_x, local_coords_in_file, reflectFile['FWHM(nm)'])
+        # interpolate 'Peak lambda', 'Peak' [reflectivity],
+        # and 'FWHM(nm)' to the actual photon positions
+        peak_wavelength = np.interp(local_x, local_coords_in_file,
+                                    reflectFile['Peak lambda'])
+        max_refl = np.interp(local_x, local_coords_in_file,
+                             reflectFile['Peak']) / tested_polarized_fraction
+        spread_refl = np.interp(local_x, local_coords_in_file,
+                                reflectFile['FWHM(nm)'])
 
         return peak_wavelength, max_refl, spread_refl
 
-    def specific_process_photons(self, photons, intersect, intersection, local):
+    def specific_process_photons(self, photons, intersect, intersection,
+                                 local):
          # wavelength is in nm assuming energy is in keV
         wavelength = 1.23984282 / photons['energy'].data[intersect]
         peak_wavelength, max_refl, spread_refl = self.interp_files(photons[intersect], local[intersect])
 
-        # the standard deviation squared of the Gaussian reflectivity functions of each photon's wavelength
+        # the standard deviation squared of the Gaussian reflectivity functions
+        # of each photon's wavelength
         c_squared = (spread_refl ** 2) / (8. * np.log(2))
-        # skip the case when there is no Gaussian (this is assumed to just be the zero function)
+        # skip the case when there is no Gaussian
+        # (this is assumed to just be the zero function)
         c_is_zero = (c_squared == 0)
 
         refl_prob = np.zeros(len(wavelength))
         refl_prob[~c_is_zero] = max_refl[~c_is_zero] * np.exp(-((wavelength[~c_is_zero] - peak_wavelength[~c_is_zero]) ** 2) / (2 * c_squared[~c_is_zero]))
         return {'probability': refl_prob / 100}
 
+
 class MultiLayerMirror(FlatStack):
     def __init__(self, **kwargs):
-        super(MultiLayerMirror, self).__init__(elements=[FlatBrewsterMirror, MultiLayerEfficiency],
-                                               keywords=[{}, {'reflFile': kwargs.pop('reflFile'),
-                                                              'testedPolarization': kwargs.pop('testedPolarization')}],
-                                               **kwargs)
+        super().__init__(elements=[FlatBrewsterMirror,  MultiLayerEfficiency],
+                         keywords=[{},
+                                   {'reflFile': kwargs.pop('reflFile'),
+                                    'testedPolarization': kwargs.pop('testedPolarization')}],
+                         **kwargs)
```

### Comparing `marxs-1.2/marxs/optics/scatter.py` & `marxs-2.0/marxs/optics/scatter.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import astropy.units as u
 
 from ..math.utils import e2h, h2e, norm_vector
 from ..math.rotations import axangle2mat
 from ..math.polarization import parallel_transport
 from .base import FlatOpticalElement
 
+
 class RadialMirrorScatter(FlatOpticalElement):
     '''Add scatter to any sort of radial mirror.
 
     Scatter is added in the plane of reflection, which is defined here
     as the plane which contains (i) the current direction the ray and (ii) the
     vector connecting the center of the `RadialMirrorScatter` element and the
     point of last interaction for the ray.
@@ -33,18 +34,21 @@
     ----------
     inplanescatter : `astropy.Quantity`
         sigma of Gaussian for in-plane scatter
     perpplanescatter : `astropy.Quantity`
         sigma of Gaussian for scatter perpendicular to the plane of reflection
         (default = 0)
     '''
+    inplanescattercol = 'inplanescatter'
+    perpplanescattercol = 'perpplanescatter'
+
     def __init__(self, **kwargs):
         self.inplanescatter = kwargs.pop('inplanescatter').to(u.rad).value
         self.perpplanescatter = kwargs.pop('perpplanescatter', 0. * u.rad).to(u.rad).value
-        super(RadialMirrorScatter, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def specific_process_photons(self, photons, intersect, interpos, intercoos):
         n = intersect.sum()
         center = self.pos4d[:-1, -1]
         radial = h2e(photons['pos'][intersect].data) - center
         perpplane = np.cross(h2e(photons['dir'][intersect].data), radial)
 
@@ -65,15 +69,16 @@
         else:
             perpangle = np.zeros_like(inplaneangle)
 
         pol = parallel_transport(photons['dir'].data[intersect, :], outdir,
                                  photons['polarization'].data[intersect, :])
 
         return {'dir': outdir, 'polarization': pol,
-                'inplanescatter': inplaneangle, 'perpplanescatter': perpangle}
+                self.inplanescattercol: inplaneangle,
+                self.perpplanescattercol: perpangle}
 
 
 class RandomGaussianScatter(FlatOpticalElement):
     '''Add scatter to any sort of radial mirror.
 
     This element scatters rays by a small angle, drawn from a Gaussian
     distribution. The direction of the scatter is random.
@@ -132,11 +137,9 @@
             outdir = np.einsum('...ij,...i->...j', rot, pdir)
             # Now rotate result by up to 2 pi to randomize direction
             angle2 = np.random.uniform(size=n) * 2 * np.pi
             rot = axangle2mat(pdir, angle2)
             outdir = e2h(np.einsum('...ij,...i->...j', rot, outdir), 0)
             pol = parallel_transport(photons['dir'].data[intersect, :], outdir,
                                      photons['polarization'].data[intersect, :])
-            out = {'dir': outdir, 'polarization': pol}
-        if self.scattername is not None:
-            out[self.scattername] = angle
+            out = {'dir': outdir, 'polarization': pol, self.scattername: angle}
         return out
```

### Comparing `marxs-1.2/marxs/optics/tests/test_all_optics.py` & `marxs-2.0/marxs/optics/tests/test_all_optics.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,74 +10,76 @@
 from collections import OrderedDict
 import copy
 
 import numpy as np
 import pytest
 from astropy.coordinates import SkyCoord
 from astropy import units as u
+from astropy.utils.data import get_pkg_data_filename
+
 import transforms3d.axangles
 
 from .. import (RectangleAperture, ThinLens, FlatDetector, CircularDetector,
                 FlatGrating, OrderSelector,
                 MarxMirror, CircleAperture, MultiAperture)
 
 from ..aperture import BaseAperture
 from ...source import PointSource, FixedPointing
 from ..base import FlatStack
 from ...base import _parse_position_keywords
-from ...design import (RowlandTorus, GratingArrayStructure,
-                       LinearCCDArray, RowlandCircleArray,
-                       RectangularGrid)
-from ..baffle import Baffle
+from marxs.design import (RowlandTorus, GratingArrayStructure,
+                       RectangularGrid,
+                       CircularMeshGrid)
+from marxs.optics import Baffle
 from ..multiLayerMirror import MultiLayerMirror
 from ...simulator import Sequence
-from ...missions.chandra.hess import HETG
+from ...missions.chandra import HETG
 from ...missions.mitsnl.catgrating import (QualityFactor, L1,
                                            L2Abs, L2Diffraction,
                                            CATL1L2Stack,
                                            NonParallelCATGrating)
 from ..scatter import RadialMirrorScatter, RandomGaussianScatter
 from ..filter import EnergyFilter
 
-
 # Initialize all optical elements to be tested
 mytorus = RowlandTorus(0.5, 0.5)
 
 all_oe = [ThinLens(focallength=100),
           RectangleAperture(),
           CircleAperture(),
           MultiAperture(elements=[RectangleAperture(),
                                   CircleAperture(position=[0, 200, 0])]),
           FlatDetector(pixsize=2., zoom=100.),
           CircularDetector(),
           FlatGrating(d=0.001, order_selector=OrderSelector([0])),
-          MarxMirror(parfile='marxs/optics/hrma.par'),
-          GratingArrayStructure(mytorus, d_element=0.1, x_range=[0.5, 1.], radius=[0,.5],
+          MarxMirror(parfile=get_pkg_data_filename('hrma.par',
+                                                   package='marxs.optics')),
+          GratingArrayStructure(rowland=mytorus, d_element=[0.1, 0.1],
+                                radius=[0,.5],
                                 elem_class=FlatGrating,
                                 elem_args={'zoom':0.05, 'd':0.002,
                                            'order_selector': OrderSelector([1])
                                            }),
-          LinearCCDArray(mytorus, d_element=0.05, x_range=[0., 0.5],
-                          radius=[0., 0.5], phi=0., elem_class=FlatGrating,
-                         elem_args={'zoom': 0.05, 'd':0.002,
+          CircularMeshGrid(rowland=mytorus, d_element=[0.05, 0.05],
+                          radius=[0., 0.5], elem_class=FlatGrating,
+                          elem_args={'zoom': 0.05, 'd':0.002,
                                     'order_selector': OrderSelector([2])
                                 }),
-          RowlandCircleArray(rowland=mytorus, elem_class=FlatGrating,
-                             elem_args={'zoom': 0.04, 'd': 1e-3,
-                                        'order_selector': OrderSelector([2])},
-                             d_element=0.1,theta=[np.pi - 0.2, np.pi + 0.1]),
           RectangularGrid(rowland=mytorus, elem_class=FlatGrating,
                           elem_args={'zoom': 0.04, 'd': 1e-3,
                                      'order_selector': OrderSelector([-1, 0])},
-                          d_element=0.1, x_range=[0.8, 1.1], y_range=[0, 0.1],
-                          z_range=[0, 0.1]),
+                          d_element=[0.1, 0.1], y_range=[0, 0.1],
+                          z_range=[0, 0.1],
+                          guess_distance=1.),
           Baffle(),
           # MLMirror assumes 45 deg angle and will return nan otherwise
-          MultiLayerMirror(reflFile='./marxs/optics/data/testFile_mirror.txt',
-                           testedPolarization='./marxs/optics/data/ALSpolarization2.txt',
+          MultiLayerMirror(reflFile=get_pkg_data_filename('data/testFile_mirror.txt',
+                                                          package='marxs.optics'),
+                           testedPolarization=get_pkg_data_filename('data/ALSpolarization2.txt',
+                                                                    package='marxs.optics'),
                            orientation=transforms3d.axangles.axangle2mat([0,1,0], np.pi/4)),
           Sequence(elements=[]),
           HETG(),
           RadialMirrorScatter(inplanescatter=0.1 * u.arcsec),
           RandomGaussianScatter(scatter=.1 * u.arcmin),
           # not a useful filterfunc, but OK for testing with a few other dependencies
           EnergyFilter(filterfunc=lambda x: np.abs(np.cos(x))),
```

### Comparing `marxs-1.2/marxs/optics/tests/test_apertures.py` & `marxs-2.0/marxs/optics/tests/test_apertures.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/tests/test_baffle.py` & `marxs-2.0/marxs/optics/tests/test_baffle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 from astropy.table import Table
-from ..baffle import Baffle
+from ..baffles import Baffle
 
 
 def test_photons_through():
     ''' tests that three photons go through or hit the baffle as predicted'''
     pos = np.array([[1., 0., 0., 1],
                     [1., 0., 0., 1],
                     [1., 0., 0., 1]])
```

### Comparing `marxs-1.2/marxs/optics/tests/test_filter.py` & `marxs-2.0/marxs/optics/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/tests/test_grating.py` & `marxs-2.0/marxs/optics/tests/test_grating.py`

 * *Files 3% similar despite different names*

```diff
@@ -62,20 +62,20 @@
         assert np.allclose(p['dir'][0, :], p['dir'][1, :])
         assert np.allclose(p['pos'][0, :], p['pos'][1, :] - delta_pos)
 
 def test_angle_dependence():
     '''Test the grating angle for non-perpendicular incidence.
 
     For this test, I write the grating equation in its simple traditional form:
-    :math:`m \lambda = \delta s = d sin(\alpha)`.
+    m lambda = delta s = d sin(alpha).
 
     If the incoming ray is not perpendicular to the grating, we use the angle beta
-    between the incoming ray and the grating normal. The grating equation than looks
+    between the incoming ray and the grating normal. The grating equation then looks
     like this for m = 1:
-    :math:`\delta s = \delta s_2 - \delta s_1 = d sin(\alpha) - d sin(\beta)`.
+    delta s = delta s_2 - delta s_1 = d sin(alpha) - d sin(beta).
     '''
     d = 0.001
     beta = np.deg2rad([0., 5., 10., 20.])
     dir = np.zeros((len(beta), 4))
     dir[:, 1] = np.sin(beta)
     dir[:, 0] = -np.cos(beta)
     pos = np.ones((len(beta), 4))
```

### Comparing `marxs-1.2/marxs/optics/tests/test_marx.py` & `marxs-2.0/marxs/optics/tests/test_marx.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 way. In particular, it holds regression tests for issues that were already discovered
 and fixed.
 '''
 import numpy as np
 from scipy.stats import ks_2samp
 from astropy.coordinates import SkyCoord
 import astropy.units as u
+from astropy.utils.data import get_pkg_data_filename
 
 import marxs
 import marxs.source
 import marxs.optics.marx
 
 def test_noexplicettimedependence():
     '''In an older implementation, the first half of all photons went of
@@ -22,11 +23,13 @@
     while marx expects an *unsigned* int.
     '''
     mysource = marxs.source.PointSource(coords=SkyCoord(30., 30., unit="deg"))
     photons = mysource.generate_photons(1 * u.ks)
     mypointing = marxs.source.FixedPointing(coords=SkyCoord(30, 30., unit='deg'))
     photons = mypointing(photons)
 
-    marxm = marxs.optics.marx.MarxMirror('./marxs/optics/hrma.par', position=np.array([0., 0,0]))
+    marxm = marxs.optics.marx.MarxMirror(parfile=get_pkg_data_filename('hrma.par',
+                                                   package='marxs.optics'),
+                                         position=np.array([0., 0,0]))
     photons = marxm(photons)
     ks, p_value = ks_2samp(photons['mirror_shell'][:400], photons['mirror_shell'][600:])
     assert p_value > 1e-5
```

### Comparing `marxs-1.2/marxs/optics/tests/test_mirror.py` & `marxs-2.0/marxs/optics/tests/test_mirror.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 import pytest
 from astropy.coordinates import SkyCoord
 import astropy.units as u
+from scipy.interpolate import RectBivariateSpline
+
 from ... import source, optics
 from ...math.utils import h2e
+from marxs.utils import generate_test_photons
 
 
 @pytest.mark.parametrize("ra", [0., 30., -60.])
 def test_PerfectLens(ra):
     mysource = source.PointSource(coords=SkyCoord(0., ra, unit="deg"))
     mypointing = source.FixedPointing(coords=SkyCoord(0., 0., unit='deg'))
     myslit = optics.RectangleAperture(zoom=2, position=[+100, 0, 0])
@@ -31,7 +34,47 @@
     assert np.std(photons['det_y']) < 1e-4
 
     # Check that they actually diverge for other detector placement
     mdet = optics.FlatDetector(pixsize=0.01, position=np.array([-2 * d, 0, 0]), zoom=1e5)
     photons = mdet(photons)
     assert np.std(photons['det_x']) > 1e-4
     assert np.std(photons['det_y']) > 1e-4
+
+
+def test_PerfectLens_offset():
+    """Test a lens that is not centered on the optical axis."""
+    lens = optics.PerfectLens(focallength=100, position=[0, 0, 10], zoom=400)
+    lens2 = optics.PerfectLens(
+        focallength=100, position=[0, 0, 0], zoom=400, d_center_optical_axis=-10
+    )
+    lens3 = optics.PerfectLens(
+        focallength=100, position=[0, 0, 0], zoom=400, d_center_optical_axis=0
+    )
+    photons = generate_test_photons(1)
+    p2 = generate_test_photons(1)
+    p3 = generate_test_photons(1)
+    photons = lens(photons)
+    p2 = lens2(p2)
+    p3 = lens3(p3)
+    np.testing.assert_allclose(photons["dir"], p2["dir"])
+    not np.allclose(photons["dir"], p3["dir"])
+
+
+def test_PerfectLens_refl():
+    """Test a reflection.
+
+    This test sis a bit silly in the sense that it
+    uses an unnecessarily complicated reflectivity function
+    but then reflect at 0 deg."""
+    xarr = np.linspace(-3, 3, 100)
+    yarr = np.linspace(-3, 3, 100)
+    xgrid, ygrid = np.meshgrid(xarr, yarr, indexing="ij")
+    zdata = np.exp(-np.sqrt((xgrid / 2) ** 2 + ygrid**2))
+    interp = RectBivariateSpline(xarr, yarr, zdata, kx=1, ky=1)
+
+    lens = optics.PerfectLens(focallength=123.0, reflectivity_interpolator=interp)
+    photons = generate_test_photons(1)
+    photons = lens(photons)
+
+    assert np.allclose(photons["energy"], 1)
+    assert np.allclose(photons["polarization"], [0, 1, 0, 0])
+    assert np.allclose(photons["probability"], 0.367205)
```

### Comparing `marxs-1.2/marxs/optics/tests/test_mlMirror.py` & `marxs-2.0/marxs/optics/tests/test_mlMirror.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,56 +1,68 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 from astropy.table import Table
 from astropy.io import ascii
+from astropy.utils.data import get_pkg_data_filename
+
 from transforms3d import euler
 from ...math.utils import norm_vector
 from ..multiLayerMirror import MultiLayerMirror, FlatBrewsterMirror
 
 import pytest
 
+
 def test_photon_reflection():
-    ''' tests that three photons are accurately reflected
+    '''tests that three photons are accurately reflected
+
+    TODO: This test should be broken down into smaller components, as
+    should the multilayer mirror process photons function.
 
-    TODO: This test should be broken down into smaller components, as should the
-    multilayer mirror process photons function.
     '''
-    pos = np.tile([1.,0.,0.,1.], (4,1))
-    # hitting y = 23mm, 26mm, 24mm; std dev = 0.02, 0.04, 0.01; max = 5.81, 0.42, 6.21; lambda = 3, 6, 4
+    pos = np.tile([1., 0., 0., 1.], (4, 1))
+    # hitting y = 23mm, 26mm, 24mm;
+    # std dev = 0.02, 0.04, 0.01;
+    # max = 5.81, 0.42, 6.21;
+    # lambda = 3, 6, 4
     dir = np.array([[-1., -1.5, 0., 0],
                     [-1., 1.5, 0., 0],
                     [-1., -0.5, 13., 0],
                     [-1., -1.5, 0., 0]])
-    # note: these photons will not hit at 45 degrees (only ok for testing purposes)
+    # note: these photons will not hit at 45 degrees
+    # (only ok for testing purposes)
     polarization = np.array([[0., 0., 1., 0],
                              [1., 0., 0., 0],
                              [1., 0., 0., 0],
                              [1. / np.sqrt(2.), 0., 1. / np.sqrt(2.), 0.]])
-    # z axis is the parallel polarization, v_1, so crossing that with direction (perpendicular to z) is v_2
-    polarization[1, 0:3] = np.cross(dir[1,0:3], polarization[0,0:3])
-    polarization[1, 0:3] /= np.linalg.norm(polarization[1,0:3])
+    # z axis is the parallel polarization, v_1,
+    # so crossing that with direction (perpendicular to z) is v_2
+    polarization[1, 0:3] = np.cross(dir[1, 0:3], polarization[0, 0:3])
+    polarization[1, 0:3] /= np.linalg.norm(polarization[1, 0:3])
 
     photons = Table({'pos': pos,
                      'dir': dir,
                      'energy': [1.23984282 / 3.02, 1.23984282 / 6, 0.4,
                                 1.23984282 / 3.02],
                      'polarization': polarization,
                      'probability': [1., 1., 1., 1.]})
-    mirror = MultiLayerMirror(reflFile='./marxs/optics/data/testFile_mirror.txt', testedPolarization='./marxs/optics/data/ALSpolarization2.txt', zoom=[1, 24.5, 12])
+    mirror = MultiLayerMirror(reflFile=get_pkg_data_filename('data/testFile_mirror.txt', package='marxs.optics'),
+                              testedPolarization=get_pkg_data_filename('data/ALSpolarization2.txt',
+                                                                       package='marxs.optics'),
+                              zoom=[1, 24.5, 12])
     photons = mirror(photons)
 
     # confirm reflection angle
     expected_dir = norm_vector(np.array([[1., -1.5, 0., 0],
                                          [1., 1.5, 0., 0],
                                          [-1., -0.5, 13., 0],
                                          [1., -1.5, 0., 0]]))
     assert np.allclose(norm_vector(np.array(photons['dir'])), expected_dir)
 
     # confirm reflection probability
-    polarizedFile = ascii.read('./marxs/optics/data/ALSpolarization2.txt')
+    polarizedFile = ascii.read(get_pkg_data_filename('data/ALSpolarization2.txt', package='marxs.optics'))
     correctTestPolar = np.interp(1.23984282 / 3.02,
                                  polarizedFile['Photon energy'] / 1000,
                                  polarizedFile['Polarization'])
     expected_prob = np.array([0.0581 * np.exp(-0.5) * 1. / correctTestPolar,
                               0.0042 * 0.,
                               1.,
                               0.5 * 0.0581 * np.exp(-0.5) * 1. / correctTestPolar])
@@ -69,39 +81,47 @@
 def test_photon_reflection2():
     '''more rigorous reflection test'''
     pos = np.array([[0., 0., 1., 1],
                     [0., -0.6, 1., 1],
                     [0., 0., 1., 1],
                     [0., 0.5, 1., 1]])
     # hitting y = 24.5mm, 24mm, 24.5mm, 25mm;
-    # ---XXX--- std dev = 0.02, 0.04, 0.01; max = 5.81, 0.42, 6.21; lambda = 3, 6, 4
+    # ---XXX--- std dev = 0.02, 0.04, 0.01; max = 5.81,
+    # 0.42, 6.21; lambda = 3, 6, 4
     dir = np.array([[0., 0., -1., 0],
                     [0., 0.1, -1., 0],
                     [0., 0., -1., 0],
                     [0., 0., -1., 0]])
-    # note: these photons will not hit at 45 degrees (only ok for testing purposes)
+    # note: these photons will not hit at 45 degrees
+    #(only ok for testing purposes)
     polarization = np.array([[0., 1., 0., 0],
                              [0., 1., 0.1, 0],
                              [1., 0., 0., 0],
                              [1., 0., 0., 0]])
-    # z axis is the parallel polarization, v_1, so crossing that with direction (perpendicular to z) is v_2
+    # z axis is the parallel polarization, v_1,
+    # so crossing that with direction (perpendicular to z) is v_2
 
     photons = Table({'pos': pos, 'dir': dir,
                      'energy': [1.23984282 / 3.02, 1.23984282 / 6, 0.4, 0.5],
                      'polarization': polarization,
                      'probability': [1., 1., 1., 1.]})
     a = 2**(-0.5)
-    mirror = MultiLayerMirror(reflFile='./marxs/optics/data/testFile_mirror.txt',
-                              testedPolarization='./marxs/optics/data/ALSpolarization2.txt',
-                              orientation=np.array([[-a, 0, a],[0, -1, 0],[a, 0, a]]))
+    mirror = MultiLayerMirror(
+        reflFile=get_pkg_data_filename('data/testFile_mirror.txt',
+                                       package='marxs.optics'),
+        testedPolarization=get_pkg_data_filename('data/ALSpolarization2.txt',
+                                                 package='marxs.optics'),
+        orientation=np.array([[-a, 0, a], [0, -1, 0], [a, 0, a]]))
     photons = mirror(photons)
 
-
     # confirm reflection angle
-    expected_dir = norm_vector(np.array([[-1., 0., 0., 0], [-1., 0.1, 0., 0], [-1., 0., 0., 0], [-1., 0., 0., 0]]))
+    expected_dir = norm_vector(np.array([[-1., 0., 0., 0],
+                                         [-1., 0.1, 0., 0],
+                                         [-1., 0., 0., 0],
+                                         [-1., 0., 0., 0]]))
     assert np.allclose(norm_vector(np.array(photons['dir'])), expected_dir)
 
     # This test could be expanded but the numbers in the 'expected' arrays have not been correctly calculated yet.
     #
     # # confirm reflection probability
     # polarizedFile = ascii.read('./marxs/optics/data/ALSpolarization2.txt')
     # correctTestPolar = np.interp(1.23984282 / 3.02, polarizedFile['Photon energy'] / 1000, polarizedFile['Polarization'])
@@ -110,31 +130,37 @@
     #
     # # confirm correct new polarization
     # expected_pol = np.array([[0., 1., 0., 0], [1., 1.5, 0., 0], [0., 0., 1., 0], [0., 0., 1., 0]])
     # #expected_pol[1,0:3] = np.cross(photons['dir'][1,0:3] / np.linalg.norm(photons['dir'][1,0:3]), expected_pol[0,0:3])
     # for i in range(0, 2):
     #   assert np.allclose(np.array(photons['polarization'][i]), expected_pol[i]) or np.allclose(np.array(photons['polarization'][i]), -expected_pol[i])
 
+
 @pytest.mark.parametrize("angle,avgpol", [(0., 0.5), (np.pi/2, 0.)])
 def test_double_reflection(angle, avgpol):
     '''Two mirrors
 
     The first mirror polarizes the light and the second
     one perfectly reflects that polarized light or perfectly absorbs it.
     '''
     pos = np.tile([1., 0., 0., 1.], (8, 1))
     dir = np.tile([-1., 0., 0., 0.], (8, 1))
 
     ang = np.arange(0, 2. * np.pi, np.pi / 4)
-    polarization = np.vstack([np.zeros(8), np.sin(ang), np.cos(ang), np.zeros(8)]).T
+    polarization = np.vstack([np.zeros(8),
+                              np.sin(ang),
+                              np.cos(ang),
+                              np.zeros(8)]).T
 
     photons = Table({'pos': pos,
                      'dir': dir,
                      'energy': np.ones(8),
                      'polarization': polarization,
                      'probability': np.ones(8)})
-    ml1 = FlatBrewsterMirror(orientation=euler.euler2mat(np.pi / 4, 0, 0, 'szxy'))
+    ml1 = FlatBrewsterMirror(orientation=euler.euler2mat(np.pi / 4, 0, 0,
+                                                         'szxy'))
     ml2 = FlatBrewsterMirror(position=[0, 1, 0],
-                             orientation=euler.euler2mat(-np.pi / 4, angle, 0, 'szyx'))
+                             orientation=euler.euler2mat(-np.pi / 4, angle,
+                                                         0, 'szyx'))
     photons = ml1(photons)
     photons = ml2(photons)
     assert np.isclose(np.mean(photons['probability']), avgpol)
```

### Comparing `marxs-1.2/marxs/optics/tests/test_optics.py` & `marxs-2.0/marxs/optics/tests/test_optics.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/optics/tests/test_scatter.py` & `marxs-2.0/marxs/optics/tests/test_scatter.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/simulator/simulator.py` & `marxs-2.0/marxs/simulator/simulator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 from transforms3d.affines import decompose44
 
 from ..math.utils import translation2aff, zoom2aff, mat2aff, e2h, h2e
 from ..math.geometry import Geometry
+from ..math.rotations import ex2vec_fix
 from ..base import SimulationSequenceElement, _parse_position_keywords
 import transforms3d
 from transforms3d.utils import normalized_vector
 
 __all__ = ['SimulationSetupError',
            'BaseContainer',
            'Sequence',
@@ -32,15 +33,15 @@
 
     def __init__(self, **kwargs):
         self.preprocess_steps = kwargs.pop('preprocess_steps', [])
         self.postprocess_steps = kwargs.pop('postprocess_steps', [])
         for elem in self.elements + self.preprocess_steps + self.postprocess_steps:
             if not callable(elem):
                 raise SimulationSetupError('{0} is not callable.'.format(str(elem)))
-        super(BaseContainer, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __call__(self, photons):
         for elem in self.elements:
             for p in self.preprocess_steps:
                 p(photons)
             photons = elem(photons)
             for p in self.postprocess_steps:
@@ -95,14 +96,56 @@
         for e in self.elements:
             if compfunc(e, cls):
                 a += [e]
             elif hasattr(e, 'elements_of_class'):
                 a += e.elements_of_class(cls, subclass_ok)
         return a
 
+
+    def first_of_class_top_level(self, cls, subclass_ok=False):
+        '''Return the index of the first sub-element that has ``cls`` in it.
+
+        This walks the hiracy of `marxs.simulator.Sequence` and
+        `marxs.simulator.Parallel` objects and returns the index of the
+        first sub-element that contains a certain class.
+
+        Typically, this function is used to study and instrument with small
+        modifications. If e.g. only the detector are changed, we might want to
+        run a simulation up to the detectors, save te rays and then try out
+        different detector combinations without rerunning the simulations for
+        all earlier steps. This methid can help to identify the step that
+        contains the detectors.
+
+        Parameters
+        ----------
+        cls : class
+            The class searched for, e.g. `marxs.optics.FlatDetector` to find all
+            detectors.
+        subclass_ok : bool
+            Controls if subclasses of `cls` count as match.
+
+        Returns
+        -------
+        out : int or None
+            index for the first element in ``self.elements`` that is or contains
+            an objects of class ``cls``. If none is found, the method return
+            ``None``.
+        '''
+        for i, e in enumerate(self.elements):
+            if subclass_ok:
+                compfunc = lambda a, b: isinstance(a, b)
+            else:
+                compfunc = lambda a, b: type(a) == b
+            if compfunc(e, cls):
+                return i
+            elif hasattr(e, 'elements_of_class') and len(e.elements_of_class(cls, subclass_ok)) > 0:
+                return i
+        return None
+
+
 class Sequence(BaseContainer):
     '''A `Sequence` is a container that summarizes several optical elements.
 
     Parameters
     ----------
     elements : list
         The elements of this list are all optical elements that process photons.
@@ -153,15 +196,15 @@
 
     As expected, they fall right around the center of the detector (row 19 and 20 of a
     40 * 40 pixel detector).
     '''
 
     def __init__(self, **kwargs):
         self.elements = kwargs.pop('elements')
-        super(Sequence, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class Parallel(BaseContainer):
     '''A container for several identical optical elements.
 
     This object describes a set of similar elements that operate in
     parallel, meaning that each photon will only interact with one of
@@ -304,15 +347,15 @@
                 elem_pos_dict = {}
                 for k in keys:
                     elem_pos_dict[k] = elem_pos[k][i]
                 self.elem_pos.append(_parse_position_keywords(elem_pos_dict))
         else:
             self.elem_pos = elem_pos
 
-        super(Parallel, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
         if 'id_col' not in self.elem_args:
             self.elem_args['id_col'] = self.id_col
         self.elem_uncertainty = [np.eye(4)] * len(self.elem_pos)
         self.generate_elements()
 
     def move_center(self, change4d):
@@ -442,15 +485,15 @@
     '''
 
     def __init__(self, **kwargs):
         self.pos_spec = kwargs.pop('pos_spec')
         self.normal_spec = kwargs.pop('normal_spec')
         self.parallel_spec = kwargs.pop('parallel_spec')
         kwargs['elem_pos'] = self.calculate_elempos()
-        super(ParallelCalculated, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def calculate_elempos(self):
         '''Calculate the position of elements based on some algorithm.
 
         Classes derived from `ParallelCalculated` can overwrite this
         method if they want to provide a way to calculate the pos4d
         matrices for the elements that make up this
@@ -466,24 +509,17 @@
 
         '''
         pos4d = []
 
         xyzw = self.get_elemxyzw()
         normals = self.get_spec('normal_spec', xyzw)
         parallels = self.get_spec('parallel_spec', xyzw, normals)
-        normals = h2e(normals)
-        parallels = h2e(parallels)
 
         for i in range(xyzw.shape[0]):
-            n = normalized_vector(normals[i, :])
-            p = parallels[i, :]
-            rot_mat = np.zeros((3,3))
-            rot_mat[:, 0] = n
-            rot_mat[:, 1] = normalized_vector(p - n * np.dot(n, p))
-            rot_mat[:, 2] = normalized_vector(np.cross(n, rot_mat[:, 1]))
+            rot_mat = ex2vec_fix(h2e(normals[i, :]), h2e(parallels[i, :]))
             pos4d.append(transforms3d.affines.compose(h2e(xyzw[i, :]), rot_mat, np.ones(3)))
         return pos4d
 
     def get_elemxyzw(self):
         if callable(self.pos_spec):
             return self.pos_spec()
         else:
@@ -545,26 +581,26 @@
         will only work for columns that store data in homogeneous coordinates,
         for all other cases, simply call `numpy.asanyarray` on your `KeepCol`
         object.
 
         Parameters
         ----------
         atol : float or None
-            Sometimes several consequtive elements record identical photon positions in
+            Sometimes several consecutive elements record identical photon positions in
             `keepcol`. Those are removed from the output to speed up rendering in 3D
             programs.
             ``atol`` sets the limit up to which two positions are considered *identical*.
             See `np.allclose` for a detailed description of ``atol``.
             Set to ``None`` to skip this step.
 
         Returns
         -------
         pos : np.array
             Array of shape (N, n, 3), where N is the number of photons and n the number of
-            unique photon positions in eukledian coordinates.
+            unique photon positions in euclidean coordinates.
         '''
         if len(self.data) == 0:
             raise ValueError('KeepCol object contains no data.')
         if not self.data[0].ndim == 2 or self.data[0].shape[1] !=4:
             raise ValueError('format_position only works for columns that store homogeneous coordinates.')
         d = np.dstack(self.data)
         d = np.swapaxes(d, 1, 2)
@@ -594,15 +630,15 @@
         Parameters
         ----------
         distance : float
             Distance for the photons to move. Negative values move photons
             backwards.
         '''
         self.distance = kwargs.pop('distance')
-        super(Propagator, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __call__(self, photons):
         photons['pos'] = photons['pos'] + self.distance * photons['dir']
         return photons
 
 
 def propagate(photons, d):
```

### Comparing `marxs-1.2/marxs/simulator/tests/test_parallel.py` & `marxs-2.0/marxs/simulator/tests/test_parallel.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import numpy as np
 from transforms3d.affines import decompose
 from transforms3d.euler import euler2mat
 
 from ...utils import generate_test_photons
 from .. import Parallel, ParallelCalculated
 from ...optics import FlatDetector as CCD
-from ...design import RowlandTorus, RowlandCircleArray
+from ...design import RowlandTorus, RectangularGrid
 
 def test_Parallel_numbering():
     '''Test automatic numbering and numbers assigned to photons.
     '''
     pos = [[0, -10.1, -10.1],[0, .1, -10.1],[0, -10.1, .1],[0, .1, .1]]
     detect = Parallel(elem_class=CCD, elem_args={'pixsize': 0.01, 'zoom': 5},
                       elem_pos={'position': pos}, id_col='CCD_ID')
@@ -69,17 +69,19 @@
 
 def test_parallel_calculated_normals():
     '''Regression test: At one point the rotation matrix was reversed,
     mixing active and passive rotations. As a result, the detector elements
     did not match up on the Rowland circle.'''
     rowland = RowlandTorus(5900., 6020.)
     detccdargs = {'pixsize': 0.024,'zoom': [1, 24.576, 12.288]}
-    det = RowlandCircleArray(rowland=rowland, elem_class=CCD,
+    det = RectangularGrid(rowland=rowland, elem_class=CCD,
                              elem_args=detccdargs,
-                             d_element=49.652, theta=[np.pi - 0.2, np.pi -0.19])
+                             d_element=[49.652, 49.652],
+                             y_range=[-100, 100],
+                             guess_distance=25.)
     e1 = det.elements[0]
     e2 = det.elements[1]
     # These two edges should be close together:
     edge1 = e1.geometry['center'] + e1.geometry['v_y']
     edge2 = e2.geometry['center'] - e2.geometry['v_y']
     assert np.all(np.abs(edge1 - edge2) < 3.)
```

### Comparing `marxs-1.2/marxs/simulator/tests/test_simulator.py` & `marxs-2.0/marxs/simulator/tests/test_simulator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from astropy.table import Table
 import pytest
 
 from ..simulator import KeepCol, Sequence, BaseContainer
-from ...optics import FlatDetector
+from ...optics import FlatDetector, FlatOpticalElement
 
 f1 = FlatDetector()
 f2 = FlatDetector()
 f3 = FlatDetector()
 s_l2 = Sequence(elements=[f2, f3])
 
 mission = Sequence(elements=[f1, s_l2])
@@ -31,14 +31,22 @@
     assert [f1, f2, f3] == mission.elements_of_class(FlatDetector,
                                                      stop_at_first=True)
     assert [f1, f2, f3] == mission.elements_of_class(FlatDetector,
                                                      subclass_ok=True,
                                                      stop_at_first=True)
 
 
+def test_first_of_class():
+    '''Check that the first of class method returns expected indices.'''
+    assert mission.first_of_class_top_level(FlatDetector) == 0
+    assert mission.first_of_class_top_level(FlatOpticalElement) is None
+    assert mission.first_of_class_top_level(FlatOpticalElement, subclass_ok=True) == 0
+    assert mission.first_of_class_top_level(Sequence) == 1
+
+
 def test_format_saved_positions():
     '''Reformat saved positions and drop nearly identical values.'''
     pos0 = np.arange(20).reshape(5,4)
     pos1 = pos0 + 1
     pos2 = pos1 + 1e-4
     pos = KeepCol('testcase')
     pos.data = [pos0, pos1, pos2]
```

### Comparing `marxs-1.2/marxs/source/labSource.py` & `marxs-2.0/marxs/source/labSource.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 from astropy.table import Column
 import astropy.units as u
 import transforms3d
 
 from ..optics.base import FlatOpticalElement
-from .source import Source
+from .basesources import Source
 from ..math.polarization import polarization_vectors
 from ..math.utils import h2e, e2h
 
 
 class FarLabPointSource(Source, FlatOpticalElement):
     '''Simple in-lab point source used with aperture
 
@@ -18,28 +18,31 @@
     - photon direction determined by location of source, and selected photon starting position
     - aperture is in its local y-z plane
 
     Parameters
     ----------
     sourcePos: 3 element list
         3D coordinates of photon source (not aperture)
-    kwargs: ``pos4d`` or ``position``, ``orientation``, and ``zoom`` can be used to set the position,
-        size and orientation of the rectangular apeture; see `pos4d` for details.
-        Other keyword arguments include ``flux``, ``energy`` and ``polarization``.
+    kwargs:
+        ``pos4d`` or ``position``, ``orientation``, and ``zoom`` can
+        be used to set the position, size and orientation of the
+        rectangular apeture; see `pos4d` for details.  Other keyword
+        arguments include ``flux``, ``energy`` and ``polarization``.
         See `Source` for details.
+
     '''
     def __init__(self, sourcePos, **kwargs):
         self.sourcePos = sourcePos
-        if not 'flux' in kwargs:
+        if 'flux' not in kwargs:
             kwargs['flux'] = 1 / u.s
-        super(FarLabPointSource, self).__init__(geomarea=None, **kwargs)
+        super().__init__(geomarea=None, **kwargs)
 
     @u.quantity_input
     def generate_photons(self, exposuretime: u.s):
-        photons = super(FarLabPointSource, self).generate_photons(exposuretime)
+        photons = super().generate_photons(exposuretime)
         n = len(photons)
         # randomly choose direction - photons uniformly distributed over aperture area
         # measurements in mm
         pos = np.dot(self.pos4d, np.array([np.zeros(n),
                                            np.random.uniform(-1, 1, n),
                                            np.random.uniform(-1, 1, n),
                                            np.ones(n)]))
@@ -80,17 +83,17 @@
                  direction=[1., 0., 0.],
                  **kwargs):
         if (len(position) != 3) or (len(direction) != 3):
             raise ValueError('Direction and position are expected in Eukledian coordinates.')
         self.dir = e2h(np.asanyarray(direction) / np.linalg.norm(direction), 0)
         self.position = e2h(np.asanyarray(position), 1)
         self.half_opening = half_opening
-        if not 'flux' in kwargs:
+        if 'flux' not in kwargs:
             kwargs['flux'] = 1 / u.s
-        super(LabPointSourceCone, self).__init__(geomarea=None, **kwargs)
+        super().__init__(geomarea=None, **kwargs)
 
     @u.quantity_input
     def generate_photons(self, exposuretime: u.s):
         photons = super(LabPointSourceCone, self).generate_photons(exposuretime)
         n = len(photons)
 
         # assign position to photons
```

### Comparing `marxs-1.2/marxs/source/pointing.py` & `marxs-2.0/marxs/source/pointing.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
         self.coords = kwargs.pop('coords')
         if not self.coords.isscalar:
             raise ValueError("Coordinate must be scalar, not array.")
         self.roll = kwargs.pop('roll', 0. * u.rad)
 
         self.reference_transform = kwargs.pop('reference_transform', np.eye(4))
 
-        super(FixedPointing, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @property
     def offset_coos(self):
         '''Return `~astropy.coordinates.SkyOffsetFrame`'''
         return self.coords.skyoffset_frame(rotation=self.roll)
 
     def photons_dir(self, coos, time):
@@ -146,54 +146,59 @@
 
     def process_photons(self, photons):
         '''
         Parameters
         ----------
         photons : `astropy.table.Table`
         '''
-        photons = super(FixedPointing, self).process_photons(photons)
-        photons['dir'] = self.photons_dir(SkyCoord(photons['ra'], photons['dec'],
+        photons = super().process_photons(photons)
+        photons['dir'] = self.photons_dir(SkyCoord(photons['ra'],
+                                                   photons['dec'],
                                                    unit='deg'),
                                           photons['time'].data)
         photons['polarization'] = self.photons_pol(photons['dir'].data,
                                                    photons['polangle'].data,
                                                    photons['time'].data)
         photons.meta['RA_PNT'] = (self.coords.ra.degree, '[deg] Pointing RA')
-        photons.meta['DEC_PNT'] = (self.coords.dec.degree, '[deg] Pointing Dec')
+        photons.meta['DEC_PNT'] = (self.coords.dec.degree,
+                                   '[deg] Pointing Dec')
         photons.meta['ROLL_PNT'] = (self.roll.to(u.degree).value,
                                     '[deg] Pointing Roll')
-        photons.meta['RA_NOM'] = (self.coords.ra.degree, '[deg] Nominal Pointing RA')
-        photons.meta['DEC_NOM'] = (self.coords.dec.degree, '[deg] Nominal Pointing Dec')
+        photons.meta['RA_NOM'] = (self.coords.ra.degree,
+                                  '[deg] Nominal Pointing RA')
+        photons.meta['DEC_NOM'] = (self.coords.dec.degree,
+                                   '[deg] Nominal Pointing Dec')
         photons.meta['ROLL_NOM'] = (self.roll.to(u.degree).value,
                                     '[deg] Nominal Pointing Roll')
 
         return photons
 
 
 class JitterPointing(FixedPointing):
     '''Transform spacecraft to fixed sky system.
 
-    This extends `marxs.sourcs.FixedPointing` by adding a random jitter coordinate.
-    In this simple implementation the jitter angles applied to two consecutive
-    photons are entirely uncorrelated, even if these two photons arrive at the
-    same time.
-    This class makes the assumption that jitter is small (no change in the projected
-    geometric area of the aperture due to jitter).
+    This extends `marxs.sourcs.FixedPointing` by adding a random
+    jitter coordinate.  In this simple implementation the jitter
+    angles applied to two consecutive photons are entirely
+    uncorrelated, even if these two photons arrive at the same time.
+    This class makes the assumption that jitter is small (no change in
+    the projected geometric area of the aperture due to jitter).
 
     Parameters
     ----------
     jitter : `~astropy.units.quantity.Quantity`
         Gaussian sigma of jitter angle
+
     '''
     def __init__(self, **kwargs):
         self.jitter = np.abs(kwargs.pop('jitter'))
-        super(JitterPointing, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def process_photons(self, photons):
-        photons = super(JitterPointing, self).process_photons(photons)
+        photons = super().process_photons(photons)
         # Get random jitter direction
         n = len(photons)
         randang = np.random.rand(n) * 2. * np.pi
         ax = np.vstack([np.zeros(n), np.sin(randang), np.cos(randang)]).T
         if self.jitter > 0:
             # For comparison it's often useful to run a model with jitter=0
             # but that would fail np.random.normal(scale=0)
```

### Comparing `marxs-1.2/marxs/source/source.py` & `marxs-2.0/marxs/source/basesources.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,25 @@
 # Licensed under GPL version 3 - see LICENSE.rst
-'''
-Sources generate photons with all photon properties: energy, direction, time, polarization.
+'''Sources generate photons with all photon properties: energy, direction, time, polarization.
 
-For objects of type `AstroSource`, the coordinates of the photon origin on the sky are added to the photon list. `astropy.coords.SkyCoord` is an object well suited for this task. These objects can be added to photon tables through the mechanims of `mixin columns <http://docs.astropy.org/en/latest/table/index.html#mixin-columns>`). However, mix-in columns don't (yet) support saving to all table formats or tables operations such as stacking. Thus, it is much better to include the coordinates as two columns of floats with names ``ra`` and ``dec`` into the table.
+For objects of type `AstroSource`, the coordinates of the photon
+origin on the sky are added to the photon
+list. `astropy.coords.SkyCoord` is an object well suited for this
+task. These objects can be added to photon tables through the
+mechanims of `mixin columns
+<http://docs.astropy.org/en/latest/table/index.html#mixin-columns>`). However,
+mix-in columns don't (yet) support saving to all table formats or
+tables operations such as stacking. Thus, it is much better to include
+the coordinates as two columns of floats with names ``ra`` and ``dec``
+into the table.
+
+Sources take a `~astropy.coordinates.SkyCoord` from the user to avoid
+any ambiguity about the coordinate systme used, but convert this into
+plain floats used in the photon table.
 
-Sources take a `~astropy.coordinates.SkyCoord` from the user to avoid any ambiguity about the coordinate systme used, but convert this into plain floats used in the photon table.
 '''
 
 import os
 from datetime import datetime
 
 import numpy as np
 from scipy.stats import expon
@@ -145,15 +156,15 @@
     def __init__(self, energy=1*u.keV, flux=1 / u.s / u.cm**2,
                  polarization=None, geomarea=1*u.cm**2, **kwargs):
         self.energy = energy
         self.flux = flux
         self.polarization = polarization
         self.geomarea = 1 if geomarea is None else geomarea
 
-        super(Source, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def __call__(self, *args, **kwargs):
         return self.generate_photons(*args, **kwargs)
 
     @u.quantity_input()
     def generate_times(self, exposuretime: u.s):
         if callable(self.flux):
@@ -244,15 +255,15 @@
         n = len(times)
         photons = Table([times.to(u.s).value,
                          energies.to(u.keV).value,
                          pol.to(u.rad).value,
                          np.ones(n)],
                         names=['time', 'energy', 'polangle', 'probability'])
         photons.meta['EXTNAME'] = 'EVENTS'
-        photons.meta['EXPOSURE'] = (exposuretime.to(u.s),
+        photons.meta['EXPOSURE'] = (exposuretime.to(u.s).value,
                                     'total exposure time [s]')
 
         #photons.meta['DATE-OBS'] =
         photons.meta['CREATOR'] = 'MARXS - Version {0}'.format(marxsversion)
         photons.meta["LONGSTRN"] = ("OGIP 1.0", "The OGIP long string convention may be used.")
         photons.meta['MARXSVER'] = (marxsversion, 'MARXS version')
         now = datetime.now()
@@ -284,15 +295,15 @@
         if isinstance(coords, SkyCoord):
             self.coords = coords
         else:
             self.coords = SkyCoord(coords)
 
         if not self.coords.isscalar:
             raise ValueError("Coordinate must be scalar, not array.")
-        super(AstroSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def set_pos(self, photons, coo):
         '''Set Ra, Dec of photons in table
 
         This function write Ra, Dec to a table. It is defined here to
         make the way `astropy.coordinates.SkyCoord` objects are stored
         more uniform.  Currently, mixin columns in tables have some
@@ -320,146 +331,158 @@
 
 class PointSource(AstroSource):
     '''Astrophysical point source.
 
     Parameters
     ----------
     kwargs : see `Source`
-        Other keyword arguments include ``flux``, ``energy`` and ``polarization``.
-        See `Source` for details.
+        Other keyword arguments include ``flux``, ``energy`` and
+        ``polarization``. See `Source` for details.
     '''
     def __init__(self, **kwargs):
-        super(PointSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @u.quantity_input
     def generate_photons(self, exposuretime: u.s):
-        photons = super(PointSource, self).generate_photons(exposuretime)
+        photons = super().generate_photons(exposuretime)
         self.set_pos(photons, self.coords)
         return photons
 
 
 class RadialDistributionSource(AstroSource):
-    ''' Base class for sources where photons follow some radial distribution on the sky
+    '''Base class for sources where photons follow some radial distribution on the sky
 
     Parameters
     ----------
     radial_distribution : callable
         A function that takes an interger as input, which specifies the number
-        of photons to produce. The output must be an `astropy.units.Quantity`` object
-        with n angles in it.
+        of photons to produce. The output must be an `astropy.units.Quantity`
+        object with n angles in it.
     func_par : object
-        ``radial_distribution`` has access to ``self.func_par`` to hold function
-        parameters. This could be, e.g. a tuple with coeffications.
+        ``radial_distribution`` has access to ``self.func_par`` to
+        hold function parameters. This could be, e.g. a tuple with
+        coeffications.
     kwargs : see `Source`
         Other keyword arguments include ``flux``, ``energy`` and ``polarization``.
         See `Source` for details.
+
     '''
     def __init__(self, **kwargs):
         self.func = kwargs.pop('radial_distribution')
         self.func_par = kwargs.pop('func_par', None)
-        super(RadialDistributionSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @u.quantity_input
     def generate_photons(self, exposuretime: u.s):
         '''Photon positions are generated in a frame that is centered on the
-        coordinates set in ``coords``, then they get transformed into the global sky
-        system.
+        coordinates set in ``coords``, then they get transformed into
+        the global sky system.
         '''
-        photons = super(RadialDistributionSource, self).generate_photons(exposuretime)
+        photons = super().generate_photons(exposuretime)
 
         relative_frame = SkyOffsetFrame(origin=self.coords)
         n = len(photons)
         phi = np.random.rand(n) * 2. * np.pi * u.rad
         d = self.func(n)
-        relative_coords = SkyCoord(d * np.sin(phi), d * np.cos(phi), frame=relative_frame)
+        relative_coords = SkyCoord(d * np.sin(phi), d * np.cos(phi),
+                                   frame=relative_frame)
         origin_coord = relative_coords.transform_to(self.coords)
         self.set_pos(photons, origin_coord)
 
         return photons
 
 
 class SphericalDiskSource(RadialDistributionSource):
     '''Astrophysical source with the shape of a circle or ring.
 
-    The `DiskSource` makes a small angle approximation. In contrast, this source
-    implements the full spherical geometry at the cost of running slower.
-    For radii less than a few degrees the difference is negligible and we recommend
-    use of the faster `DiskSource`.
+    The `DiskSource` makes a small angle approximation. In contrast,
+    this source implements the full spherical geometry at the cost of
+    running slower.  For radii less than a few degrees the difference
+    is negligible and we recommend use of the faster `DiskSource`.
 
     Parameters
     ----------
     a_inner, a_outer : `astropy.coordinates.Angle`
         Inner and outer angle of the ring (e.g. in arcsec).
         The default is a disk with no inner hole (``a_inner`` is set to zero.)
+
     '''
     def __init__(self, **kwargs):
         kwargs['func_par'] = [kwargs.pop('a_outer'),
                               kwargs.pop('a_inner', 0. * u.rad)]
         kwargs['radial_distribution'] = self.radial_distribution
-        super(SphericalDiskSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     def radial_distribution(self, n):
         '''Radial distribution function.
 
-        See http://6degreesoffreedom.co/circle-random-sampling/ for an explanation
-        of how to derive the formula. Note however, that here we use sin instead of cos
-        because we measure the angle from the top.
+        See http://6degreesoffreedom.co/circle-random-sampling/ for an
+        explanation of how to derive the formula. Note however, that
+        here we use sin instead of cos because we measure the angle
+        from the top.
+
         '''
         u = np.random.rand(n)
         return np.arccos(np.cos(self.func_par[1]) * (1. - u) + u * np.cos(self.func_par[0]))
 
 
 class DiskSource(RadialDistributionSource):
     '''Astrophysical source with the shape of a circle or ring.
 
-    This source uses a small angle approximation which is valid for radii less than
-    a few degrees and runs much faster. See ``SphericalDiskSource`` for an
-    implementation using full spherical geometry.
+    This source uses a small angle approximation which is valid for
+    radii less than a few degrees and runs much faster. See
+    ``SphericalDiskSource`` for an implementation using full spherical
+    geometry.
 
     Parameters
     ----------
     a_inner, a_outer : `astropy.coordinates.Angle`
         Inner and outer angle of the ring (e.g. in arcsec).
         The default is a disk with no inner hole (``a_inner`` is set to zero.)
+
     '''
     def __init__(self, **kwargs):
         kwargs['func_par'] = [kwargs.pop('a_outer'),
                               kwargs.pop('a_inner', 0. * u.rad)]
         kwargs['radial_distribution'] = lambda n: np.sqrt(self.func_par[1]**2 +
                           np.random.rand(n) * (self.func_par[0]**2 - self.func_par[1]**2))
-        super(DiskSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
 
 class GaussSource(AstroSource):
     '''Astrophysical source with a Gaussian brightness profile.
 
-    This source uses a small angle approximation which is valid for radii less than
-    a few degrees.
+    This source uses a small angle approximation which is valid for
+    radii less than a few degrees.
 
     Parameters
     ----------
     sigma : `astropy.coordinates.Angle`
         Gaussian sigma setting the width of the distribution
+
     '''
     def __init__(self, **kwargs):
         self.sigma = kwargs.pop('sigma')
-        super(GaussSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @u.quantity_input()
     def generate_photons(self, exposuretime: u.s):
         '''Photon positions are generated in a frame that is centered on the
-        coordinates set in ``coords``, then they get transformed into the global sky
-        system.
+        coordinates set in ``coords``, then they get transformed into
+        the global sky system.
+
         '''
-        photons = super(GaussSource, self).generate_photons(exposuretime)
+        photons = super().generate_photons(exposuretime)
 
         relative_frame = SkyOffsetFrame(origin=self.coords)
         n = len(photons)
-        relative_coords = SkyCoord(np.random.normal(scale=self.sigma.value, size=n) * self.sigma.unit,
-                                   np.random.normal(scale=self.sigma.value, size=n) * self.sigma.unit,
+        relative_coords = SkyCoord(np.random.normal(scale=self.sigma.value,
+                                                    size=n) * self.sigma.unit,
+                                   np.random.normal(scale=self.sigma.value,
+                                                    size=n) * self.sigma.unit,
                                    frame=relative_frame)
         origin_coord = relative_coords.transform_to(self.coords)
         self.set_pos(photons, origin_coord)
 
         return photons
 
 
@@ -469,24 +492,24 @@
     This source provides a non-symmetric source for testing purposes.
 
     Parameters
     ----------
     size : `astropy.units.quantity`
         angular size
     kwargs : see `Source`
-        Other keyword arguments include ``flux``, ``energy`` and ``polarization``.
-        See `Source` for details.
+        Other keyword arguments include ``flux``, ``energy`` and
+        ``polarization``. See `Source` for details.
     '''
     def __init__(self, **kwargs):
         self.size = kwargs.pop('size', 1. * u.degree)
-        super(SymbolFSource, self).__init__(**kwargs)
+        super().__init__(**kwargs)
 
     @u.quantity_input()
     def generate_photons(self, exposuretime: u.s):
-        photons = super(SymbolFSource, self).generate_photons(exposuretime)
+        photons = super().generate_photons(exposuretime)
         n = len(photons)
         elem = np.random.choice(3, size=n)
 
         ra = np.ones(n) * self.coords.icrs.ra
         dec = np.ones(n) * self.coords.icrs.dec
         size = self.size
         ra[elem == 0] += size * np.random.random(np.sum(elem == 0))
```

### Comparing `marxs-1.2/marxs/source/tests/test_farLabPointSource.py` & `marxs-2.0/marxs/source/tests/test_farLabPointSource.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/source/tests/test_labPointSource.py` & `marxs-2.0/marxs/source/tests/test_labPointSource.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/source/tests/test_pointing.py` & `marxs-2.0/marxs/source/tests/test_pointing.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/source/tests/test_source.py` & `marxs-2.0/marxs/source/tests/test_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from astropy.coordinates import SkyCoord
 import astropy.units as u
 
 from ...source import (SymbolFSource, Source, poisson_process,
                        PointSource,
                        DiskSource, SphericalDiskSource, GaussSource)
 from ...optics import RectangleAperture
-from ..source import SourceSpecificationError
+from ..basesources import SourceSpecificationError
 
 
 def test_photons_header():
     '''All generated photons should have some common keywords.
 
     Just test that some of the keywords are there. It's unlikely
     that I need a full list here.
```

### Comparing `marxs-1.2/marxs/tests/test_analysis.py` & `marxs-2.0/marxs/tests/test_analysis.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,16 +46,15 @@
 
     uptomirror = Sequence(elements=[aper, lens, rms])
     # CAT grating with blaze angle ensure that positive and negative orders
     # are defined the same way for all gratings in the GAS.
     blazeang = 1.91
     rowland = RowlandTorus(6000., 6000.)
     blazemat = transforms3d.axangles.axangle2mat(np.array([0, 0, 1]), np.deg2rad(blazeang))
-    gas = GratingArrayStructure(rowland=rowland, d_element=30.,
-                                x_range=[1e4, 1.4e4],
+    gas = GratingArrayStructure(rowland=rowland, d_element=[30., 30.],
                                 radius=[50, 100],
                                 elem_class=CATGrating,
                                 elem_args={'d': 1e-4, 'zoom': [1., 10., 10.],
                                            'orientation': blazemat,
                                            'order_selector': None},
                             )
     star = PointSource(coords=SkyCoord(23., 45., unit="degree"), flux=5. / u.s / u.cm**2)
@@ -69,15 +68,15 @@
     res1 = resolvingpower_per_order(gas, p.copy(), orders=o, detector=None)
     res2 = resolvingpower_per_order(gas, p.copy(), orders=o, detector=rowland)
     res3 = resolvingpower_per_order(gas, p.copy(), orders=o, detector=FlatDetector(zoom=1000))
 
     # FWHM is similar
     assert np.isclose(res1[1][0], res2[1][0], atol=0.1)
     assert np.isclose(res1[1][1], res2[1][1], atol=0.2)  # differs stronger here if fit not good
-    assert np.isclose(res2[1][0], 1.8, rtol=0.1, atol=0.1)
+    assert np.isclose(res2[1][0], 2.0, rtol=0.1, atol=0.1)
     # Resolution of 0th order is essentially 0
     assert np.isclose(res1[0][0], 0, atol=0.5)
     assert np.isclose(res2[0][0], 0, atol=0.5)
     assert np.isclose(res3[0][0], 0, atol=0.5)
     # Resolution of higher orders is consistent and higher
     assert np.isclose(res1[0][1], res2[0][1], rtol=0.1)
     assert np.isclose(res1[0][2], res2[0][2], rtol=0.2)
```

### Comparing `marxs-1.2/marxs/tests/test_simulator.py` & `marxs-2.0/marxs/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/tests/test_src_mir_det.py` & `marxs-2.0/marxs/tests/test_src_mir_det.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 import numpy as np
 import astropy.units as u
+from astropy.utils.data import get_pkg_data_filename
 
 from marxs.source.labSource import LabPointSourceCone
 from marxs.optics.multiLayerMirror import MultiLayerMirror
 from marxs.optics.detector import FlatDetector
 
+
 def test_src_mir_det():
     '''This tests that source, multilayer mirror, and detector run without producing any errors.
     '''
-    string1 = 'marxs/optics/data/A12113.txt'
-    string2 = 'marxs/optics/data/ALSpolarization2.txt'
+    string1 = get_pkg_data_filename('data/A12113.txt', package='marxs.optics')
+    string2 = get_pkg_data_filename('data/ALSpolarization2.txt', package='marxs.optics')
     a = 2**(-0.5)
     rotation1 = np.array([[a, 0, -a],
                           [0, 1, 0],
                           [a, 0, a]])
     rotation2 = np.array([[0, 0, 1],
                           [0, 1, 0],
                           [-1, 0, 0]])
```

### Comparing `marxs-1.2/marxs/visualization/mayavi.py` & `marxs-2.0/marxs/visualization/mayavi.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,67 +1,72 @@
 # Licensed under GPL version 3 - see LICENSE.rst
 '''`Mayavi <http://docs.enthought.com/mayavi/mayavi/>`__ plotting backend
 
-Mayavi is a python package for interactive 3-D displays that uses VTK underneath.
-Fuctions in this module display rays or objects in 3D using mayavi. Each of them
-requires a ``mayavi.core.scene.Scene`` instance as input and returns a mayavi object
-(or a list of those), e.g. a ``mayavi.visual.Box`` instance.
+Mayavi is a python package for interactive 3-D displays that uses VTK
+underneath.  Functions in this module display rays or objects in 3D
+using mayavi. Each of them requires a ``mayavi.core.scene.Scene``
+instance as input and returns a mayavi object (or a list of those),
+e.g. a ``mayavi.visual.Box`` instance.
+
+The plotting routines attempt to find all valid OpenGL properties by
+name in the ``display`` dictionaries and apply those to the plotted
+object.
 
-The plotting routines attempt to find all valid OpenGL properties by name in the
-``display`` dictionaries and apply those to the plotted object.
 '''
-from __future__ import absolute_import
-
 import numpy as np
 from astropy.utils.decorators import format_doc
 
 from ..math import utils as mutils
 from . import utils
 
 # The following import fails on headless servers (Travis, readthedocs).
 # from mayavi import mlab
 # Thus, I've moved the import statement into the individual functions, so that
 # this module can still be imported when Travis or readthedocs build the documentation.
 
-doc_plot='''
+doc_plot = '''
     {__doc__}
 
     Parameters
     ----------
     obj : `marxs.base.MarxsElement`
         The element that should be plotted.
     display : dict of None
         Dictionary with display settings.
     viewer : ``mayavi.core.scene.Scene instance``.
-        If None, the source is not added
-        to any figure, and will be added automatically by the modules or filters.
-        If False, no figure will be created by modules or filters applied to the
-        source: the source can only be used for testing, or numerical algorithms,
-        not visualization.
+        If None, the source is not added to any figure, and will be
+        added automatically by the modules or filters.  If False, no
+        figure will be created by modules or filters applied to the
+        source: the source can only be used for testing, or numerical
+        algorithms, not visualization.
 
     Returns
     -------
     out : mayavi object
         Return the result of a mayavi plotting method.
 '''
 
+
 @format_doc(doc_plot)
 def container(obj, display=None, viewer=None):
-    '''Recursively plot objects containted in a container.'''
+    '''Recursively plot objects contained in a container.'''
     return [plot_object(e, display=None, viewer=viewer) for e in obj.elements]
 
+
 @format_doc(doc_plot)
 def triangulation(obj, display, viewer=None):
     '''Plot a plane with an inner hole such as an aperture.'''
     from mayavi import mlab
 
     xyz, triangles = obj.geometry.triangulate(display)
-    t = mlab.triangular_mesh(xyz[:, 0], xyz[:, 1], xyz[:, 2], triangles, color=display['color'])
+    t = mlab.triangular_mesh(xyz[:, 0], xyz[:, 1], xyz[:, 2],
+                             triangles, color=display['color'])
     return t
 
+
 @format_doc(doc_plot)
 def surface(surface, display, viewer=None):
     '''Plot a parametric surface.
 
     The parameter boundaries are taken from the ``coo1`` and ``coo2`` in the
     display dictionary. The plotting routine is generic. It calls the
     ``parametric_surface()`` method of the object that is plotted; see there
@@ -75,54 +80,36 @@
     xyz = mutils.h2e(xyz)
     x = xyz[..., 0]
     y = xyz[..., 1]
     z = xyz[..., 2]
     m = mlab.mesh(x, y, z, figure=viewer, color=display['color'])
     return m
 
+
 @format_doc(doc_plot)
 def box(obj, display, viewer=None):
     '''Plot a rectangular box for an object.
 
     By default, the box extends in x,y, and z direction. The display keyword
     "box-half" can be used to show only one half of the box, e.g. "+x" would
     show  the full extend in y and z direction, but only the lower half in
     x direction (such that rays coming from the +x direction are
     visible up to the interaction point).
     Use this for elements such as mirrors or detectors where
     photon interaction happens on the surface, not in the substrate.
     '''
     from mayavi import mlab
-
-    corners = np.array([[-1, -1, -1], [-1,+1, -1],
-                        [-1, -1,  1], [-1, 1,  1],
-                        [ 1, -1, -1], [ 1, 1, -1],
-                        [ 1, -1, +1], [ 1, 1, +1]])
-    if 'box-half' in display:
-        # write in a way that it works with any value for that keyword
-        try:
-            if display['box-half'][0] == '+':
-                factor = +1
-            elif display['box-half'][0] == '-':
-                factor = -1
-            else:
-                factor = 0
-            xyz = {'x': 0, 'y': 1, 'z': 2}
-            if display['box-half'][1] in xyz:
-                j = xyz[display['box-half'][1]]
-                corners[corners[:, j] == factor, j] = 0
-        except:
-            pass
     triangles = [(0,2,6), (0,4,6), (0,1,5), (0,4,5), (0,1,3), (0,2,3),
                  (7,3,2), (7,6,2), (7,3,1), (7,5,1), (7,6,4), (7,5,4)]
-    corners = np.einsum('ij,...j->...i', obj.pos4d, mutils.e2h(corners, 1))
-    b = mlab.triangular_mesh(corners[:,0], corners[:,1], corners[:,2],
+    corners = utils.halfbox_corners(obj, display)
+    b = mlab.triangular_mesh(corners[:, 0], corners[:, 1], corners[:, 2],
                              triangles, color=display['color'])
     return b
 
+
 @format_doc(doc_plot)
 def cylinder(obj, display, viewer=None):
     '''Plot a cylinder for an object.
 
     The radius is taken from the y dimensions, the length of the tube from
     the x dimension.
     The display keyword "tube-sides" (default: 20) sets the number of vortices
@@ -134,23 +121,25 @@
     x1 = obj.geometry['center'] + obj.geometry['v_x']
     c = mlab.plot3d([x0[0], x1[0]], [x0[1], x1[1]], [x0[2], x1[2]],
                     color=display['color'],
                     tube_radius=np.linalg.norm(obj.geometry['v_y']),
                     tube_sides=display.get('tube_sides', 20))
     return c
 
+
 def plot_rays(data, scalar=None, viewer=None,
-              kwargssurface={'colormap': 'Accent', 'line_width': 1, 'opacity': .4}):
+              kwargssurface={'colormap': 'Accent', 'line_width': 1,
+                             'opacity': .4}):
     '''Plot lines for simulated rays.
 
     Parameters
     ----------
     data : np.array of shape(n, N, 3)
         where n is the number of rays, N the number of positions per ray and
-        the last dimension is the (x,y,z) of an Eukledian position vector.
+        the last dimension is the (x,y,z) of an Euclidean position vector.
     scalar : None or nd.array of shape (n,) or (n, N)
         This quantity is used to color the rays. If ``None`` all rays will have
         the same color. If it has n elements, each ray will have exactly one
         color (e.g. color according to the energy of the ray), if it has n*N
         elements, rays will be multicolored.
     viewer : ``mayavi.core.scene.Scene instance``.
        If None, the source is not added to any figure, and will be added
@@ -178,21 +167,21 @@
     elif scalar.shape == (n, ):
         s = np.repeat(scalar, N)
     elif scalar.shape == (n, N):
         s = scalar.flatten()
     else:
         raise ValueError('Scalar quantity for each point must have shape ({0},) or ({0}, {1})'.format(n, N))
 
-    x = data[:,:, 0].flatten()
-    y = data[:,:, 1].flatten()
-    z = data[:,:, 2].flatten()
+    x = data[:, :, 0].flatten()
+    y = data[:, :, 1].flatten()
+    z = data[:, :, 2].flatten()
 
     a = np.arange(n * N).reshape((-1, N))[:, :-1].flatten()
     b = a + 1
-    connections = np.vstack([a,b]).T
+    connections = np.vstack([a, b]).T
 
     # Create the points
     src = mlab.pipeline.scalar_scatter(x, y, z, s, figure=viewer)
 
     # Connect them
     src.mlab_source.dataset.lines = connections
     src.update()
@@ -201,14 +190,15 @@
     lines = mlab.pipeline.stripper(src, figure=viewer)
 
     # Finally, display the set of lines
     surface = mlab.pipeline.surface(lines, figure=viewer, **kwargssurface)
 
     return src, lines, surface
 
+
 plot_registry = {'triangulation': triangulation,
                  'surface': surface,
                  'box': box,
                  'container': container,
                  'cylinder': cylinder,
                  }
```

### Comparing `marxs-1.2/marxs/visualization/tests/test_threejsjson.py` & `marxs-2.0/marxs/visualization/tests/test_threejsjson.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     HAS_JSONSCHEMA = False
 
 
 def test_skip_plot():
     '''Test that plot is skipped with no warning if explicitly
     requested.'''
     det = FlatDetector(zoom=2, position=[2., 3., 4.])
-    # First on does not exist, but second one should lead to skip
+    # First one does not exist, but second one should lead to skip
     # with no warning
     det.display = copy.copy(det.display)
     det.display['shape'] = 'boxxx; None'
     out = plot_object(det)
 
     # check that only one warning was raised
     assert out is None
```

### Comparing `marxs-1.2/marxs/visualization/tests/test_utils.py` & `marxs-2.0/marxs/visualization/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/visualization/threejs.py` & `marxs-2.0/marxs/visualization/threejs.py`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/visualization/threejs_files/MARXSloader.js` & `marxs-2.0/marxs/visualization/threejs_files/MARXSloader.js`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/visualization/threejs_files/ModifiedTorusBufferGeometry.js` & `marxs-2.0/marxs/visualization/threejs_files/ModifiedTorusBufferGeometry.js`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/visualization/threejs_files/jsonschema.json` & `marxs-2.0/marxs/visualization/threejs_files/jsonschema.json`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/visualization/threejs_files/loader.html` & `marxs-2.0/marxs/visualization/threejs_files/loader.html`

 * *Files identical despite different names*

### Comparing `marxs-1.2/marxs/visualization/threejsjson.py` & `marxs-2.0/marxs/visualization/threejsjson.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 - otherwise:
   - ``pos4d``: list of lists of 16 numbers
   - ``geometrypars``: list (meaning depends on geometry, e.g. radius of torus)
 '''
 import os
 import json
 import datetime
+import warnings
 import numpy as np
 from astropy.utils.decorators import format_doc
 
 from ..version import version
 from . import threejs
 from . import utils
 
@@ -57,15 +58,15 @@
     ----------
     obj : `marxs.base.MarxsElement`
         The element that should be plotted.
     display : dict of None
         Dictionary with display settings.
 
     Returns
-    --------
+    -------
     outjson : dict
         ``outjson`` is a (possibly nested)  dictionaries that describes the scene
         in form that the included MARXSloader.js can read.
 '''
 
 
 @format_doc(doc_plot)
@@ -75,15 +76,15 @@
     This method will inspect the object that is passed in and select the
     correct plotting method for its shape.
     '''
     return utils.plot_object_general(plot_registry, obj, display=display, **kwargs)
 
 
 def container(obj, display=None,  **kwargs):
-    ''''Recursivey output three.js json to describe all elements of a container.
+    ''''Recursively output three.js json to describe all elements of a container.
 
     Output of each element can be a dict (if it is a leaf) or a list
     (if it is a container). We need to flatten the list here to avoid
     arbitrarily deep recursion.
     '''
     out = []
     for elem in obj.elements:
```

