# Comparing `tmp/AnimatedWordCloudTimelapse-1.0.8.tar.gz` & `tmp/animatedwordcloudtimelapse-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AnimatedWordCloudTimelapse-1.0.8.tar", last modified: Sun Jan  7 16:12:05 2024, max compression
+gzip compressed data, was "animatedwordcloudtimelapse-1.0.9.tar", last modified: Thu May  2 06:08:44 2024, max compression
```

## Comparing `AnimatedWordCloudTimelapse-1.0.8.tar` & `animatedwordcloudtimelapse-1.0.9.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.786288 AnimatedWordCloudTimelapse-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.778288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.778288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.778288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/AllocationCalculator.py
--rw-r--r--   0 runner    (1001) docker     (127)     8829 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/AnimatetdAllocationCalculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.778288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/
--rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationCalculator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.778288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.782288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/
--rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagnetOuterFrontier.py
--rw-r--r--   0 runner    (1001) docker     (127)    12824 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagneticAllocation.py
--rw-r--r--   0 runner    (1001) docker     (127)      221 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/RandomAllocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/StaticAllocationStrategy.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AnimationIntegrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/Animator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/ImageCreator.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.778288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.782288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Assets/Fonts/
--rw-r--r--   0 runner    (1001) docker     (127)  1707908 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Assets/Fonts/NotoSansMono-VariableFont_wdth,wght.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.782288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Collisions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Config.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Consts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.786288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/
--rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/AllocationData.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/Rect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/TimelapseWordVector.py
--rw-r--r--   0 runner    (1001) docker     (127)      650 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/Word.py
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/FileManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Vector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 16:12:05.786288 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-01-07 16:12:05.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-01-07 16:12:05.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 16:12:05.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 16:12:05.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-01-07 16:12:05.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-07 16:12:05.000000 AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9898 2024-01-07 16:12:05.786288 AnimatedWordCloudTimelapse-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 16:12:05.786288 AnimatedWordCloudTimelapse-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-01-07 16:11:59.000000 AnimatedWordCloudTimelapse-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.980509 animatedwordcloudtimelapse-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.972509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.972509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.972509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/AllocationCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/AnimatetdAllocationCalculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.972509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/
+-rw-r--r--   0 runner    (1001) docker     (127)     5796 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationCalculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.972509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.976509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/
+-rw-r--r--   0 runner    (1001) docker     (127)    12905 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagnetOuterFrontier.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13325 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagneticAllocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      221 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/RandomAllocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/StaticAllocationStrategy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1634 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AnimationIntegrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/Animator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/ImageCreator.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.972509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.976509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Assets/Fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)  1707908 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Assets/Fonts/NotoSansMono-VariableFont_wdth,wght.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.976509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Collisions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7355 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Consts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.980509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2425 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/AllocationData.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/Rect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6465 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/TimelapseWordVector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      650 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/Word.py
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/FileManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3451 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Vector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 06:08:44.980509 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-02 06:08:44.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-02 06:08:44.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:08:44.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 06:08:44.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-02 06:08:44.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-02 06:08:44.000000 animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-02 06:08:44.980509 animatedwordcloudtimelapse-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 06:08:44.980509 animatedwordcloudtimelapse-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-02 06:08:38.000000 animatedwordcloudtimelapse-1.0.9/setup.py
```

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/AllocationCalculator.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/AllocationCalculator.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/AnimatetdAllocationCalculator.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/AnimatetdAllocationCalculator.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,15 @@
         # get static frame data
         from_allocation_frame = allocation_timelapse.get_frame(index)
         to_allocation_frame = allocation_timelapse.get_frame(index + 1)
         time_name_from = allocation_timelapse.timelapse[index][0]
         time_name_to = allocation_timelapse.timelapse[index + 1][0]
 
         # interpolate between two frames
-        interpolated_frames: list[
-            AllocationInFrame
-        ] = _get_interpolated_frames(
+        interpolated_frames = _get_interpolated_frames(
             from_allocation_frame,
             to_allocation_frame,
             config,
         )
 
         # add static frame first
         timelapse_output.add(time_name_from, from_allocation_frame)
```

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationCalculator.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationCalculator.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagnetOuterFrontier.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagnetOuterFrontier.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagneticAllocation.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/MagneticAllocation/MagneticAllocation.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 Repeating this process, all words will be allocated.
 """
 
 from __future__ import annotations
 import math
 from typing import Iterable
 from tqdm import tqdm
-import joblib
 from AnimatedWordCloud.Utils import (
     is_rect_hitting_rects,
     AllocationInFrame,
     Vector,
     Rect,
     Word,
     Config,
@@ -226,23 +225,17 @@
             magnet_outer_frontier.from_down,
             magnet_outer_frontier.from_up,
             magnet_outer_frontier.from_left,
             magnet_outer_frontier.from_right,
         ]
 
         # get center position candidates
-        results_by_sides = joblib.Parallel(n_jobs=-1, verbose=0)(
-            joblib.delayed(self._get_candidates_from_one_side)(
-                pivots_to_center_list[cnt], frontier_sides[cnt]
-            )
-            for cnt in range(4)
+        center_position_candidates = self._compute_candidates(
+            pivots_to_center_list, frontier_sides
         )
-        center_position_candidates = []
-        for results_by_side in results_by_sides:
-            center_position_candidates.extend(results_by_side)
 
         # error handling: too small image area that cannot put the word anywhere anymore
         if len(center_position_candidates) == 0:
             raise Exception(
                 "No available position found. Try to reduce font size or expand image size."
             )
 
@@ -255,14 +248,39 @@
         best_position_left_top = (
             best_position[0] - word.text_size[0] / 2,
             best_position[1] - word.text_size[1] / 2,
         )
 
         return best_position_left_top
 
+    def _compute_candidates(
+        self,
+        pivots_to_center_list: Iterable[Iterable[Vector]],
+        frontier_sides: Iterable[Iterable[Vector]],
+    ) -> list[tuple[int, int]]:
+        """
+        Compute all candidates of the center position
+
+        :param Iterable[Iterable[Vector]] pivots_to_center_list:
+            List of vectors from the pivot to the center of the word
+        :param Iterable[Iterable[Vector]]
+            List of vectors from the frontier to the center of the word
+        :return: Candidates of the center position
+        """
+
+        center_position_candidates = []
+        for cnt in range(4):
+            center_position_candidates.extend(
+                self._get_candidates_from_one_side(
+                    pivots_to_center_list[cnt], frontier_sides[cnt]
+                )
+            )
+
+        return center_position_candidates
+
     def _get_candidates_from_one_side(
         self,
         pivots_to_center: Iterable[Vector],
         points_on_side: Iterable[Vector],
     ) -> list[tuple[int, int]]:
         """
         Get all candidates of the center position from one side
