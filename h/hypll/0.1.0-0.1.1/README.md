# Comparing `tmp/hypll-0.1.0.tar.gz` & `tmp/hypll-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypll-0.1.0.tar", last modified: Tue Sep  5 08:45:07 2023, max compression
+gzip compressed data, was "hypll-0.1.1.tar", last modified: Thu May  2 14:21:45 2024, max compression
```

## Comparing `hypll-0.1.0.tar` & `hypll-0.1.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.166798 hypll-0.1.0/
--rw-rw-r--   0 max       (1000) max       (1000)     1095 2023-06-07 10:59:16.000000 hypll-0.1.0/LICENSE
--rw-rw-r--   0 max       (1000) max       (1000)      168 2023-09-05 08:45:07.166798 hypll-0.1.0/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1779 2023-07-18 12:15:14.000000 hypll-0.1.0/README.md
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/manifolds/
--rw-rw-r--   0 max       (1000) max       (1000)       27 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/manifolds/base/
--rw-rw-r--   0 max       (1000) max       (1000)       31 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/base/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3198 2023-07-24 14:13:37.000000 hypll-0.1.0/hypll/manifolds/base/manifold.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/manifolds/euclidean/
--rw-rw-r--   0 max       (1000) max       (1000)       32 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/euclidean/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     8322 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/euclidean/manifold.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/manifolds/poincare_ball/
--rw-rw-r--   0 max       (1000) max       (1000)       68 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1343 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/curvature.py
--rw-rw-r--   0 max       (1000) max       (1000)    11930 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/manifold.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/manifolds/poincare_ball/math/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/math/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     5067 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/math/diffgeom.py
--rw-rw-r--   0 max       (1000) max       (1000)     2383 2023-09-05 08:44:51.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/math/linalg.py
--rw-rw-r--   0 max       (1000) max       (1000)    10548 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/manifolds/poincare_ball/math/stats.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll/nn/
--rw-rw-r--   0 max       (1000) max       (1000)      411 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/__init__.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.166798 hypll-0.1.0/hypll/nn/modules/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)      623 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/activation.py
--rw-rw-r--   0 max       (1000) max       (1000)     2828 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/batchnorm.py
--rw-rw-r--   0 max       (1000) max       (1000)     1335 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/change_manifold.py
--rw-rw-r--   0 max       (1000) max       (1000)      723 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/container.py
--rw-rw-r--   0 max       (1000) max       (1000)     4452 2023-07-18 12:15:14.000000 hypll-0.1.0/hypll/nn/modules/convolution.py
--rw-rw-r--   0 max       (1000) max       (1000)     1271 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/embedding.py
--rw-rw-r--   0 max       (1000) max       (1000)      691 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/flatten.py
--rw-rw-r--   0 max       (1000) max       (1000)     1037 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/fold.py
--rw-rw-r--   0 max       (1000) max       (1000)     1377 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/linear.py
--rw-rw-r--   0 max       (1000) max       (1000)     3869 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/nn/modules/pooling.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.166798 hypll-0.1.0/hypll/optim/
--rw-rw-r--   0 max       (1000) max       (1000)       64 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/optim/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     6572 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/optim/adam.py
--rw-rw-r--   0 max       (1000) max       (1000)     5125 2023-06-07 16:56:00.000000 hypll-0.1.0/hypll/optim/sgd.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.166798 hypll-0.1.0/hypll/tensors/
--rw-rw-r--   0 max       (1000) max       (1000)      136 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/tensors/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     3147 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/tensors/manifold_parameter.py
--rw-rw-r--   0 max       (1000) max       (1000)     7698 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/tensors/manifold_tensor.py
--rw-rw-r--   0 max       (1000) max       (1000)     5645 2023-09-04 12:35:55.000000 hypll-0.1.0/hypll/tensors/tangent_tensor.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.166798 hypll-0.1.0/hypll/utils/
--rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/utils/__init__.py
--rw-rw-r--   0 max       (1000) max       (1000)     1082 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/utils/layer_utils.py
--rw-rw-r--   0 max       (1000) max       (1000)      149 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/utils/math.py
--rw-rw-r--   0 max       (1000) max       (1000)     1762 2023-06-07 10:59:16.000000 hypll-0.1.0/hypll/utils/tensor_utils.py
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.162798 hypll-0.1.0/hypll.egg-info/
--rw-rw-r--   0 max       (1000) max       (1000)      168 2023-09-05 08:45:07.000000 hypll-0.1.0/hypll.egg-info/PKG-INFO
--rw-rw-r--   0 max       (1000) max       (1000)     1340 2023-09-05 08:45:07.000000 hypll-0.1.0/hypll.egg-info/SOURCES.txt
--rw-rw-r--   0 max       (1000) max       (1000)        1 2023-09-05 08:45:07.000000 hypll-0.1.0/hypll.egg-info/dependency_links.txt
--rw-rw-r--   0 max       (1000) max       (1000)      136 2023-09-05 08:45:07.000000 hypll-0.1.0/hypll.egg-info/requires.txt
--rw-rw-r--   0 max       (1000) max       (1000)        6 2023-09-05 08:45:07.000000 hypll-0.1.0/hypll.egg-info/top_level.txt
--rw-rw-r--   0 max       (1000) max       (1000)      583 2023-09-05 08:44:51.000000 hypll-0.1.0/pyproject.toml
--rw-rw-r--   0 max       (1000) max       (1000)       38 2023-09-05 08:45:07.166798 hypll-0.1.0/setup.cfg
-drwxrwxr-x   0 max       (1000) max       (1000)        0 2023-09-05 08:45:07.166798 hypll-0.1.0/tests/
--rw-rw-r--   0 max       (1000) max       (1000)     4146 2023-06-07 10:59:16.000000 hypll-0.1.0/tests/test_manifold_tensor.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/
+-rw-rw-r--   0 max       (1000) max       (1000)     1095 2023-06-07 10:59:16.000000 hypll-0.1.1/LICENSE
+-rw-r--r--   0 max       (1000) max       (1000)      652 2024-05-02 14:21:45.593118 hypll-0.1.1/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     1779 2023-07-18 12:15:14.000000 hypll-0.1.1/README.md
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.589118 hypll-0.1.1/hypll/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.589118 hypll-0.1.1/hypll/manifolds/
+-rw-rw-r--   0 max       (1000) max       (1000)       27 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/manifolds/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.589118 hypll-0.1.1/hypll/manifolds/base/
+-rw-rw-r--   0 max       (1000) max       (1000)       31 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/manifolds/base/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3547 2024-03-11 15:12:45.000000 hypll-0.1.1/hypll/manifolds/base/manifold.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.589118 hypll-0.1.1/hypll/manifolds/euclidean/
+-rw-rw-r--   0 max       (1000) max       (1000)       32 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/manifolds/euclidean/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     8878 2024-03-11 15:12:45.000000 hypll-0.1.1/hypll/manifolds/euclidean/manifold.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.589118 hypll-0.1.1/hypll/manifolds/poincare_ball/
+-rw-rw-r--   0 max       (1000) max       (1000)       68 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1343 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/curvature.py
+-rw-rw-r--   0 max       (1000) max       (1000)    13139 2024-03-11 15:12:45.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/manifold.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.589118 hypll-0.1.1/hypll/manifolds/poincare_ball/math/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/math/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5741 2023-09-21 08:55:51.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/math/diffgeom.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2383 2023-09-05 08:44:51.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/math/linalg.py
+-rw-rw-r--   0 max       (1000) max       (1000)    10548 2024-03-11 15:12:45.000000 hypll-0.1.1/hypll/manifolds/poincare_ball/math/stats.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/hypll/nn/
+-rw-rw-r--   0 max       (1000) max       (1000)      411 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/__init__.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/hypll/nn/modules/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)      623 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/activation.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2828 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/batchnorm.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1335 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/change_manifold.py
+-rw-rw-r--   0 max       (1000) max       (1000)      723 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/container.py
+-rw-rw-r--   0 max       (1000) max       (1000)     4452 2023-07-18 12:15:14.000000 hypll-0.1.1/hypll/nn/modules/convolution.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1271 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/embedding.py
+-rw-rw-r--   0 max       (1000) max       (1000)      691 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/flatten.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1037 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/fold.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1377 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/linear.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3869 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/nn/modules/pooling.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/hypll/optim/
+-rw-rw-r--   0 max       (1000) max       (1000)       64 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/optim/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     6572 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/optim/adam.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5125 2023-06-07 16:56:00.000000 hypll-0.1.1/hypll/optim/sgd.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/hypll/tensors/
+-rw-rw-r--   0 max       (1000) max       (1000)      136 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/tensors/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     3147 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/tensors/manifold_parameter.py
+-rw-rw-r--   0 max       (1000) max       (1000)     8419 2024-05-02 14:17:59.000000 hypll-0.1.1/hypll/tensors/manifold_tensor.py
+-rw-rw-r--   0 max       (1000) max       (1000)     5899 2023-09-21 08:55:51.000000 hypll-0.1.1/hypll/tensors/tangent_tensor.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/hypll/utils/
+-rw-rw-r--   0 max       (1000) max       (1000)        0 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/utils/__init__.py
+-rw-rw-r--   0 max       (1000) max       (1000)     1082 2023-06-07 10:59:16.000000 hypll-0.1.1/hypll/utils/layer_utils.py
+-rw-rw-r--   0 max       (1000) max       (1000)      532 2023-09-21 08:55:51.000000 hypll-0.1.1/hypll/utils/math.py
+-rw-rw-r--   0 max       (1000) max       (1000)     2403 2023-09-21 08:55:51.000000 hypll-0.1.1/hypll/utils/tensor_utils.py
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/hypll.egg-info/
+-rw-r--r--   0 max       (1000) max       (1000)      652 2024-05-02 14:21:45.000000 hypll-0.1.1/hypll.egg-info/PKG-INFO
+-rw-rw-r--   0 max       (1000) max       (1000)     1340 2024-05-02 14:21:45.000000 hypll-0.1.1/hypll.egg-info/SOURCES.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        1 2024-05-02 14:21:45.000000 hypll-0.1.1/hypll.egg-info/dependency_links.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      136 2024-05-02 14:21:45.000000 hypll-0.1.1/hypll.egg-info/requires.txt
+-rw-rw-r--   0 max       (1000) max       (1000)        6 2024-05-02 14:21:45.000000 hypll-0.1.1/hypll.egg-info/top_level.txt
+-rw-rw-r--   0 max       (1000) max       (1000)      583 2024-05-02 14:17:52.000000 hypll-0.1.1/pyproject.toml
+-rw-rw-r--   0 max       (1000) max       (1000)       38 2024-05-02 14:21:45.593118 hypll-0.1.1/setup.cfg
+drwxrwxr-x   0 max       (1000) max       (1000)        0 2024-05-02 14:21:45.593118 hypll-0.1.1/tests/
+-rw-rw-r--   0 max       (1000) max       (1000)     4353 2024-05-02 14:17:59.000000 hypll-0.1.1/tests/test_manifold_tensor.py
```

### Comparing `hypll-0.1.0/LICENSE` & `hypll-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/README.md` & `hypll-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/manifolds/base/manifold.py` & `hypll-0.1.1/hypll/manifolds/base/manifold.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, List, Optional, Tuple, Union
 
 from torch import Tensor
 from torch.nn import Module, Parameter
 from torch.nn.common_types import _size_2_t
 
 # TODO: find a less hacky solution for this
 if TYPE_CHECKING:
