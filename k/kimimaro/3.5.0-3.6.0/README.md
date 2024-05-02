# Comparing `tmp/kimimaro-3.5.0.tar.gz` & `tmp/kimimaro-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kimimaro-3.5.0.tar", last modified: Thu Feb  8 18:34:41 2024, max compression
+gzip compressed data, was "kimimaro-3.6.0.tar", last modified: Thu May  2 18:00:57 2024, max compression
```

## Comparing `kimimaro-3.5.0.tar` & `kimimaro-3.6.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-08 18:34:41.373380 kimimaro-3.5.0/
--rw-r--r--   0 wms        (501) staff       (20)       88 2021-01-11 02:21:49.000000 kimimaro-3.5.0/AUTHORS
--rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-11 02:21:49.000000 kimimaro-3.5.0/LICENSE
--rw-r--r--   0 wms        (501) staff       (20)       39 2021-01-11 02:21:49.000000 kimimaro-3.5.0/MANIFEST.in
--rw-r--r--   0 wms        (501) staff       (20)    45218 2024-02-08 18:34:41.372988 kimimaro-3.5.0/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)    43393 2024-02-08 02:48:07.000000 kimimaro-3.5.0/README.md
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-08 18:34:41.346869 kimimaro-3.5.0/ext/
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-08 18:34:41.364745 kimimaro-3.5.0/ext/skeletontricks/
--rw-r--r--   0 wms        (501) staff       (20)    94949 2022-10-16 02:32:57.000000 kimimaro-3.5.0/ext/skeletontricks/robinhood.hpp
--rw-r--r--   0 wms        (501) staff       (20)  4101822 2024-02-08 02:40:31.000000 kimimaro-3.5.0/ext/skeletontricks/skeletontricks.cpp
--rw-r--r--   0 wms        (501) staff       (20)    12249 2023-01-29 09:55:10.000000 kimimaro-3.5.0/ext/skeletontricks/skeletontricks.hpp
--rw-r--r--   0 wms        (501) staff       (20)     3943 2022-10-16 02:33:33.000000 kimimaro-3.5.0/ext/skeletontricks/skeletontricks.pxd
--rw-r--r--   0 wms        (501) staff       (20)    26546 2024-01-23 06:25:47.000000 kimimaro-3.5.0/ext/skeletontricks/skeletontricks.pyx
--rw-r--r--   0 wms        (501) staff       (20)      518 2021-01-11 02:21:49.000000 kimimaro-3.5.0/ext/skeletontricks/test.cpp
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-08 18:34:41.370065 kimimaro-3.5.0/kimimaro/
--rw-r--r--   0 wms        (501) staff       (20)      906 2024-01-30 20:14:19.000000 kimimaro-3.5.0/kimimaro/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)    25910 2024-01-30 20:14:19.000000 kimimaro-3.5.0/kimimaro/intake.py
--rw-r--r--   0 wms        (501) staff       (20)    19101 2022-03-02 04:56:57.000000 kimimaro-3.5.0/kimimaro/postprocess.py
--rw-r--r--   0 wms        (501) staff       (20)    14248 2024-01-27 20:57:44.000000 kimimaro-3.5.0/kimimaro/trace.py
--rw-r--r--   0 wms        (501) staff       (20)     5082 2024-02-08 03:11:57.000000 kimimaro-3.5.0/kimimaro/utility.py
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-08 18:34:41.372401 kimimaro-3.5.0/kimimaro.egg-info/
--rw-r--r--   0 wms        (501) staff       (20)    45218 2024-02-08 18:34:41.000000 kimimaro-3.5.0/kimimaro.egg-info/PKG-INFO
--rw-r--r--   0 wms        (501) staff       (20)      675 2024-02-08 18:34:41.000000 kimimaro-3.5.0/kimimaro.egg-info/SOURCES.txt
--rw-r--r--   0 wms        (501) staff       (20)        1 2024-02-08 18:34:41.000000 kimimaro-3.5.0/kimimaro.egg-info/dependency_links.txt
--rw-r--r--   0 wms        (501) staff       (20)       47 2024-02-08 18:34:41.000000 kimimaro-3.5.0/kimimaro.egg-info/entry_points.txt
--rw-r--r--   0 wms        (501) staff       (20)      194 2024-02-08 18:34:41.000000 kimimaro-3.5.0/kimimaro.egg-info/requires.txt
--rw-r--r--   0 wms        (501) staff       (20)       22 2024-02-08 18:34:41.000000 kimimaro-3.5.0/kimimaro.egg-info/top_level.txt
-drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-02-08 18:34:41.371611 kimimaro-3.5.0/kimimaro_cli/
--rw-r--r--   0 wms        (501) staff       (20)     8072 2023-01-29 09:55:10.000000 kimimaro-3.5.0/kimimaro_cli/__init__.py
--rw-r--r--   0 wms        (501) staff       (20)       94 2023-12-19 05:31:04.000000 kimimaro-3.5.0/pyproject.toml
--rw-r--r--   0 wms        (501) staff       (20)       38 2024-02-08 18:34:41.373463 kimimaro-3.5.0/setup.cfg
--rw-r--r--   0 wms        (501) staff       (20)     2591 2024-02-08 02:47:10.000000 kimimaro-3.5.0/setup.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-02 18:00:57.723156 kimimaro-3.6.0/
+-rw-r--r--   0 wms        (501) staff       (20)       88 2021-01-11 02:21:49.000000 kimimaro-3.6.0/AUTHORS
+-rw-r--r--   0 wms        (501) staff       (20)    35149 2021-01-11 02:21:49.000000 kimimaro-3.6.0/LICENSE
+-rw-r--r--   0 wms        (501) staff       (20)       39 2021-01-11 02:21:49.000000 kimimaro-3.6.0/MANIFEST.in
+-rw-r--r--   0 wms        (501) staff       (20)    45784 2024-05-02 18:00:57.722806 kimimaro-3.6.0/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)    43959 2024-04-28 09:53:03.000000 kimimaro-3.6.0/README.md
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-02 18:00:57.693411 kimimaro-3.6.0/ext/
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-02 18:00:57.713779 kimimaro-3.6.0/ext/skeletontricks/
+-rw-r--r--   0 wms        (501) staff       (20)    94949 2022-10-16 02:32:57.000000 kimimaro-3.6.0/ext/skeletontricks/robinhood.hpp
+-rw-r--r--   0 wms        (501) staff       (20)  4102457 2024-04-06 06:50:50.000000 kimimaro-3.6.0/ext/skeletontricks/skeletontricks.cpp
+-rw-r--r--   0 wms        (501) staff       (20)    12249 2023-01-29 09:55:10.000000 kimimaro-3.6.0/ext/skeletontricks/skeletontricks.hpp
+-rw-r--r--   0 wms        (501) staff       (20)     3943 2022-10-16 02:33:33.000000 kimimaro-3.6.0/ext/skeletontricks/skeletontricks.pxd
+-rw-r--r--   0 wms        (501) staff       (20)    26546 2024-01-23 06:25:47.000000 kimimaro-3.6.0/ext/skeletontricks/skeletontricks.pyx
+-rw-r--r--   0 wms        (501) staff       (20)      518 2021-01-11 02:21:49.000000 kimimaro-3.6.0/ext/skeletontricks/test.cpp
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-02 18:00:57.719655 kimimaro-3.6.0/kimimaro/
+-rw-r--r--   0 wms        (501) staff       (20)      919 2024-04-28 09:53:03.000000 kimimaro-3.6.0/kimimaro/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)    25910 2024-04-06 00:15:42.000000 kimimaro-3.6.0/kimimaro/intake.py
+-rw-r--r--   0 wms        (501) staff       (20)    19101 2022-03-02 04:56:57.000000 kimimaro-3.6.0/kimimaro/postprocess.py
+-rw-r--r--   0 wms        (501) staff       (20)    14248 2024-01-27 20:57:44.000000 kimimaro-3.6.0/kimimaro/trace.py
+-rw-r--r--   0 wms        (501) staff       (20)     9294 2024-04-28 09:53:03.000000 kimimaro-3.6.0/kimimaro/utility.py
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-02 18:00:57.722118 kimimaro-3.6.0/kimimaro.egg-info/
+-rw-r--r--   0 wms        (501) staff       (20)    45784 2024-05-02 18:00:57.000000 kimimaro-3.6.0/kimimaro.egg-info/PKG-INFO
+-rw-r--r--   0 wms        (501) staff       (20)      675 2024-05-02 18:00:57.000000 kimimaro-3.6.0/kimimaro.egg-info/SOURCES.txt
+-rw-r--r--   0 wms        (501) staff       (20)        1 2024-05-02 18:00:57.000000 kimimaro-3.6.0/kimimaro.egg-info/dependency_links.txt
+-rw-r--r--   0 wms        (501) staff       (20)       47 2024-05-02 18:00:57.000000 kimimaro-3.6.0/kimimaro.egg-info/entry_points.txt
+-rw-r--r--   0 wms        (501) staff       (20)      194 2024-05-02 18:00:57.000000 kimimaro-3.6.0/kimimaro.egg-info/requires.txt
+-rw-r--r--   0 wms        (501) staff       (20)       22 2024-05-02 18:00:57.000000 kimimaro-3.6.0/kimimaro.egg-info/top_level.txt
+drwxr-xr-x   0 wms        (501) staff       (20)        0 2024-05-02 18:00:57.721722 kimimaro-3.6.0/kimimaro_cli/
+-rw-r--r--   0 wms        (501) staff       (20)     8072 2023-01-29 09:55:10.000000 kimimaro-3.6.0/kimimaro_cli/__init__.py
+-rw-r--r--   0 wms        (501) staff       (20)       94 2023-12-19 05:31:04.000000 kimimaro-3.6.0/pyproject.toml
+-rw-r--r--   0 wms        (501) staff       (20)       38 2024-05-02 18:00:57.723216 kimimaro-3.6.0/setup.cfg
+-rw-r--r--   0 wms        (501) staff       (20)     2591 2024-05-02 17:19:56.000000 kimimaro-3.6.0/setup.py
```

### Comparing `kimimaro-3.5.0/LICENSE` & `kimimaro-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/PKG-INFO` & `kimimaro-3.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimimaro
-Version: 3.5.0
+Version: 3.6.0
 Summary: Skeletonize densely labeled image volumes.
 Home-page: https://github.com/seung-lab/kimimaro/
 Author: William Silversmith, Alex Bae, Forrest Collman, Peter Li
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Keywords: volumetric-data numpy teasar skeletonization centerline medial-axis-transform centerline-extraction computer-vision-alogithms connectomics image-processing biomedical-image-processing voxel
 Classifier: Intended Audience :: Developers