@@ -299,20 +317,18 @@
         :param tuple[int,int] size: Size of the word
         :param tuple[int,int] position_from:
             Position of the center of the word comming from
         :return: Best center position
         :rtype: tuple[int, int]
         """
 
-        results_evaluation = joblib.Parallel(n_jobs=-1, verbose=0)(
-            joblib.delayed(self._try_put_position)(
-                center_position, size, position_from
-            )
+        results_evaluation = [
+            self._try_put_position(center_position, size, position_from)
             for center_position in center_positions
-        )
+        ]
 
         # find best score
         best_position = None
         best_score = -float("inf")
         for cnt, result_evaluation in enumerate(results_evaluation):
             if (result_evaluation is not None) and (
                 result_evaluation > best_score
```

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/RandomAllocation.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/RandomAllocation.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/StaticAllocationStrategy.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/StaticAllocationStrategy.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/__init__.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AllocationCalculator/StaticAllocationCalculator/StaticAllocationStrategies/__init__.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/AnimationIntegrator.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/AnimationIntegrator.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/Animator.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/Animator.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Animator/ImageCreator.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Animator/ImageCreator.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Assets/Fonts/NotoSansMono-VariableFont_wdth,wght.ttf` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Assets/Fonts/NotoSansMono-VariableFont_wdth,wght.ttf`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Collisions.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Collisions.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Config.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Config.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Consts.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Consts.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/AllocationData.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/AllocationData.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/Rect.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/Rect.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/TimelapseWordVector.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/TimelapseWordVector.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Data/Word.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Data/Word.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/FileManager.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/FileManager.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/Vector.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/Vector.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloud/Utils/__init__.py` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloud/Utils/__init__.py`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/PKG-INFO` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimatedWordCloudTimelapse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Animate a timelapse of word cloud
 Home-page: https://github.com/konbraphat51/AnimatedWordCloud/tree/main
 Author: konbraphat51, superhotdogcat
 Author-email: konbraphat51@gmail.com, siromisochan@gmail.com
 License: MIT License
 Project-URL: GitHub Repository, https://github.com/konbraphat51/AnimatedWordCloud
 Keywords: NLP,World Cloud,Animation,Natural Language Processing,video,Visualization,Data Science
@@ -16,23 +16,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow==10.1.0
+Requires-Dist: Pillow==10.3.0
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: joblib
 Requires-Dist: tqdm
 
-# AnimatedWordCloud ver 1.0.8
-
-**UNDER CONSTRUCTION**
+# AnimatedWordCloud ver 1.0.9
 
 <a href="https://codeclimate.com/github/konbraphat51/AnimatedWordCloud/maintainability"><img src="https://api.codeclimate.com/v1/badges/7a03252f77e7af46dc0f/maintainability" /></a>
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/gh/konbraphat51/AnimatedWordCloud/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![unit-test](https://github.com/konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml/badge.svg?branch=main)](https://github.com/konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml)[![codecov](https://codecov.io/gh/konbraphat51/AnimatedWordCloud/graph/badge.svg?token=4OOX0GSJDJ)](https://codecov.io/gh/konbraphat51/AnimatedWordCloud)
 
 AnimatedWordCloud animates the timelapse of your words vector.
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1 Name: AnimatedWordCloudTimelapse Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: AnimatedWordCloudTimelapse Version: 1.0.9 Summary:
 Animate a timelapse of word cloud Home-page: https://github.com/konbraphat51/
 AnimatedWordCloud/tree/main Author: konbraphat51, superhotdogcat Author-email:
 konbraphat51@gmail.com, siromisochan@gmail.com License: MIT License Project-
 URL: GitHub Repository, https://github.com/konbraphat51/AnimatedWordCloud
 Keywords: NLP,World Cloud,Animation,Natural Language
 Processing,video,Visualization,Data Science Classifier: Development Status :: 1
 - Planning Classifier: Programming Language :: Python :: 3 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Topic :: Multimedia :: Video Classifier:
 Topic :: Scientific/Engineering :: Information Analysis Classifier: Topic ::
 Text Processing Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Pillow==10.1.0 Requires-Dist: numpy
+License-File: LICENSE Requires-Dist: Pillow==10.3.0 Requires-Dist: numpy
 Requires-Dist: matplotlib Requires-Dist: joblib Requires-Dist: tqdm #
-AnimatedWordCloud ver 1.0.8 **UNDER CONSTRUCTION** _[_h_t_t_p_s_:_/_/
-_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_7_a_0_3_2_5_2_f_7_7_e_7_a_f_4_6_d_c_0_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![Codacy
-Badge](https://app.codacy.com/project/badge/Grade/
-20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/gh/konbraphat51/
-AnimatedWordCloud/
+AnimatedWordCloud ver 1.0.9 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/
+_7_a_0_3_2_5_2_f_7_7_e_7_a_f_4_6_d_c_0_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![Codacy Badge](https://app.codacy.com/
+project/badge/Grade/20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/
+gh/konbraphat51/AnimatedWordCloud/
 dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![unit-test](https://github.com/konbraphat51/AnimatedWordCloud/actions/
 workflows/python-tester.yml/badge.svg?branch=main)](https://github.com/
 konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml)[![codecov]
 (https://codecov.io/gh/konbraphat51/AnimatedWordCloud/graph/
 badge.svg?token=4OOX0GSJDJ)](https://codecov.io/gh/konbraphat51/
 AnimatedWordCloud) AnimatedWordCloud animates the timelapse of your words
```

### Comparing `AnimatedWordCloudTimelapse-1.0.8/AnimatedWordCloudTimelapse.egg-info/SOURCES.txt` & `animatedwordcloudtimelapse-1.0.9/AnimatedWordCloudTimelapse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/LICENSE` & `animatedwordcloudtimelapse-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `AnimatedWordCloudTimelapse-1.0.8/PKG-INFO` & `animatedwordcloudtimelapse-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AnimatedWordCloudTimelapse
-Version: 1.0.8
+Version: 1.0.9
 Summary: Animate a timelapse of word cloud
 Home-page: https://github.com/konbraphat51/AnimatedWordCloud/tree/main
 Author: konbraphat51, superhotdogcat
 Author-email: konbraphat51@gmail.com, siromisochan@gmail.com
 License: MIT License
 Project-URL: GitHub Repository, https://github.com/konbraphat51/AnimatedWordCloud
 Keywords: NLP,World Cloud,Animation,Natural Language Processing,video,Visualization,Data Science
@@ -16,23 +16,21 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Multimedia :: Video
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: Pillow==10.1.0
+Requires-Dist: Pillow==10.3.0
 Requires-Dist: numpy
 Requires-Dist: matplotlib
 Requires-Dist: joblib
 Requires-Dist: tqdm
 
-# AnimatedWordCloud ver 1.0.8
-
-**UNDER CONSTRUCTION**
+# AnimatedWordCloud ver 1.0.9
 
 <a href="https://codeclimate.com/github/konbraphat51/AnimatedWordCloud/maintainability"><img src="https://api.codeclimate.com/v1/badges/7a03252f77e7af46dc0f/maintainability" /></a>
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/gh/konbraphat51/AnimatedWordCloud/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![unit-test](https://github.com/konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml/badge.svg?branch=main)](https://github.com/konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml)[![codecov](https://codecov.io/gh/konbraphat51/AnimatedWordCloud/graph/badge.svg?token=4OOX0GSJDJ)](https://codecov.io/gh/konbraphat51/AnimatedWordCloud)
 
 AnimatedWordCloud animates the timelapse of your words vector.
```

#### html2text {}

```diff
@@ -1,27 +1,26 @@
-Metadata-Version: 2.1 Name: AnimatedWordCloudTimelapse Version: 1.0.8 Summary:
+Metadata-Version: 2.1 Name: AnimatedWordCloudTimelapse Version: 1.0.9 Summary:
 Animate a timelapse of word cloud Home-page: https://github.com/konbraphat51/
 AnimatedWordCloud/tree/main Author: konbraphat51, superhotdogcat Author-email:
 konbraphat51@gmail.com, siromisochan@gmail.com License: MIT License Project-
 URL: GitHub Repository, https://github.com/konbraphat51/AnimatedWordCloud
 Keywords: NLP,World Cloud,Animation,Natural Language
 Processing,video,Visualization,Data Science Classifier: Development Status :: 1
 - Planning Classifier: Programming Language :: Python :: 3 Classifier: Intended
 Audience :: Developers Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: MIT License Classifier: Topic :: Multimedia :: Video Classifier:
 Topic :: Scientific/Engineering :: Information Analysis Classifier: Topic ::
 Text Processing Requires-Python: >=3.8 Description-Content-Type: text/markdown
-License-File: LICENSE Requires-Dist: Pillow==10.1.0 Requires-Dist: numpy
+License-File: LICENSE Requires-Dist: Pillow==10.3.0 Requires-Dist: numpy
 Requires-Dist: matplotlib Requires-Dist: joblib Requires-Dist: tqdm #
-AnimatedWordCloud ver 1.0.8 **UNDER CONSTRUCTION** _[_h_t_t_p_s_:_/_/
-_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_7_a_0_3_2_5_2_f_7_7_e_7_a_f_4_6_d_c_0_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![Codacy
-Badge](https://app.codacy.com/project/badge/Grade/
-20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/gh/konbraphat51/
-AnimatedWordCloud/
+AnimatedWordCloud ver 1.0.9 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/
+_7_a_0_3_2_5_2_f_7_7_e_7_a_f_4_6_d_c_0_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![Codacy Badge](https://app.codacy.com/
+project/badge/Grade/20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/
+gh/konbraphat51/AnimatedWordCloud/
 dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![unit-test](https://github.com/konbraphat51/AnimatedWordCloud/actions/
 workflows/python-tester.yml/badge.svg?branch=main)](https://github.com/
 konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml)[![codecov]
 (https://codecov.io/gh/konbraphat51/AnimatedWordCloud/graph/
 badge.svg?token=4OOX0GSJDJ)](https://codecov.io/gh/konbraphat51/
 AnimatedWordCloud) AnimatedWordCloud animates the timelapse of your words
```

### Comparing `AnimatedWordCloudTimelapse-1.0.8/README.md` & `animatedwordcloudtimelapse-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# AnimatedWordCloud ver 1.0.8
-
-**UNDER CONSTRUCTION**
+# AnimatedWordCloud ver 1.0.9
 
 <a href="https://codeclimate.com/github/konbraphat51/AnimatedWordCloud/maintainability"><img src="https://api.codeclimate.com/v1/badges/7a03252f77e7af46dc0f/maintainability" /></a>
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/gh/konbraphat51/AnimatedWordCloud/dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![unit-test](https://github.com/konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml/badge.svg?branch=main)](https://github.com/konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml)[![codecov](https://codecov.io/gh/konbraphat51/AnimatedWordCloud/graph/badge.svg?token=4OOX0GSJDJ)](https://codecov.io/gh/konbraphat51/AnimatedWordCloud)
 
 AnimatedWordCloud animates the timelapse of your words vector.
```

#### html2text {}

```diff
@@ -1,12 +1,11 @@
-# AnimatedWordCloud ver 1.0.8 **UNDER CONSTRUCTION** _[_h_t_t_p_s_:_/_/
-_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/_7_a_0_3_2_5_2_f_7_7_e_7_a_f_4_6_d_c_0_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![Codacy
-Badge](https://app.codacy.com/project/badge/Grade/
-20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/gh/konbraphat51/
-AnimatedWordCloud/
+# AnimatedWordCloud ver 1.0.9 _[_h_t_t_p_s_:_/_/_a_p_i_._c_o_d_e_c_l_i_m_a_t_e_._c_o_m_/_v_1_/_b_a_d_g_e_s_/
+_7_a_0_3_2_5_2_f_7_7_e_7_a_f_4_6_d_c_0_f_/_m_a_i_n_t_a_i_n_a_b_i_l_i_t_y_][![Codacy Badge](https://app.codacy.com/
+project/badge/Grade/20a71da0d9d841a2af236f6362a08ae7)](https://app.codacy.com/
+gh/konbraphat51/AnimatedWordCloud/
 dashboard?utm_source=gh&utm_medium=referral&utm_content=&utm_campaign=Badge_grade)
 [![unit-test](https://github.com/konbraphat51/AnimatedWordCloud/actions/
 workflows/python-tester.yml/badge.svg?branch=main)](https://github.com/
 konbraphat51/AnimatedWordCloud/actions/workflows/python-tester.yml)[![codecov]
 (https://codecov.io/gh/konbraphat51/AnimatedWordCloud/graph/
 badge.svg?token=4OOX0GSJDJ)](https://codecov.io/gh/konbraphat51/
 AnimatedWordCloud) AnimatedWordCloud animates the timelapse of your words
```

### Comparing `AnimatedWordCloudTimelapse-1.0.8/setup.py` & `animatedwordcloudtimelapse-1.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,28 +15,28 @@
 
 def requirements_from_file(file_name):
     return open(file_name).read().splitlines()
 
 
 setup(
     name="AnimatedWordCloudTimelapse",
-    version="1.0.8",
+    version="1.0.9",
     description="Animate a timelapse of word cloud",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="konbraphat51, superhotdogcat",
     author_email="konbraphat51@gmail.com, siromisochan@gmail.com",
     url="https://github.com/konbraphat51/AnimatedWordCloud/tree/main",
     packages=find_packages(exclude=["tests", "Docs"]),
     test_suite="tests",
     python_requires=">=3.8",
     package_data={"AnimatedWordCloud": ["Assets/**"]},
     include_package_data=True,
     install_requires=[
-        "Pillow==10.1.0",
+        "Pillow==10.3.0",
         "numpy",
         "matplotlib",
         "joblib",
         "tqdm",
     ],
     license="MIT License",
     zip_safe=False,
```