@@ -33,14 +33,18 @@
         raise NotImplementedError
 
     @abstractmethod
     def dist(self, x: ManifoldTensor, y: ManifoldTensor) -> Tensor:
         raise NotImplementedError
 
     @abstractmethod
+    def cdist(self, x: ManifoldTensor, y: ManifoldTensor) -> Tensor:
+        raise NotImplementedError
+
+    @abstractmethod
     def euc_to_tangent(self, x: ManifoldTensor, u: ManifoldTensor) -> TangentTensor:
         raise NotImplementedError
 
     @abstractmethod
     def hyperplane_dists(self, x: ManifoldTensor, z: ManifoldTensor, r: Optional[Tensor]) -> Tensor:
         raise NotImplementedError
 
@@ -100,7 +104,15 @@
         input: ManifoldTensor,
         kernel_size: _size_2_t,
         dilation: _size_2_t = 1,
         padding: _size_2_t = 0,
         stride: _size_2_t = 1,
     ) -> ManifoldTensor:
         raise NotImplementedError
+
+    @abstractmethod
+    def cat(
+        self,
+        manifold_tensors: Union[Tuple[ManifoldTensor, ...], List[ManifoldTensor]],
+        dim: int = 0,
+    ) -> ManifoldTensor:
+        raise NotImplementedError
```

### Comparing `hypll-0.1.0/hypll/manifolds/euclidean/manifold.py` & `hypll-0.1.1/hypll/manifolds/euclidean/manifold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from math import sqrt
-from typing import Optional, Union
+from typing import List, Optional, Tuple, Union
 
 import torch
 from torch import Tensor, broadcast_shapes, empty, matmul, var
 from torch.nn import Parameter
 from torch.nn.common_types import _size_2_t
 from torch.nn.functional import unfold
 from torch.nn.init import _calculate_fan_in_and_fan_out, kaiming_uniform_, uniform_
 
 from hypll.manifolds.base import Manifold
 from hypll.tensors import ManifoldParameter, ManifoldTensor, TangentTensor
 from hypll.utils.tensor_utils import (
     check_dims_with_broadcasting,
+    check_if_man_dims_match,
     check_tangent_tensor_positions,
 )
 
 
 class Euclidean(Manifold):
     def __init__(self):
         super(Euclidean, self).__init__()
