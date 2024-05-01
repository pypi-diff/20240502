# Comparing `tmp/vollseg_napari_trackmate-2.5.8.tar.gz` & `tmp/vollseg_napari_trackmate-2.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vollseg_napari_trackmate-2.5.8.tar", last modified: Sun Apr 28 11:12:44 2024, max compression
+gzip compressed data, was "vollseg_napari_trackmate-2.5.9.tar", last modified: Wed May  1 22:12:06 2024, max compression
```

## Comparing `vollseg_napari_trackmate-2.5.8.tar` & `vollseg_napari_trackmate-2.5.9.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.442908 vollseg_napari_trackmate-2.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.434908 vollseg_napari_trackmate-2.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.438908 vollseg_napari_trackmate-2.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.github/workflows/napari-hub-preview.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.github/workflows/test_and_deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.438908 vollseg_napari_trackmate-2.5.8/.napari-hub/
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.napari-hub/DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.napari-hub/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/ALGORITHM.md
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/MITOSIS.md
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-28 11:12:44.442908 vollseg_napari_trackmate-2.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/RADIAL_ANGLE.md
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/_config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/_toc.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.438908 vollseg_napari_trackmate-2.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/examples/annotate_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/examples/apply_autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/examples/create_oneat_patches.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/examples/train_oneat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/examples/visualize_point_clouds.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-04-28 11:12:44.442908 vollseg_napari_trackmate-2.5.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.434908 vollseg_napari_trackmate-2.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.438908 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_data_model.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_temporal_plots.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.442908 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    73158 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_widget.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/launch.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.442908 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/resources/kapoorlogo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-28 11:12:44.442908 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-04-28 11:12:43.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-04-28 11:12:44.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-28 11:12:43.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-28 11:12:43.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-28 11:12:43.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-28 11:12:43.000000 vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/tox.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-28 11:12:32.000000 vollseg_napari_trackmate-2.5.8/update_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.840549 vollseg_napari_trackmate-2.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.832548 vollseg_napari_trackmate-2.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.836548 vollseg_napari_trackmate-2.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.github/workflows/napari-hub-preview.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.github/workflows/test_and_deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.836548 vollseg_napari_trackmate-2.5.9/.napari-hub/
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.napari-hub/DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.napari-hub/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5579 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/ALGORITHM.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/MITOSIS.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-01 22:12:06.840549 vollseg_napari_trackmate-2.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/RADIAL_ANGLE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-01 22:11:53.000000 vollseg_napari_trackmate-2.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/_toc.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.836548 vollseg_napari_trackmate-2.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/examples/annotate_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/examples/apply_autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/examples/create_oneat_patches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/examples/train_oneat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/examples/visualize_point_clouds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-01 22:12:06.840549 vollseg_napari_trackmate-2.5.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.832548 vollseg_napari_trackmate-2.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.836548 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2118 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_temporal_plots.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.840549 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72398 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/launch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.840549 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/resources/kapoorlogo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 22:12:06.840549 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5000 2024-05-01 22:12:06.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-01 22:12:06.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 22:12:06.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-01 22:12:06.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-01 22:12:06.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-01 22:12:06.000000 vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/tox.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-01 22:11:54.000000 vollseg_napari_trackmate-2.5.9/update_version.py
```

### Comparing `vollseg_napari_trackmate-2.5.8/.github/workflows/deploy.yml` & `vollseg_napari_trackmate-2.5.9/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/.github/workflows/napari-hub-preview.yml` & `vollseg_napari_trackmate-2.5.9/.github/workflows/napari-hub-preview.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/.github/workflows/test_and_deploy.yml` & `vollseg_napari_trackmate-2.5.9/.github/workflows/test_and_deploy.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/.gitignore` & `vollseg_napari_trackmate-2.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/.napari-hub/DESCRIPTION.md` & `vollseg_napari_trackmate-2.5.9/.napari-hub/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/.napari-hub/config.yml` & `vollseg_napari_trackmate-2.5.9/.napari-hub/config.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/.pre-commit-config.yaml` & `vollseg_napari_trackmate-2.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/ALGORITHM.md` & `vollseg_napari_trackmate-2.5.9/ALGORITHM.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/LICENSE` & `vollseg_napari_trackmate-2.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/MITOSIS.md` & `vollseg_napari_trackmate-2.5.9/MITOSIS.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/PKG-INFO` & `vollseg_napari_trackmate-2.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.8
+Version: 2.5.9
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg_napari_trackmate-2.5.8/README.md` & `vollseg_napari_trackmate-2.5.9/README.md`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/_config.yml` & `vollseg_napari_trackmate-2.5.9/_config.yml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/examples/apply_autoencoder.py` & `vollseg_napari_trackmate-2.5.9/examples/apply_autoencoder.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/examples/create_oneat_patches.py` & `vollseg_napari_trackmate-2.5.9/examples/create_oneat_patches.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/examples/train_oneat.py` & `vollseg_napari_trackmate-2.5.9/examples/train_oneat.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/examples/visualize_point_clouds.py` & `vollseg_napari_trackmate-2.5.9/examples/visualize_point_clouds.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/setup.cfg` & `vollseg_napari_trackmate-2.5.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_data_model.py` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_data_model.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_temporal_plots.py` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_temporal_plots.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_tests/test_widget.py` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/_widget.py` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/_widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -387,15 +387,14 @@
                         )
                         (
                             cluster_time,
                             cluster_z,
                             cluster_y,
                             cluster_x,
                             cluster_radius,
-                            cluster_radius_pixel,
                             cluster_eccentricity_comp_first,
                             cluster_eccentricity_comp_second,
                             cluster_eccentricity_comp_third,
                             cluster_local_cell_density,
                             cluster_surface_area,
                             _,
                         ) = unique_shape_properties_tracklet
@@ -445,15 +444,14 @@
                         unique_shape_properties.append(
                             [
                                 cluster_time,
                                 cluster_z,
                                 cluster_y,
                                 cluster_x,
                                 cluster_radius,
-                                cluster_radius_pixel,
                                 cluster_eccentricity_comp_first,
                                 cluster_eccentricity_comp_second,
                                 cluster_eccentricity_comp_third,
                                 cluster_local_cell_density,
                                 cluster_surface_area,
                                 countk + 1,
                             ]
@@ -541,36 +539,34 @@
                                 )
 
                         for count, i in enumerate(range(len(unique_shape_properties))):
 
                             current_unique_shape_properties = unique_shape_properties[i]
                             cluster_time = current_unique_shape_properties[0]
                             cluster_radius = current_unique_shape_properties[1]
-                            cluster_radius_pixel = current_unique_shape_properties[2]
                             cluster_eccentricity_comp_first = (
-                                current_unique_shape_properties[3]
+                                current_unique_shape_properties[2]
                             )
                             cluster_eccentricity_comp_second = (
-                                current_unique_shape_properties[4]
+                                current_unique_shape_properties[3]
                             )
                             cluster_eccentricity_comp_third = (
-                                current_unique_shape_properties[5]
+                                current_unique_shape_properties[4]
                             )
                             cluster_local_cell_density = (
-                                current_unique_shape_properties[6]
+                                current_unique_shape_properties[5]
                             )
-                            cluster_surface_area = current_unique_shape_properties[7]
+                            cluster_surface_area = current_unique_shape_properties[6]
 
                             cluster_id = current_unique_shape_properties[-1]
 
                             data_cluster_plot = pd.DataFrame(
                                 {
                                     "Time": cluster_time,
                                     "Radius": cluster_radius,
-                                    "Radius_Pixel": cluster_radius_pixel,
                                     "Eccentricity_Comp_First": cluster_eccentricity_comp_first,
                                     "Eccentricity_Comp_Second": cluster_eccentricity_comp_second,
                                     "Eccentricity_Comp_Third": cluster_eccentricity_comp_third,
                                     "Local_Cell_Density": cluster_local_cell_density,
                                     "Surface_Area": cluster_surface_area,
                                     "id": cluster_id,
                                 }
@@ -793,28 +789,15 @@
                     ax=plot_ax,
                     legend=False,
                 )
 
                 plot_ax.set_title("Radius")
                 plot_ax.set_xlabel("Time (sec)")
 
-                phenotype_plot_class._repeat_after_plot()
-                plot_ax = phenotype_plot_class.plot_ax
-                sns.set_palette(flatui)
-                sns.lineplot(
-                    global_data_cluster_plot,
-                    x="Time",
-                    y="Radius_Pixel",
-                    hue="id",
-                    ax=plot_ax,
-                    legend=False,
-                )
-
-                plot_ax.set_title("Radius_Pixel")
-                plot_ax.set_xlabel("Time (sec)")
+              
 
                 phenotype_plot_class._repeat_after_plot()
                 plot_ax = phenotype_plot_class.plot_ax
                 sns.set_palette(flatui)
                 sns.lineplot(
                     global_data_cluster_plot,
                     x="Time",
```

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/napari.yaml` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/napari.yaml`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate/resources/kapoorlogo.png` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate/resources/kapoorlogo.png`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/PKG-INFO` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vollseg-napari-trackmate
-Version: 2.5.8
+Version: 2.5.9
 Summary: Track analysis using TrackMate xml and csv generated tracks using NapaTrackMater as the base library
 Home-page: https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate
 Author: Varun Kapoor, Mari Tolonen, Jakub Sedzinski
 Author-email: randomaccessiblekapoor@gmail.com
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate/issues
 Project-URL: Documentation, https://github.com/Kapoorlabs-CAPED/vollseg-napari-trackmate#README.md
```

### Comparing `vollseg_napari_trackmate-2.5.8/src/vollseg_napari_trackmate.egg-info/SOURCES.txt` & `vollseg_napari_trackmate-2.5.9/src/vollseg_napari_trackmate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/tox.ini` & `vollseg_napari_trackmate-2.5.9/tox.ini`

 * *Files identical despite different names*

### Comparing `vollseg_napari_trackmate-2.5.8/update_version.py` & `vollseg_napari_trackmate-2.5.9/update_version.py`

 * *Files identical despite different names*