@@ -166,26 +166,39 @@
 # like to assign (e.g. for pre-synaptic and post-synaptic) this finds the 
 # nearest voxel to the centroid for that label.
 # Input: { label: [ ((x,y,z), swc_label), ... ] }
 # Returns: { (x,y,z): swc_label, ... }
 extra_targets = kimimaro.synapses_to_targets(labels, synapses)
 
 
-# LISTING 3: Drawing a centerline between
+# LISTING 4: Drawing a centerline between
 #   preselected points on a binary image.
 #   This is a much simpler option for when
 #   you know exactly what you want, but may
 #   be less efficient for large scale procesing.
 
 skel = kimimaro.connect_points(
   labels == 67301298,
   start=(3, 215, 202), 
   end=(121, 426, 227),
   anisotropy=(32,32,40),
 )
+
+# LISTING 5: Using skeletons to oversegment existing
+#  segmentations for integration into proofreading systems 
+#  that on merging atomic labels. oversegmented_labels 
+#  is returned numbered from 1. skels is a copy returned 
+#  with the property skel.segments that associates a label
+#  to each vertex (labels will not be unique if downsampling 
+#  is used)
+oversegmented_labels, skels = kimimaro.oversegment(
+  labels, skels, 
+  anisotropy=(32,32,40), 
+  downsample=10,
+)
 ```
 
 `connectomics.npy` is multilabel connectomics data derived from pinky40, a 2018 experimental automated segmentation of ~1.5 million cubic micrometers of mouse visual cortex. It is an early predecessor to the now public pinky100_v185 segmentation that can be found at https://microns-explorer.org/phase1 You will need to run `lzma -d connectomics.npy.lzma` to obtain the 512x512x512 uint32 volume at 32x32x40 nm<sup>3</sup> resolution.  
 
 ### CLI Interface
 
 The CLI supports producing skeletons from a single image as SWCs and viewing the resulting SWC files one at a time. By default, the SWC files are written to `./kimimaro_out/$LABEL.swc`.
@@ -448,15 +461,16 @@
 
 Several classic algorithms had to be specially tuned to make this module possible.  
 
 1. [edt](https://github.com/seung-lab/euclidean-distance-transform-3d): A single pass, multi-label anisotropy supporting euclidean distance transform implementation. 
 2. [dijkstra3d](https://github.com/seung-lab/dijkstra3d): Dijkstra's shortest-path algorithm defined on 26-connected 3D images. This avoids the time cost of edge generation and wasted memory of a graph representation.
 3. [connected-components-3d](https://github.com/seung-lab/connected-components-3d): A connected components implementation defined on 26-connected 3D images with multiple labels.
 4. [fastremap](https://github.com/seung-lab/fastremap): Allows high speed renumbering of labels from 1 in a 3D array in order to reduce memory consumption caused by unnecessarily large 32 and 64-bit labels.
-5. [fill_voids](https://github.com/seung-lab/fill_voids): High speed binary_fill_holes.  
+5. [fill_voids](https://github.com/seung-lab/fill_voids): High speed binary_fill_holes.
+6. [xs3d](https://github.com/seung-lab/cross-section): Cross section analysis of 3D images.
 
 This module was originally designed to be used with CloudVolume and Igneous. 
 
 1. [CloudVolume](https://github.com/seung-lab/cloud-volume): Serverless client for reading and writing petascale chunked images of neural tissue, meshes, and skeletons.
 2. [Igneous](https://github.com/seung-lab/igneous/tree/master/igneous): Distributed computation for visualizing connectomics datasets.  
 
 Some of the TEASAR modifications used in this package were first demonstrated by Alex Bae.
```