@@ -216,7 +217,20 @@
         # Flatten the tensor and return the new instance.
         flattened = torch.flatten(
             input=x.tensor,
             start_dim=start_dim,
             end_dim=end_dim,
         )
         return ManifoldTensor(data=flattened, manifold=x.manifold, man_dim=man_dim)
+
+    def cdist(self, x: ManifoldTensor, y: ManifoldTensor) -> Tensor:
+        return torch.cdist(x.tensor, y.tensor)
+
+    def cat(
+        self,
+        manifold_tensors: Union[Tuple[ManifoldTensor, ...], List[ManifoldTensor]],
+        dim: int = 0,
+    ) -> ManifoldTensor:
+        check_if_man_dims_match(manifold_tensors)
+        cat = torch.cat([t.tensor for t in manifold_tensors], dim=dim)
+        man_dim = manifold_tensors[0].man_dim
+        return ManifoldTensor(data=cat, manifold=self, man_dim=man_dim)
```

### Comparing `hypll-0.1.0/hypll/manifolds/poincare_ball/curvature.py` & `hypll-0.1.1/hypll/manifolds/poincare_ball/curvature.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/manifolds/poincare_ball/manifold.py` & `hypll-0.1.1/hypll/manifolds/poincare_ball/manifold.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import functools
-from typing import Optional, Union
+from typing import List, Optional, Tuple, Union
 
 import torch
 from torch import Tensor, empty, eye, no_grad
 from torch.nn import Parameter
 from torch.nn.common_types import _size_2_t
 from torch.nn.functional import softplus, unfold
 from torch.nn.init import normal_, zeros_
