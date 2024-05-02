# Comparing `tmp/vsensebox-0.1.0.tar.gz` & `tmp/vsensebox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vsensebox-0.1.0.tar", last modified: Thu Apr 11 18:57:51 2024, max compression
+gzip compressed data, was "vsensebox-0.1.1.tar", last modified: Thu May  2 13:26:07 2024, max compression
```

## Comparing `vsensebox-0.1.0.tar` & `vsensebox-0.1.1.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.154204 vsensebox-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6728 2024-04-11 18:57:45.000000 vsensebox-0.1.0/GETSTARTED.md
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-11 18:57:45.000000 vsensebox-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 18:57:45.000000 vsensebox-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-11 18:57:51.150205 vsensebox-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-11 18:57:45.000000 vsensebox-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1650 2024-04-11 18:57:45.000000 vsensebox-0.1.0/RELEASENOTES.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-11 18:57:45.000000 vsensebox-0.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.138205 vsensebox-0.1.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 18:57:45.000000 vsensebox-0.1.0/requirements/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-04-11 18:57:45.000000 vsensebox-0.1.0/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 18:57:51.154204 vsensebox-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-04-11 18:57:45.000000 vsensebox-0.1.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-04-11 18:57:45.000000 vsensebox-0.1.0/setup_extra.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.142205 vsensebox-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-11 18:57:45.000000 vsensebox-0.1.0/tests/pretests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-11 18:57:45.000000 vsensebox-0.1.0/tests/test_01.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.142205 vsensebox-0.1.0/vsensebox/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.142205 vsensebox-0.1.0/vsensebox/config/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/confighelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/configurator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.142205 vsensebox-0.1.0/vsensebox/config/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.142205 vsensebox-0.1.0/vsensebox/config/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/detectors.zip
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.142205 vsensebox-0.1.0/vsensebox/config/strings/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/strings/strings.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/strings/strings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/config/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/trackers/basiciou.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/trackers/centroid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/trackers/deepsort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/trackers/default.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/trackers/sort.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/config/trackers/trackers.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/data/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/data/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/datasets/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/data/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/detectors/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/data/logs/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/logs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/data/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/data/trackers/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/gui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/gui/assets/
--rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/gui/assets/settings.ico
--rw-r--r--   0 runner    (1001) docker     (127)    53774 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/gui/cfgloader_ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/gui/uitools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.146205 vsensebox-0.1.0/vsensebox/modules/detectors/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/detectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/detectors/detectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/detectors/yolo_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/detectors/yolo_ultralytics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.150205 vsensebox-0.1.0/vsensebox/modules/trackers/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/basiciou.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/centroid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/deepsort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/trackers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.150205 vsensebox-0.1.0/vsensebox/modules/trackers/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/box_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/detection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/detection_yolo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/generate_detections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/iou_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/kalman_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/linear_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/nn_matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/preprocessing.py
--rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/modules/trackers/utils/voc_classes.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.150205 vsensebox-0.1.0/vsensebox/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/utils/about.py
--rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/utils/commontools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/utils/logtools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/utils/visualizetools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.150205 vsensebox-0.1.0/vsensebox/vsense/
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/vsense/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-04-11 18:57:45.000000 vsensebox-0.1.0/vsensebox/vsense/vsense.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:57:51.150205 vsensebox-0.1.0/vsensebox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4005 2024-04-11 18:57:51.000000 vsensebox-0.1.0/vsensebox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-11 18:57:51.000000 vsensebox-0.1.0/vsensebox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:57:51.000000 vsensebox-0.1.0/vsensebox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-11 18:57:51.000000 vsensebox-0.1.0/vsensebox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 18:57:51.000000 vsensebox-0.1.0/vsensebox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     6725 2024-05-02 13:25:57.000000 vsensebox-0.1.1/GETSTARTED.md
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-02 13:25:57.000000 vsensebox-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-02 13:25:57.000000 vsensebox-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-02 13:26:07.386489 vsensebox-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-02 13:25:57.000000 vsensebox-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2008 2024-05-02 13:25:57.000000 vsensebox-0.1.1/RELEASENOTES.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-02 13:25:58.000000 vsensebox-0.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.374489 vsensebox-0.1.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:25:58.000000 vsensebox-0.1.1/requirements/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-02 13:25:58.000000 vsensebox-0.1.1/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 13:26:07.386489 vsensebox-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2024-05-02 13:25:58.000000 vsensebox-0.1.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-02 13:25:58.000000 vsensebox-0.1.1/setup_extra.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.374489 vsensebox-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-02 13:25:58.000000 vsensebox-0.1.1/tests/pretests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-02 13:25:58.000000 vsensebox-0.1.1/tests/test_01.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.374489 vsensebox-0.1.1/vsensebox/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7888 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/confighelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/configurator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2551 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/detectors.zip
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_classic_v3tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_classic_v4tiny.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v3tinyu.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v5su.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v8n.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v8s.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/detectors/yolo_ultralytics_v9c.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/strings/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/strings/strings.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/strings/strings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.378489 vsensebox-0.1.1/vsensebox/config/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/basiciou.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/centroid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/deepsort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/default.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/sort.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/config/trackers/trackers.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/datasets/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/detectors/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/logs/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/logs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/data/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/data/trackers/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/gui/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)    33692 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/assets/settings.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    53774 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/cfgloader_ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/gui/uitools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/modules/detectors/
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/detectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/yolo_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4251 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/detectors/yolo_ultralytics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.382489 vsensebox-0.1.1/vsensebox/modules/trackers/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/basiciou.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/centroid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3425 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/deepsort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/trackers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox/modules/trackers/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/box_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection_yolo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8347 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/generate_detections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2864 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/iou_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7787 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/kalman_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7941 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/linear_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5470 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/nn_matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/preprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11819 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4976 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5292 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/modules/trackers/utils/voc_classes.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/about.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5154 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/commontools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3172 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/logtools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/utils/visualizetools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox/vsense/
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/vsense/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-02 13:25:58.000000 vsensebox-0.1.1/vsensebox/vsense/vsense.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 13:26:07.386489 vsensebox-0.1.1/vsensebox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-02 13:26:07.000000 vsensebox-0.1.1/vsensebox.egg-info/top_level.txt
```

### Comparing `vsensebox-0.1.0/GETSTARTED.md` & `vsensebox-0.1.1/GETSTARTED.md`

 * *Files 2% similar despite different names*

```diff
@@ -115,8 +115,8 @@
 
 ### 1️⃣ Customized OpenCV
 
 OpenCV is widely used in many well-known packages, but the majority of the prebuilt WHLs on the Internet including the official one on PyPI do not include GPU support. Thus, we build our custom one which includes NVIDIA [CUDA](https://developer.nvidia.com/cuda-downloads) & [cuDNN](https://developer.nvidia.com/rdp/cudnn-download) supports for the [OpenCV DNN module](https://docs.opencv.org/4.x/d2/d58/tutorial_table_of_content_dnn.html). In order to well distinguish from the rest, we decided to build and change the package name from `opencv-contrib-python` to [`pyppbox-opencv`](https://github.com/rathaumons/opencv-for-pyppbox) -> [[Repo]](https://github.com/rathaumons/opencv-for-pyppbox) [[WHL]](https://github.com/rathaumons/opencv-for-pyppbox/releases)
 
 ### 2️⃣ Customized Ultralytics
 
-Also, similar to `pyppbox-opencv`, our custom `ultralytics` is changed to [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `pyppbox` and `vsensebox` need the customized `pyppbox-ultralytics` -> [[Repo]](https://github.com/rathaumons/ultralytics-for-pyppbox) [[PyPI]](https://pypi.org/project/pyppbox-ultralytics/)
+Also, similar to `pyppbox-opencv`, our custom `ultralytics` is changed to [`vsensebox-ultralytics`](https://github.com/rathaumons/ultralytics-for-vsensebox), but this time, the module name is still the same `ultralytics` and it is the main reason why the official `ultralytics` must be removed. Find out more why `VSenseBox` needs the customized `vsensebox-ultralytics` -> [[Repo]](https://github.com/rathaumons/ultralytics-for-vsensebox) [[PyPI]](https://pypi.org/project/vsensebox-ultralytics/)
```

### Comparing `vsensebox-0.1.0/LICENSE` & `vsensebox-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/PKG-INFO` & `vsensebox-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.1.0
+Version: 0.1.1
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
@@ -45,17 +45,17 @@
 Requires-Dist: future
 Requires-Dist: protobuf
 Requires-Dist: tensorflow
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: filterpy
-Requires-Dist: lapx
+Requires-Dist: lapx>=0.5.8
 Requires-Dist: PyQt6
-Requires-Dist: pyppbox-ultralytics>=8.0.218
+Requires-Dist: vsensebox-ultralytics>=8.1.48
 
 # 👁️📦 [**VSenseBox**](https://github.com/rathaumons/vsensebox)
 
 <div align="center">
 
 [![Documentation](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml)
```

### Comparing `vsensebox-0.1.0/README.md` & `vsensebox-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/RELEASENOTES.md` & `vsensebox-0.1.1/RELEASENOTES.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Release Notes 
 
 ## **VSenseBox v0.1.x - One Small Step!**
 
+* `VSenseBox` [v0.1.1](https://github.com/rathaumons/vsensebox/tree/v0.1.1)
+  - Replace [`pyppbox-ultralytics`](https://github.com/rathaumons/ultralytics-for-pyppbox) with [`vsensebox-ultralytics`](https://github.com/rathaumons/ultralytics-for-vsensebox)
+  - Use `lapx>=0.5.8` for speed boost
+  - Update and improve documentation
+  - Update GitHub workflow
+
 * `VSenseBox` [v0.1.0](https://github.com/rathaumons/vsensebox/tree/v0.1.0)
   - Add basic IoU tracker -> `BasicIoU`
   - Fix minor bugs
   - Clean up and improve unified strings
   - Update and improve configurator and GUI
   - Update and improve documentation
```

### Comparing `vsensebox-0.1.0/requirements/requirements.txt` & `vsensebox-0.1.1/requirements/requirements.txt`

 * *Files 20% similar despite different names*

```diff
@@ -25,12 +25,12 @@
 # Please follow the installation on:
 # https://pytorch.org/get-started
 torch
 torchvision
 torchaudio
 ### Tracker: SORT
 filterpy
-lapx
+lapx>=0.5.8
 ### GUI
 PyQt6
-### Customized pyppbox-ultralytics
-pyppbox-ultralytics>=8.0.218
+### Customized vsensebox-ultralytics
+vsensebox-ultralytics>=8.1.48
```

### Comparing `vsensebox-0.1.0/setup.py` & `vsensebox-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/setup_extra.yaml` & `vsensebox-0.1.1/setup_extra.yaml`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/tests/pretests.py` & `vsensebox-0.1.1/tests/pretests.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/tests/test_01.py` & `vsensebox-0.1.1/tests/test_01.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/__init__.py` & `vsensebox-0.1.1/vsensebox/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # Copyright (C) 2024 UMONS-Numediart
 
 
 from vsensebox.vsense import VSense
 from vsensebox.gui import config, reset
 from vsensebox.utils.about import docs, github
 
-__version__ = "0.1.0"
+__version__ = "0.1.1"
 __author__ = "Ratha SIV"
 __description__ = "VSenseBox - Python toolbox for visual sensing."
 __homepage__ = "https://rathaumons.github.io/vsensebox"
 __url__ = "https://github.com/rathaumons/vsensebox.git"
 
 __all__ = (
     "__version__",
```

### Comparing `vsensebox-0.1.0/vsensebox/config/confighelper.py` & `vsensebox-0.1.1/vsensebox/config/confighelper.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/config/configurator.py` & `vsensebox-0.1.1/vsensebox/config/configurator.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/config/detectors/detectors.zip` & `vsensebox-0.1.1/vsensebox/config/detectors/detectors.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/config/strings.py` & `vsensebox-0.1.1/vsensebox/config/strings.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/config/trackers/trackers.zip` & `vsensebox-0.1.1/vsensebox/config/trackers/trackers.zip`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/gui/assets/settings.ico` & `vsensebox-0.1.1/vsensebox/gui/assets/settings.ico`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/gui/cfgloader_ui.py` & `vsensebox-0.1.1/vsensebox/gui/cfgloader_ui.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/gui/uitools.py` & `vsensebox-0.1.1/vsensebox/gui/uitools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/detectors/detectors.py` & `vsensebox-0.1.1/vsensebox/modules/detectors/detectors.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/detectors/yolo_classic.py` & `vsensebox-0.1.1/vsensebox/modules/detectors/yolo_classic.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/detectors/yolo_ultralytics.py` & `vsensebox-0.1.1/vsensebox/modules/detectors/yolo_ultralytics.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/basiciou.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/basiciou.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/centroid.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/centroid.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/deepsort.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/deepsort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/sort.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/trackers.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/trackers.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/box_matching.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/box_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/detection.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/detection_yolo.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/detection_yolo.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/generate_detections.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/generate_detections.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/iou_matching.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/iou_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/kalman_filter.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/linear_assignment.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/linear_assignment.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/nn_matching.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/nn_matching.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/preprocessing.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/preprocessing.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/sort.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/sort.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/track.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/track.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/modules/trackers/utils/tracker.py` & `vsensebox-0.1.1/vsensebox/modules/trackers/utils/tracker.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/utils/about.py` & `vsensebox-0.1.1/vsensebox/utils/about.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/utils/commontools.py` & `vsensebox-0.1.1/vsensebox/utils/commontools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/utils/logtools.py` & `vsensebox-0.1.1/vsensebox/utils/logtools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/utils/visualizetools.py` & `vsensebox-0.1.1/vsensebox/utils/visualizetools.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox/vsense/vsense.py` & `vsensebox-0.1.1/vsensebox/vsense/vsense.py`

 * *Files identical despite different names*

### Comparing `vsensebox-0.1.0/vsensebox.egg-info/PKG-INFO` & `vsensebox-0.1.1/vsensebox.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vsensebox
-Version: 0.1.0
+Version: 0.1.1
 Summary: VSenseBox - Python toolbox for visual sensing.
 Home-page: https://github.com/rathaumons/vsensebox
 Author: Ratha SIV
 Maintainer: rathaROG
 License: GPL-3.0-or-later
 Keywords: Toolbox,Detect,Track,Visual,Sense
 Classifier: Development Status :: 4 - Beta
@@ -45,17 +45,17 @@
 Requires-Dist: future
 Requires-Dist: protobuf
 Requires-Dist: tensorflow
 Requires-Dist: torch
 Requires-Dist: torchvision
 Requires-Dist: torchaudio
 Requires-Dist: filterpy
-Requires-Dist: lapx
+Requires-Dist: lapx>=0.5.8
 Requires-Dist: PyQt6
-Requires-Dist: pyppbox-ultralytics>=8.0.218
+Requires-Dist: vsensebox-ultralytics>=8.1.48
 
 # 👁️📦 [**VSenseBox**](https://github.com/rathaumons/vsensebox)
 
 <div align="center">
 
 [![Documentation](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/documentation.yaml) [![Publish on PyPI](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/publish_pypi.yaml) [![Test Build](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml/badge.svg)](https://github.com/rathaumons/vsensebox/actions/workflows/test_build.yaml)
```

### Comparing `vsensebox-0.1.0/vsensebox.egg-info/SOURCES.txt` & `vsensebox-0.1.1/vsensebox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