### Comparing `kimimaro-3.5.0/README.md` & `kimimaro-3.6.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -123,26 +123,39 @@
 # like to assign (e.g. for pre-synaptic and post-synaptic) this finds the 
 # nearest voxel to the centroid for that label.
 # Input: { label: [ ((x,y,z), swc_label), ... ] }
 # Returns: { (x,y,z): swc_label, ... }
 extra_targets = kimimaro.synapses_to_targets(labels, synapses)
 
 
-# LISTING 3: Drawing a centerline between
+# LISTING 4: Drawing a centerline between
 #   preselected points on a binary image.
 #   This is a much simpler option for when
 #   you know exactly what you want, but may
 #   be less efficient for large scale procesing.
 
 skel = kimimaro.connect_points(
   labels == 67301298,
   start=(3, 215, 202), 
   end=(121, 426, 227),
   anisotropy=(32,32,40),
 )
+
+# LISTING 5: Using skeletons to oversegment existing
+#  segmentations for integration into proofreading systems 
+#  that on merging atomic labels. oversegmented_labels 
+#  is returned numbered from 1. skels is a copy returned 
+#  with the property skel.segments that associates a label
+#  to each vertex (labels will not be unique if downsampling 
+#  is used)
+oversegmented_labels, skels = kimimaro.oversegment(
+  labels, skels, 
+  anisotropy=(32,32,40), 
+  downsample=10,
+)
 ```
 
 `connectomics.npy` is multilabel connectomics data derived from pinky40, a 2018 experimental automated segmentation of ~1.5 million cubic micrometers of mouse visual cortex. It is an early predecessor to the now public pinky100_v185 segmentation that can be found at https://microns-explorer.org/phase1 You will need to run `lzma -d connectomics.npy.lzma` to obtain the 512x512x512 uint32 volume at 32x32x40 nm<sup>3</sup> resolution.  
 
 ### CLI Interface
 
 The CLI supports producing skeletons from a single image as SWCs and viewing the resulting SWC files one at a time. By default, the SWC files are written to `./kimimaro_out/$LABEL.swc`.
@@ -405,15 +418,16 @@
 
 Several classic algorithms had to be specially tuned to make this module possible.  
 
 1. [edt](https://github.com/seung-lab/euclidean-distance-transform-3d): A single pass, multi-label anisotropy supporting euclidean distance transform implementation. 
 2. [dijkstra3d](https://github.com/seung-lab/dijkstra3d): Dijkstra's shortest-path algorithm defined on 26-connected 3D images. This avoids the time cost of edge generation and wasted memory of a graph representation.
 3. [connected-components-3d](https://github.com/seung-lab/connected-components-3d): A connected components implementation defined on 26-connected 3D images with multiple labels.
 4. [fastremap](https://github.com/seung-lab/fastremap): Allows high speed renumbering of labels from 1 in a 3D array in order to reduce memory consumption caused by unnecessarily large 32 and 64-bit labels.
-5. [fill_voids](https://github.com/seung-lab/fill_voids): High speed binary_fill_holes.  
+5. [fill_voids](https://github.com/seung-lab/fill_voids): High speed binary_fill_holes.
+6. [xs3d](https://github.com/seung-lab/cross-section): Cross section analysis of 3D images.
 
 This module was originally designed to be used with CloudVolume and Igneous. 
 
 1. [CloudVolume](https://github.com/seung-lab/cloud-volume): Serverless client for reading and writing petascale chunked images of neural tissue, meshes, and skeletons.
 2. [Igneous](https://github.com/seung-lab/igneous/tree/master/igneous): Distributed computation for visualizing connectomics datasets.  
 
 Some of the TEASAR modifications used in this package were first demonstrated by Alex Bae.
```

### Comparing `kimimaro-3.5.0/ext/skeletontricks/robinhood.hpp` & `kimimaro-3.6.0/ext/skeletontricks/robinhood.hpp`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/ext/skeletontricks/skeletontricks.cpp` & `kimimaro-3.6.0/ext/skeletontricks/skeletontricks.cpp`

 * *Files 0% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-/* Generated by Cython 3.0.8 */