@@ -11,18 +11,20 @@
 from hypll.manifolds.base import Manifold
 from hypll.manifolds.euclidean import Euclidean
 from hypll.manifolds.poincare_ball.curvature import Curvature
 from hypll.tensors import ManifoldParameter, ManifoldTensor, TangentTensor
 from hypll.utils.math import beta_func
 from hypll.utils.tensor_utils import (
     check_dims_with_broadcasting,
+    check_if_man_dims_match,
     check_tangent_tensor_positions,
 )
 
 from .math.diffgeom import (
+    cdist,
     dist,
     euc_to_tangent,
     expmap,
     expmap0,
     gyration,
     inner,
     logmap,
@@ -312,7 +314,33 @@
             flattened = torch.flatten(
                 input=x.tensor,
                 start_dim=start_dim,
                 end_dim=end_dim,
             )
             man_dim = x.man_dim if end_dim > x.man_dim else x.man_dim - len(dimensions_to_flatten)
             return ManifoldTensor(data=flattened, manifold=x.manifold, man_dim=man_dim)
+
+    def cdist(self, x: ManifoldTensor, y: ManifoldTensor) -> Tensor:
+        return cdist(x=x.tensor, y=y.tensor, c=self.c())
+
+    def cat(
+        self,
+        manifold_tensors: Union[Tuple[ManifoldTensor, ...], List[ManifoldTensor]],
+        dim: int = 0,
+    ) -> ManifoldTensor:
+        check_if_man_dims_match(manifold_tensors)
+        if dim == manifold_tensors[0].man_dim:
+            tangent_tensors = [self.logmap(None, t) for t in manifold_tensors]
+            ns = torch.tensor([t.shape[t.man_dim] for t in manifold_tensors])
+            n = ns.sum()
+            beta_ns = beta_func(ns / 2, 0.5)
+            beta_n = beta_func(n / 2, 0.5)
+            cat = torch.cat(
+                [(t.tensor * beta_n) / beta_n_i for (t, beta_n_i) in zip(tangent_tensors, beta_ns)],
+                dim=dim,
+            )
+            new_tensor = TangentTensor(data=cat, manifold=self, man_dim=dim)
+            return self.expmap(new_tensor)
+        else:
+            cat = torch.cat([t.tensor for t in manifold_tensors], dim=dim)
+            man_dim = manifold_tensors[0].man_dim
+            return ManifoldTensor(data=cat, manifold=self, man_dim=man_dim)
```

### Comparing `hypll-0.1.0/hypll/manifolds/poincare_ball/math/diffgeom.py` & `hypll-0.1.1/hypll/manifolds/poincare_ball/math/diffgeom.py`

 * *Files 15% similar despite different names*

```diff
@@ -144,7 +144,30 @@
 ) -> torch.Tensor:
     broadcasted_dim = max(x.dim(), u.dim())
     dim = dim if dim >= 0 else broadcasted_dim + dim
     lambda_x = 2 / (
         1 - c * x.pow(2).sum(dim=dim - broadcasted_dim + x.dim(), keepdim=True)
     ).clamp_min(1e-15)
     return u / lambda_x**2
+
+
+def cdist(
+    x: torch.Tensor,
+    y: torch.Tensor,
+    c: torch.Tensor,
+) -> torch.Tensor:
+    return 2 / c.sqrt() * (c.sqrt() * mobius_add_batch(-x, y, c).norm(dim=-1)).atanh()
+
+
+def mobius_add_batch(
+    x: torch.Tensor,
+    y: torch.Tensor,
+    c: torch.Tensor,
+):
+    xy = torch.einsum("bij,bkj->bik", (x, y))
+    x2 = x.pow(2).sum(dim=-1, keepdim=True)
+    y2 = y.pow(2).sum(dim=-1, keepdim=True)
+    num = 1 + 2 * c * xy + c * y2.permute(0, 2, 1)
+    num = num.unsqueeze(3) * x.unsqueeze(2)
+    num = num + (1 - c * x2).unsqueeze(3) * y.unsqueeze(1)
+    denom = 1 + 2 * c * xy + c**2 * x2 * y2.permute(0, 2, 1)
+    return num / denom.unsqueeze(3).clamp_min(1e-15)
```

### Comparing `hypll-0.1.0/hypll/manifolds/poincare_ball/math/linalg.py` & `hypll-0.1.1/hypll/manifolds/poincare_ball/math/linalg.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/manifolds/poincare_ball/math/stats.py` & `hypll-0.1.1/hypll/manifolds/poincare_ball/math/stats.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/activation.py` & `hypll-0.1.1/hypll/nn/modules/activation.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/batchnorm.py` & `hypll-0.1.1/hypll/nn/modules/batchnorm.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/change_manifold.py` & `hypll-0.1.1/hypll/nn/modules/change_manifold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/container.py` & `hypll-0.1.1/hypll/nn/modules/container.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/convolution.py` & `hypll-0.1.1/hypll/nn/modules/convolution.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/embedding.py` & `hypll-0.1.1/hypll/nn/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/flatten.py` & `hypll-0.1.1/hypll/nn/modules/flatten.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/fold.py` & `hypll-0.1.1/hypll/nn/modules/fold.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/linear.py` & `hypll-0.1.1/hypll/nn/modules/linear.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/nn/modules/pooling.py` & `hypll-0.1.1/hypll/nn/modules/pooling.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/optim/adam.py` & `hypll-0.1.1/hypll/optim/adam.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/optim/sgd.py` & `hypll-0.1.1/hypll/optim/sgd.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/tensors/manifold_parameter.py` & `hypll-0.1.1/hypll/tensors/manifold_parameter.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/tensors/manifold_tensor.py` & `hypll-0.1.1/hypll/tensors/manifold_tensor.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,19 @@
                     f"is not 0, but the manifold dimension is {self.man_dim}"
                 )
             new_tensor = self.tensor.__getitem__(*args)
             new_man_dim = self.man_dim + args[0].dim() - 1
             return ManifoldTensor(data=new_tensor, manifold=self.manifold, man_dim=new_man_dim)
 
         # Convert the args to a list and replace Ellipsis by the correct number of full slices