+/* Generated by Cython 3.0.10 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "ext/skeletontricks/robinhood.hpp",
             "ext/skeletontricks/skeletontricks.hpp"
         ],
         "extra_compile_args": [
             "-std=c++11",
             "-O3",
             "-ffast-math"
         ],
         "include_dirs": [
             "./ext/skeletontricks",
-            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/core/include"
+            "/private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/core/include"
         ],
         "language": "c++",
         "name": "kimimaro.skeletontricks",
         "sources": [
             "./ext/skeletontricks/skeletontricks.pyx"
         ]
     },
@@ -68,18 +68,18 @@
     #error Cython requires Python 2.7+ or Python 3.3+.
 #else
 #if defined(CYTHON_LIMITED_API) && CYTHON_LIMITED_API
 #define __PYX_EXTRA_ABI_MODULE_NAME "limited"
 #else
 #define __PYX_EXTRA_ABI_MODULE_NAME ""
 #endif
-#define CYTHON_ABI "3_0_8" __PYX_EXTRA_ABI_MODULE_NAME
+#define CYTHON_ABI "3_0_10" __PYX_EXTRA_ABI_MODULE_NAME
 #define __PYX_ABI_MODULE_NAME "_cython_" CYTHON_ABI
 #define __PYX_TYPE_MODULE_PREFIX __PYX_ABI_MODULE_NAME "."
-#define CYTHON_HEX_VERSION 0x030008F0
+#define CYTHON_HEX_VERSION 0x03000AF0
 #define CYTHON_FUTURE_DIVISION 1
 #include <stddef.h>
 #ifndef offsetof
   #define offsetof(type, member) ( (size_t) & ((type*)0) -> member )
 #endif
 #if !defined(_WIN32) && !defined(WIN32) && !defined(MS_WINDOWS)
   #ifndef __stdcall
@@ -163,14 +163,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(PYPY_VERSION)
   #define CYTHON_COMPILING_IN_PYPY 1
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #undef CYTHON_USE_TYPE_SLOTS
@@ -224,14 +226,16 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(CYTHON_LIMITED_API)
   #ifdef Py_LIMITED_API
     #undef __PYX_LIMITED_VERSION_HEX
     #define __PYX_LIMITED_VERSION_HEX Py_LIMITED_API
   #endif
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
@@ -285,60 +289,83 @@
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 0
   #endif
+  #undef CYTHON_USE_FREELISTS
+  #define CYTHON_USE_FREELISTS 0
 #elif defined(Py_GIL_DISABLED) || defined(Py_NOGIL)
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 0
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 1
   #ifndef CYTHON_USE_TYPE_SLOTS
     #define CYTHON_USE_TYPE_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_TYPE_SPECS
+    #define CYTHON_USE_TYPE_SPECS 0
+  #endif
   #undef CYTHON_USE_PYTYPE_LOOKUP
   #define CYTHON_USE_PYTYPE_LOOKUP 0
   #ifndef CYTHON_USE_ASYNC_SLOTS
     #define CYTHON_USE_ASYNC_SLOTS 1
   #endif
+  #ifndef CYTHON_USE_PYLONG_INTERNALS
+    #define CYTHON_USE_PYLONG_INTERNALS 0
+  #endif
   #undef CYTHON_USE_PYLIST_INTERNALS
   #define CYTHON_USE_PYLIST_INTERNALS 0
   #ifndef CYTHON_USE_UNICODE_INTERNALS
     #define CYTHON_USE_UNICODE_INTERNALS 1
   #endif
   #undef CYTHON_USE_UNICODE_WRITER
   #define CYTHON_USE_UNICODE_WRITER 0
-  #undef CYTHON_USE_PYLONG_INTERNALS
-  #define CYTHON_USE_PYLONG_INTERNALS 0
   #ifndef CYTHON_AVOID_BORROWED_REFS
     #define CYTHON_AVOID_BORROWED_REFS 0
   #endif
   #ifndef CYTHON_ASSUME_SAFE_MACROS
     #define CYTHON_ASSUME_SAFE_MACROS 1
   #endif
   #ifndef CYTHON_UNPACK_METHODS
     #define CYTHON_UNPACK_METHODS 1
   #endif
   #undef CYTHON_FAST_THREAD_STATE
   #define CYTHON_FAST_THREAD_STATE 0
+  #undef CYTHON_FAST_GIL
+  #define CYTHON_FAST_GIL 0
+  #ifndef CYTHON_METH_FASTCALL
+    #define CYTHON_METH_FASTCALL 1
+  #endif
   #undef CYTHON_FAST_PYCALL
   #define CYTHON_FAST_PYCALL 0
+  #ifndef CYTHON_PEP487_INIT_SUBCLASS
+    #define CYTHON_PEP487_INIT_SUBCLASS 1
+  #endif
   #ifndef CYTHON_PEP489_MULTI_PHASE_INIT
     #define CYTHON_PEP489_MULTI_PHASE_INIT 1
   #endif
+  #ifndef CYTHON_USE_MODULE_STATE
+    #define CYTHON_USE_MODULE_STATE 0
+  #endif
   #ifndef CYTHON_USE_TP_FINALIZE
     #define CYTHON_USE_TP_FINALIZE 1
   #endif
   #undef CYTHON_USE_DICT_VERSIONS
   #define CYTHON_USE_DICT_VERSIONS 0
   #undef CYTHON_USE_EXC_INFO_STACK
   #define CYTHON_USE_EXC_INFO_STACK 0
+  #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
+    #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
+  #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 0
+  #endif
 #else
   #define CYTHON_COMPILING_IN_PYPY 0
   #define CYTHON_COMPILING_IN_CPYTHON 1
   #define CYTHON_COMPILING_IN_LIMITED_API 0
   #define CYTHON_COMPILING_IN_GRAAL 0
   #define CYTHON_COMPILING_IN_NOGIL 0
   #ifndef CYTHON_USE_TYPE_SLOTS
@@ -421,14 +448,17 @@
     #define CYTHON_USE_EXC_INFO_STACK 0
   #elif !defined(CYTHON_USE_EXC_INFO_STACK)
     #define CYTHON_USE_EXC_INFO_STACK 1
   #endif
   #ifndef CYTHON_UPDATE_DESCRIPTOR_DOC
     #define CYTHON_UPDATE_DESCRIPTOR_DOC 1
   #endif
+  #ifndef CYTHON_USE_FREELISTS
+    #define CYTHON_USE_FREELISTS 1
+  #endif
 #endif
 #if !defined(CYTHON_FAST_PYCCALL)
 #define CYTHON_FAST_PYCCALL  (CYTHON_FAST_PYCALL && PY_VERSION_HEX >= 0x030600B1)
 #endif
 #if !defined(CYTHON_VECTORCALL)
 #define CYTHON_VECTORCALL  (CYTHON_FAST_PYCCALL && PY_VERSION_HEX >= 0x030800B1)
 #endif
@@ -780,16 +810,21 @@
   #ifndef METH_FASTCALL
      #define METH_FASTCALL 0x80
   #endif
   typedef PyObject *(*__Pyx_PyCFunctionFast) (PyObject *self, PyObject *const *args, Py_ssize_t nargs);
   typedef PyObject *(*__Pyx_PyCFunctionFastWithKeywords) (PyObject *self, PyObject *const *args,
                                                           Py_ssize_t nargs, PyObject *kwnames);
 #else
-  #define __Pyx_PyCFunctionFast _PyCFunctionFast
-  #define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #if PY_VERSION_HEX >= 0x030d00A4
+  #  define __Pyx_PyCFunctionFast PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords PyCFunctionFastWithKeywords
+  #else
+  #  define __Pyx_PyCFunctionFast _PyCFunctionFast
+  #  define __Pyx_PyCFunctionFastWithKeywords _PyCFunctionFastWithKeywords
+  #endif
 #endif
 #if CYTHON_METH_FASTCALL
   #define __Pyx_METH_FASTCALL METH_FASTCALL
   #define __Pyx_PyCFunction_FastCall __Pyx_PyCFunctionFast
   #define __Pyx_PyCFunction_FastCallWithKeywords __Pyx_PyCFunctionFastWithKeywords
 #else
   #define __Pyx_METH_FASTCALL METH_VARARGS
@@ -1133,15 +1168,15 @@
   #define __Pyx_PyList_SET_ITEM(o, i, v) PyList_SetItem(o, i, v)
   #define __Pyx_PyTuple_GET_SIZE(o) PyTuple_Size(o)
   #define __Pyx_PyList_GET_SIZE(o) PyList_Size(o)
   #define __Pyx_PySet_GET_SIZE(o) PySet_Size(o)
   #define __Pyx_PyBytes_GET_SIZE(o) PyBytes_Size(o)
   #define __Pyx_PyByteArray_GET_SIZE(o) PyByteArray_Size(o)
 #endif
-#if PY_VERSION_HEX >= 0x030d00A1
+#if __PYX_LIMITED_VERSION_HEX >= 0x030d00A1
   #define __Pyx_PyImport_AddModuleRef(name) PyImport_AddModuleRef(name)
 #else
   static CYTHON_INLINE PyObject *__Pyx_PyImport_AddModuleRef(const char *name) {
       PyObject *module = PyImport_AddModule(name);
       Py_XINCREF(module);
       return module;
   }
@@ -1220,15 +1255,15 @@
 #if defined(__CYGWIN__) && defined(_LDBL_EQ_DBL)
 #define __Pyx_truncl trunc
 #else
 #define __Pyx_truncl truncl
 #endif
 
 #define __PYX_MARK_ERR_POS(f_index, lineno) \
-    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__; (void)__pyx_clineno; }
+    { __pyx_filename = __pyx_f[f_index]; (void)__pyx_filename; __pyx_lineno = lineno; (void)__pyx_lineno; __pyx_clineno = __LINE__;  (void)__pyx_clineno; }
 #define __PYX_ERR(f_index, lineno, Ln_error) \
     { __PYX_MARK_ERR_POS(f_index, lineno) goto Ln_error; }
 
 #ifdef CYTHON_EXTERN_C
     #undef __PYX_EXTERN_C
     #define __PYX_EXTERN_C CYTHON_EXTERN_C
 #elif defined(__PYX_EXTERN_C)
@@ -1364,32 +1399,15 @@
 #define __Pyx_PyObject_AsSString(s)    ((const signed char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_AsUString(s)    ((const unsigned char*) __Pyx_PyObject_AsString(s))
 #define __Pyx_PyObject_FromCString(s)  __Pyx_PyObject_FromString((const char*)s)
 #define __Pyx_PyBytes_FromCString(s)   __Pyx_PyBytes_FromString((const char*)s)
 #define __Pyx_PyByteArray_FromCString(s)   __Pyx_PyByteArray_FromString((const char*)s)
 #define __Pyx_PyStr_FromCString(s)     __Pyx_PyStr_FromString((const char*)s)
 #define __Pyx_PyUnicode_FromCString(s) __Pyx_PyUnicode_FromString((const char*)s)
-#if CYTHON_COMPILING_IN_LIMITED_API
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const wchar_t *u)
-{
-    const wchar_t *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#else
-static CYTHON_INLINE size_t __Pyx_Py_UNICODE_strlen(const Py_UNICODE *u)
-{
-    const Py_UNICODE *u_end = u;
-    while (*u_end++) ;
-    return (size_t)(u_end - u - 1);
-}
-#endif
 #define __Pyx_PyUnicode_FromOrdinal(o)       PyUnicode_FromOrdinal((int)o)
-#define __Pyx_PyUnicode_FromUnicode(u)       PyUnicode_FromUnicode(u, __Pyx_Py_UNICODE_strlen(u))
-#define __Pyx_PyUnicode_FromUnicodeAndLength PyUnicode_FromUnicode
 #define __Pyx_PyUnicode_AsUnicode            PyUnicode_AsUnicode
 #define __Pyx_NewRef(obj) (Py_INCREF(obj), obj)
 #define __Pyx_Owned_Py_None(b) __Pyx_NewRef(Py_None)
 static CYTHON_INLINE PyObject * __Pyx_PyBool_FromLong(long b);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrue(PyObject*);
 static CYTHON_INLINE int __Pyx_PyObject_IsTrueAndDecref(PyObject*);
 static CYTHON_INLINE PyObject* __Pyx_PyNumber_IntOrLong(PyObject* x);
@@ -1725,195 +1743,195 @@
   Py_ssize_t strides[8];
   Py_ssize_t suboffsets[8];
 } __Pyx_memviewslice;
 #define __Pyx_MemoryView_Len(m)  (m.shape[0])
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":731
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":732
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":734
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":738
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":739
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":741
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":745
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":746
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":755
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":756
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":759
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":760
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":761
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":766
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":767
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":768
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1976,42 +1994,42 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":770
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":771
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":772
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":774
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3064,30 +3082,30 @@
 
 /* SetupReduce.proto */
 #if !CYTHON_COMPILING_IN_LIMITED_API
 static int __Pyx_setup_reduce(PyObject* type_obj);
 #endif
 
 /* TypeImport.proto */
-#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_8
-#define __PYX_HAVE_RT_ImportType_proto_3_0_8
+#ifndef __PYX_HAVE_RT_ImportType_proto_3_0_10
+#define __PYX_HAVE_RT_ImportType_proto_3_0_10
 #if defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L
 #include <stdalign.h>
 #endif
 #if (defined (__STDC_VERSION__) && __STDC_VERSION__ >= 201112L) || __cplusplus >= 201103L
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) alignof(s)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) alignof(s)
 #else
-#define __PYX_GET_STRUCT_ALIGNMENT_3_0_8(s) sizeof(void*)
+#define __PYX_GET_STRUCT_ALIGNMENT_3_0_10(s) sizeof(void*)
 #endif
-enum __Pyx_ImportType_CheckSize_3_0_8 {
-   __Pyx_ImportType_CheckSize_Error_3_0_8 = 0,
-   __Pyx_ImportType_CheckSize_Warn_3_0_8 = 1,
-   __Pyx_ImportType_CheckSize_Ignore_3_0_8 = 2
+enum __Pyx_ImportType_CheckSize_3_0_10 {
+   __Pyx_ImportType_CheckSize_Error_3_0_10 = 0,
+   __Pyx_ImportType_CheckSize_Warn_3_0_10 = 1,
+   __Pyx_ImportType_CheckSize_Ignore_3_0_10 = 2
 };
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size);
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject* module, const char *module_name, const char *class_name, size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size);
 #endif
 
 /* FetchSharedCythonModule.proto */
 static PyObject *__Pyx_FetchSharedCythonABIModule(void);
 
 /* FetchCommonType.proto */
 #if !CYTHON_USE_TYPE_SPECS