-        arg_list = list(args[0])
+        if isinstance(args[0], int):
+            arg_list = [args[0]]
+        else:
+            arg_list = list(args[0])
+
         if Ellipsis in arg_list:
             ell_id = arg_list.index(Ellipsis)
             colon_repeats = self.dim() - sum(1 for a in arg_list if a is not None) + 1
             arg_list[ell_id : ell_id + 1] = colon_repeats * [slice(None, None, None)]
 
         new_tensor = self.tensor.__getitem__(*args)
         output_man_dim = self.man_dim
@@ -101,14 +105,23 @@
                         "valid operation"
                     )
                 # If we get past the man_dim term, the output man_dim doesn't change anymore
                 break
 
         return ManifoldTensor(data=new_tensor, manifold=self.manifold, man_dim=output_man_dim)
 
+    def __hash__(self):
+        """Returns the Python unique identifier of the object.
+
+        Note: This is how PyTorch implements hash of tensors. See also:
+        https://github.com/pytorch/pytorch/issues/2569.
+
+        """
+        return id(self)
+
     def cpu(self) -> ManifoldTensor:
         """Returns a copy of this object with self.tensor in CPU memory."""
         new_tensor = self.tensor.cpu()
         return ManifoldTensor(data=new_tensor, manifold=self.manifold, man_dim=self.man_dim)
 
     def cuda(self, device=None) -> ManifoldTensor:
         """Returns a copy of this object with self.tensor in CUDA memory."""
@@ -192,7 +205,13 @@
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         # TODO: check if there are torch functions that should be allowed
         raise TypeError(
             f"Attempting to apply the torch function {func} on a ManifoldTensor. "
             f"Use ManifoldTensor.tensor as argument to {func} instead."
         )
+
+    def unsqueeze(self, dim: int) -> ManifoldTensor:
+        """Returns a new manifold tensor with a dimension of size one inserted at the specified position."""
+        new_tensor = self.tensor.unsqueeze(dim=dim)
+        new_man_dim = self.man_dim + (1 if dim <= self.man_dim else 0)
+        return ManifoldTensor(data=new_tensor, manifold=self.manifold, man_dim=new_man_dim)
```

### Comparing `hypll-0.1.0/hypll/tensors/tangent_tensor.py` & `hypll-0.1.1/hypll/tensors/tangent_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,23 @@
                 return torch_attribute
 
         else:
             raise AttributeError(
                 f"Neither {self.__class__.__name__}, nor torch.Tensor has attribute {name}"
             )
 
+    def __hash__(self):
+        """Returns the Python unique identifier of the object.
+
+        Note: This is how PyTorch implements hash of tensors. See also:
+        https://github.com/pytorch/pytorch/issues/2569.
+
+        """
+        return id(self)
+
     def cuda(self, device=None):
         new_tensor = self.tensor.cuda(device)
         new_manifold_points = self.manifold_points.cuda(device)
         return TangentTensor(
             data=new_tensor,
             manifold_points=new_manifold_points,
             manifold=self.manifold,
```

### Comparing `hypll-0.1.0/hypll/utils/layer_utils.py` & `hypll-0.1.1/hypll/utils/layer_utils.py`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/hypll/utils/tensor_utils.py` & `hypll-0.1.1/hypll/utils/tensor_utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import List, Tuple, Union
+
 from torch import broadcast_shapes, equal
 
 from hypll.tensors import ManifoldTensor, TangentTensor
 
 
 def check_dims_with_broadcasting(*args: ManifoldTensor) -> int:
     # Check if shapes can be broadcasted together
@@ -39,7 +41,26 @@
             mp.tensor.broadcast_to(broadcasted_shape) for mp in manifold_points
         ]
         for bmp in broadcasted_manifold_points[1:]:
             if not equal(broadcasted_manifold_points[0], bmp):
                 raise ValueError(
                     f"Tangent tensors are positioned at the different points on the manifold"
                 )
+
+
+def check_if_man_dims_match(
+    manifold_tensors: Union[Tuple[ManifoldTensor, ...], List[ManifoldTensor]]
+) -> None:
+    iterator = iter(manifold_tensors)
+
+    try:
+        first_item = next(iterator)
+    except StopIteration:
+        return
+
+    for i, x in enumerate(iterator):
+        if x.man_dim != first_item.man_dim:
+            raise ValueError(
+                f"Manifold dimensions of inputs do not match. "
+                f"Input at index [0] has manifold dimension {first_item.man_dim} "
+                f"but input at index [{i + 1}] has manifold dimension {x.man_dim}."
+            )
```

### Comparing `hypll-0.1.0/hypll.egg-info/SOURCES.txt` & `hypll-0.1.1/hypll.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hypll-0.1.0/pyproject.toml` & `hypll-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hypll"
 description = "A framework for hyperbolic learning in PyTorch"
-version = "0.1.0"
+version = "0.1.1"
 dependencies = [
     "torch",
 ]
 
 [project.optional-dependencies]
 dev = [
     "black",
```

### Comparing `hypll-0.1.0/tests/test_manifold_tensor.py` & `hypll-0.1.1/tests/test_manifold_tensor.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,14 +47,21 @@
 def test_slicing(manifold_tensor: ManifoldTensor):
     # First test slicing with the usual numpy slicing
     manifold_tensor = ManifoldTensor(
         data=torch.ones(2, 3, 4, 5, 6, 7, 8, 9),
         manifold=PoincareBall(Curvature()),
         man_dim=-2,
     )
+
+    # Single index
+    single_index = manifold_tensor[1]
+    assert list(single_index.size()) == [3, 4, 5, 6, 7, 8, 9]
+    assert single_index.man_dim == 5
+
+    # More complicated list of slicing arguments
     sliced_tensor = manifold_tensor[1, None, [0, 2], ..., None, 2:5, :, 1]
     # Explanation of the output size: the dimension of size 2 dissappears because of the integer
     # index. Then, a dim of size 1 is added by None. The size 3 dimension reduces to 2 because
     # of the list of indices. The Ellipsis skips the dimensions of sizes 4, 5 and 6. Then another
     # None leads to an insertion of a dimension of size 1. The dimension with size 7 is reduced
     # to 3 because of the 2:5 slice. The manifold dimension of size 8 is left alone and the last
     # dimension is removed because of an integer index.
```