@@ -21074,70 +21092,70 @@
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4real_real(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":20
  *         @property
- *         cdef inline double real(self):
+ *         cdef inline double real(self) noexcept:
  *             return self.cval.real             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = __pyx_v_self->cval.real;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":19
  * 
  *         @property
- *         cdef inline double real(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double real(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.real
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
 static CYTHON_INLINE double __pyx_f_7cpython_7complex_7complex_4imag_imag(PyComplexObject *__pyx_v_self) {
   double __pyx_r;
 
   /* "cpython/complex.pxd":24
  *         @property
- *         cdef inline double imag(self):
+ *         cdef inline double imag(self) noexcept:
  *             return self.cval.imag             # <<<<<<<<<<<<<<
  * 
  *     # PyTypeObject PyComplex_Type
  */
   __pyx_r = __pyx_v_self->cval.imag;
   goto __pyx_L0;
 
   /* "cpython/complex.pxd":23
  * 
  *         @property
- *         cdef inline double imag(self):             # <<<<<<<<<<<<<<
+ *         cdef inline double imag(self) noexcept:             # <<<<<<<<<<<<<<
  *             return self.cval.imag
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
@@ -21955,15 +21973,15 @@
   }
 
   /* "array.pxd":170
  *     if self.ob_descr.typecode != other.ob_descr.typecode:
  *         PyErr_BadArgument()
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))             # <<<<<<<<<<<<<<
  * 
- * cdef inline void zero(array self):
+ * cdef inline void zero(array self) noexcept:
  */
   __pyx_t_2 = __pyx_f_7cpython_5array_extend_buffer(__pyx_v_self, __pyx_v_other->data.as_chars, Py_SIZE(((PyObject *)__pyx_v_other))); if (unlikely(__pyx_t_2 == ((int)-1))) __PYX_ERR(3, 170, __pyx_L1_error)
   __pyx_r = __pyx_t_2;
   goto __pyx_L0;
 
   /* "array.pxd":166
  *     return 0
@@ -21980,286 +21998,286 @@
   __pyx_L0:;
   return __pyx_r;
 }
 
 /* "array.pxd":172
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
  * 
- * cdef inline void zero(array self):             # <<<<<<<<<<<<<<
+ * cdef inline void zero(array self) noexcept:             # <<<<<<<<<<<<<<
  *     """ set all elements of array to zero. """
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
 static CYTHON_INLINE void __pyx_f_7cpython_5array_zero(arrayobject *__pyx_v_self) {
 
   /* "array.pxd":174
- * cdef inline void zero(array self):
+ * cdef inline void zero(array self) noexcept:
  *     """ set all elements of array to zero. """
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)             # <<<<<<<<<<<<<<
  */
   (void)(memset(__pyx_v_self->data.as_chars, 0, (Py_SIZE(((PyObject *)__pyx_v_self)) * __pyx_v_self->ob_descr->itemsize)));
 
   /* "array.pxd":172
  *     return extend_buffer(self, other.data.as_chars, Py_SIZE(other))
  * 
- * cdef inline void zero(array self):             # <<<<<<<<<<<<<<
+ * cdef inline void zero(array self) noexcept:             # <<<<<<<<<<<<<<
  *     """ set all elements of array to zero. """
  *     memset(self.data.as_chars, 0, Py_SIZE(self) * self.ob_descr.itemsize)
  */
 
   /* function exit code */
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -22268,29 +22286,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":776
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -22301,15 +22319,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -22318,29 +22336,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -22351,15 +22369,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -22368,29 +22386,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -22401,15 +22419,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -22418,29 +22436,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -22451,15 +22469,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -22468,29 +22486,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 789, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -22501,209 +22519,209 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":793
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":792
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":795
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":791
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":971
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":972
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":970
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":975
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":977
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":976
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":978
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":974
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -22719,15 +22737,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -22735,68 +22753,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":984
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(4, 984, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":985
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(4, 985, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__9, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 986, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(4, 986, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":983
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -22804,15 +22822,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":982
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -22827,15 +22845,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -22851,15 +22869,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -22867,68 +22885,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":990
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(4, 990, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":991
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(4, 991, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 992, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(4, 992, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":989
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -22936,15 +22954,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":988
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -22959,15 +22977,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -22983,15 +23001,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -22999,68 +23017,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":996
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(4, 996, __pyx_L3_error)
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":997
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(4, 997, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
+      /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":998
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__10, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(4, 998, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(4, 998, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":995
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -23068,15 +23086,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":994
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -23091,170 +23109,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1013
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1001
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1028
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1016
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1038
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1031
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1045
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1041
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+/* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1052
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":1048
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -81873,26 +81891,26 @@
  *         from pickle import PickleError as __pyx_PickleError
  *         raise __pyx_PickleError, "Incompatible checksums (0x%x vs (0x82a3537, 0x6ae9995, 0xb068931) = (name))" % __pyx_checksum
  */
   __pyx_tuple__8 = PyTuple_Pack(3, __pyx_int_136983863, __pyx_int_112105877, __pyx_int_184977713); if (unlikely(!__pyx_tuple__8)) __PYX_ERR(1, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__8);
   __Pyx_GIVEREF(__pyx_tuple__8);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":986
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__9 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__9)) __PYX_ERR(4, 986, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__9);
   __Pyx_GIVEREF(__pyx_tuple__9);
 
-  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-as5rs5ww/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../private/var/folders/w5/99_dvybs2zd1g4mrt3lhm1h40000gn/T/pip-build-env-0oj8lqxx/overlay/lib/python3.11/site-packages/numpy/__init__.cython-30.pxd":992
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__10 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__10)) __PYX_ERR(4, 992, __pyx_L1_error)
@@ -82552,53 +82570,53 @@
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("__Pyx_modinit_type_import_code", 0);
   /*--- Type import code ---*/
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
+  __pyx_ptype_7cpython_4type_type = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "type", 
   #if defined(PYPY_VERSION_NUM) && PYPY_VERSION_NUM < 0x050B0000
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #elif CYTHON_COMPILING_IN_LIMITED_API
-  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyTypeObject),
+  sizeof(PyTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyTypeObject),
   #else
-  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyHeapTypeObject),
+  sizeof(PyHeapTypeObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyHeapTypeObject),
   #endif
-  __Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
+  __Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4type_type) __PYX_ERR(5, 9, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
+  __pyx_ptype_7cpython_4bool_bool = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "bool", sizeof(PyBoolObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyBoolObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_4bool_bool) __PYX_ERR(6, 8, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule(__Pyx_BUILTIN_MODULE_NAME); if (unlikely(!__pyx_t_1)) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_8(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
+  __pyx_ptype_7cpython_7complex_complex = __Pyx_ImportType_3_0_10(__pyx_t_1, __Pyx_BUILTIN_MODULE_NAME, "complex", sizeof(PyComplexObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyComplexObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_7complex_complex) __PYX_ERR(7, 15, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("array"); if (unlikely(!__pyx_t_1)) __PYX_ERR(3, 69, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_8(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(3, 69, __pyx_L1_error)
+  __pyx_ptype_7cpython_5array_array = __Pyx_ImportType_3_0_10(__pyx_t_1, "array", "array", sizeof(arrayobject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(arrayobject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_7cpython_5array_array) __PYX_ERR(3, 69, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 202, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(4, 202, __pyx_L1_error)
-  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(4, 225, __pyx_L1_error)
-  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(4, 229, __pyx_L1_error)
-  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(4, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(4, 812, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_number) __PYX_ERR(4, 814, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(4, 816, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(4, 818, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(4, 820, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(4, 822, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(4, 824, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(4, 826, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(4, 828, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_8); if (!__pyx_ptype_5numpy_character) __PYX_ERR(4, 830, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_8(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_8(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_8); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(4, 868, __pyx_L1_error)
+  __pyx_ptype_5numpy_dtype = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(4, 202, __pyx_L1_error)
+  __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(4, 225, __pyx_L1_error)
+  __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(4, 229, __pyx_L1_error)
+  __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(4, 238, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(4, 812, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_number) __PYX_ERR(4, 814, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(4, 816, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(4, 818, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(4, 820, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(4, 822, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(4, 824, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(4, 826, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(4, 828, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyObject),__Pyx_ImportType_CheckSize_Warn_3_0_10); if (!__pyx_ptype_5numpy_character) __PYX_ERR(4, 830, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_3_0_10(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_3_0_10(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_3_0_10); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(4, 868, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_XDECREF(__pyx_t_1);
   __Pyx_RefNannyFinishContext();
   return -1;
@@ -88836,18 +88854,18 @@
     Py_XDECREF(setstate);
     Py_XDECREF(setstate_cython);
     return ret;
 }
 #endif
 
 /* TypeImport */
-  #ifndef __PYX_HAVE_RT_ImportType_3_0_8
-#define __PYX_HAVE_RT_ImportType_3_0_8
-static PyTypeObject *__Pyx_ImportType_3_0_8(PyObject *module, const char *module_name, const char *class_name,
-    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_8 check_size)
+  #ifndef __PYX_HAVE_RT_ImportType_3_0_10
+#define __PYX_HAVE_RT_ImportType_3_0_10
+static PyTypeObject *__Pyx_ImportType_3_0_10(PyObject *module, const char *module_name, const char *class_name,
+    size_t size, size_t alignment, enum __Pyx_ImportType_CheckSize_3_0_10 check_size)
 {
     PyObject *result = 0;
     char warning[200];
     Py_ssize_t basicsize;
     Py_ssize_t itemsize;
 #if CYTHON_COMPILING_IN_LIMITED_API
     PyObject *py_basicsize;
@@ -88893,23 +88911,23 @@
     if ((size_t)(basicsize + itemsize) < size) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize+itemsize);
         goto bad;
     }
-    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_8 &&
+    if (check_size == __Pyx_ImportType_CheckSize_Error_3_0_10 &&
             ((size_t)basicsize > size || (size_t)(basicsize + itemsize) < size)) {
         PyErr_Format(PyExc_ValueError,
             "%.200s.%.200s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd-%zd from PyObject",
             module_name, class_name, size, basicsize, basicsize+itemsize);
         goto bad;
     }
-    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_8 && (size_t)basicsize > size) {
+    else if (check_size == __Pyx_ImportType_CheckSize_Warn_3_0_10 && (size_t)basicsize > size) {
         PyOS_snprintf(warning, sizeof(warning),
             "%s.%s size changed, may indicate binary incompatibility. "
             "Expected %zd from C header, got %zd from PyObject",
             module_name, class_name, size, basicsize);
         if (PyErr_WarnEx(NULL, warning, 0) < 0) goto bad;
     }
     return (PyTypeObject *)result;
@@ -89901,15 +89919,15 @@
         break;
     case 0:
         self = ((PyCFunctionObject*)cyfunc)->m_self;
         break;
     default:
         return NULL;
     }
-    return ((_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
+    return ((__Pyx_PyCFunctionFastWithKeywords)(void(*)(void))def->ml_meth)(self, args, nargs, kwnames);
 }
 static PyObject * __Pyx_CyFunction_Vectorcall_FASTCALL_KEYWORDS_METHOD(PyObject *func, PyObject *const *args, size_t nargsf, PyObject *kwnames)
 {
     __pyx_CyFunctionObject *cyfunc = (__pyx_CyFunctionObject *)func;
     PyMethodDef* def = ((PyCFunctionObject*)cyfunc)->m_ml;
     PyTypeObject *cls = (PyTypeObject *) __Pyx_CyFunction_GetClassObj(cyfunc);
 #if CYTHON_BACKPORT_VECTORCALL
```

### Comparing `kimimaro-3.5.0/ext/skeletontricks/skeletontricks.hpp` & `kimimaro-3.6.0/ext/skeletontricks/skeletontricks.hpp`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/ext/skeletontricks/skeletontricks.pxd` & `kimimaro-3.6.0/ext/skeletontricks/skeletontricks.pxd`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/ext/skeletontricks/skeletontricks.pyx` & `kimimaro-3.6.0/ext/skeletontricks/skeletontricks.pyx`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/ext/skeletontricks/test.cpp` & `kimimaro-3.6.0/ext/skeletontricks/test.cpp`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/kimimaro/__init__.py` & `kimimaro-3.6.0/kimimaro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 
 You should have received a copy of the GNU General Public License
 along with Kimimaro.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 from .intake import skeletonize, DimensionError, synapses_to_targets, connect_points
 from .postprocess import postprocess, join_close_components
-from .utility import extract_skeleton_from_binary_image, cross_sectional_area
+from .utility import extract_skeleton_from_binary_image, cross_sectional_area, oversegment
```

### Comparing `kimimaro-3.5.0/kimimaro/intake.py` & `kimimaro-3.6.0/kimimaro/intake.py`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/kimimaro/postprocess.py` & `kimimaro-3.6.0/kimimaro/postprocess.py`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/kimimaro/trace.py` & `kimimaro-3.6.0/kimimaro/trace.py`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/kimimaro.egg-info/PKG-INFO` & `kimimaro-3.6.0/kimimaro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kimimaro
-Version: 3.5.0
+Version: 3.6.0
 Summary: Skeletonize densely labeled image volumes.
 Home-page: https://github.com/seung-lab/kimimaro/
 Author: William Silversmith, Alex Bae, Forrest Collman, Peter Li
 Author-email: ws9@princeton.edu
 License: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Keywords: volumetric-data numpy teasar skeletonization centerline medial-axis-transform centerline-extraction computer-vision-alogithms connectomics image-processing biomedical-image-processing voxel
 Classifier: Intended Audience :: Developers
@@ -166,26 +166,39 @@
 # like to assign (e.g. for pre-synaptic and post-synaptic) this finds the 
 # nearest voxel to the centroid for that label.
 # Input: { label: [ ((x,y,z), swc_label), ... ] }
 # Returns: { (x,y,z): swc_label, ... }
 extra_targets = kimimaro.synapses_to_targets(labels, synapses)
 
 
-# LISTING 3: Drawing a centerline between
+# LISTING 4: Drawing a centerline between
 #   preselected points on a binary image.
 #   This is a much simpler option for when
 #   you know exactly what you want, but may
 #   be less efficient for large scale procesing.
 
 skel = kimimaro.connect_points(
   labels == 67301298,
   start=(3, 215, 202), 
   end=(121, 426, 227),
   anisotropy=(32,32,40),
 )
+
+# LISTING 5: Using skeletons to oversegment existing
+#  segmentations for integration into proofreading systems 
+#  that on merging atomic labels. oversegmented_labels 
+#  is returned numbered from 1. skels is a copy returned 
+#  with the property skel.segments that associates a label
+#  to each vertex (labels will not be unique if downsampling 
+#  is used)
+oversegmented_labels, skels = kimimaro.oversegment(
+  labels, skels, 
+  anisotropy=(32,32,40), 
+  downsample=10,
+)
 ```
 
 `connectomics.npy` is multilabel connectomics data derived from pinky40, a 2018 experimental automated segmentation of ~1.5 million cubic micrometers of mouse visual cortex. It is an early predecessor to the now public pinky100_v185 segmentation that can be found at https://microns-explorer.org/phase1 You will need to run `lzma -d connectomics.npy.lzma` to obtain the 512x512x512 uint32 volume at 32x32x40 nm<sup>3</sup> resolution.  
 
 ### CLI Interface
 
 The CLI supports producing skeletons from a single image as SWCs and viewing the resulting SWC files one at a time. By default, the SWC files are written to `./kimimaro_out/$LABEL.swc`.
@@ -448,15 +461,16 @@
 
 Several classic algorithms had to be specially tuned to make this module possible.  
 
 1. [edt](https://github.com/seung-lab/euclidean-distance-transform-3d): A single pass, multi-label anisotropy supporting euclidean distance transform implementation. 
 2. [dijkstra3d](https://github.com/seung-lab/dijkstra3d): Dijkstra's shortest-path algorithm defined on 26-connected 3D images. This avoids the time cost of edge generation and wasted memory of a graph representation.
 3. [connected-components-3d](https://github.com/seung-lab/connected-components-3d): A connected components implementation defined on 26-connected 3D images with multiple labels.
 4. [fastremap](https://github.com/seung-lab/fastremap): Allows high speed renumbering of labels from 1 in a 3D array in order to reduce memory consumption caused by unnecessarily large 32 and 64-bit labels.
-5. [fill_voids](https://github.com/seung-lab/fill_voids): High speed binary_fill_holes.  
+5. [fill_voids](https://github.com/seung-lab/fill_voids): High speed binary_fill_holes.
+6. [xs3d](https://github.com/seung-lab/cross-section): Cross section analysis of 3D images.
 
 This module was originally designed to be used with CloudVolume and Igneous. 
 
 1. [CloudVolume](https://github.com/seung-lab/cloud-volume): Serverless client for reading and writing petascale chunked images of neural tissue, meshes, and skeletons.
 2. [Igneous](https://github.com/seung-lab/igneous/tree/master/igneous): Distributed computation for visualizing connectomics datasets.  
 
 Some of the TEASAR modifications used in this package were first demonstrated by Alex Bae.
```

### Comparing `kimimaro-3.5.0/kimimaro.egg-info/SOURCES.txt` & `kimimaro-3.6.0/kimimaro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/kimimaro_cli/__init__.py` & `kimimaro-3.6.0/kimimaro_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `kimimaro-3.5.0/setup.py` & `kimimaro-3.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     return f.read()
 
 # NOTE: If skeletontricks.cpp does not exist, you must run
 # cython -3 --cplus ./ext/skeletontricks/skeletontricks.pyx
 
 setuptools.setup(
   name="kimimaro",
-  version="3.5.0",
+  version="3.6.0",
   setup_requires=["numpy", "cython"],
   install_requires=[
     "click",
     "connected-components-3d>=1.5.0",
     "cloud-volume>=0.57.6",
     "dijkstra3d>=1.9.0",
     "fill-voids>=2.0.0",
```

