# Comparing `tmp/Piscis-0.1.0.tar.gz` & `tmp/piscis-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Piscis-0.1.0.tar", last modified: Thu Feb  1 04:56:19 2024, max compression
+gzip compressed data, was "piscis-0.1.1.tar", last modified: Thu May  2 19:20:09 2024, max compression
```

## Comparing `Piscis-0.1.0.tar` & `piscis-0.1.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-02-01 04:56:19.943832 Piscis-0.1.0/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     1068 2023-08-17 16:54:34.000000 Piscis-0.1.0/LICENSE
--rw-r--r--   0 wniu      (1003) wniu      (1003)     3461 2024-02-01 04:56:19.943832 Piscis-0.1.0/PKG-INFO
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-02-01 04:56:19.943832 Piscis-0.1.0/Piscis.egg-info/
--rw-r--r--   0 wniu      (1003) wniu      (1003)     3461 2024-02-01 04:56:19.000000 Piscis-0.1.0/Piscis.egg-info/PKG-INFO
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      631 2024-02-01 04:56:19.000000 Piscis-0.1.0/Piscis.egg-info/SOURCES.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        1 2024-02-01 04:56:19.000000 Piscis-0.1.0/Piscis.egg-info/dependency_links.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)       48 2024-02-01 04:56:19.000000 Piscis-0.1.0/Piscis.egg-info/entry_points.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      102 2024-02-01 04:56:19.000000 Piscis-0.1.0/Piscis.egg-info/requires.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        7 2024-02-01 04:56:19.000000 Piscis-0.1.0/Piscis.egg-info/top_level.txt
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     2721 2023-11-14 17:43:48.000000 Piscis-0.1.0/README.md
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-02-01 04:56:19.943832 Piscis-0.1.0/piscis/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)       31 2023-09-28 16:19:28.000000 Piscis-0.1.0/piscis/__init__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     8154 2024-01-12 09:02:36.000000 Piscis-0.1.0/piscis/__main__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    19251 2024-01-26 05:59:50.000000 Piscis-0.1.0/piscis/core.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     8185 2023-11-14 17:48:53.000000 Piscis-0.1.0/piscis/data.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     2679 2023-10-21 05:34:40.000000 Piscis-0.1.0/piscis/downloads.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    20618 2024-01-12 03:19:45.000000 Piscis-0.1.0/piscis/losses.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     7164 2023-10-22 04:11:27.000000 Piscis-0.1.0/piscis/metrics.py
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-02-01 04:56:19.943832 Piscis-0.1.0/piscis/models/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-08-17 16:54:34.000000 Piscis-0.1.0/piscis/models/__init__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     3264 2023-11-14 16:39:21.000000 Piscis-0.1.0/piscis/models/spots.py
-drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-02-01 04:56:19.943832 Piscis-0.1.0/piscis/networks/
--rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-08-17 16:54:34.000000 Piscis-0.1.0/piscis/networks/__init__.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     7402 2023-10-09 18:04:26.000000 Piscis-0.1.0/piscis/networks/conv.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     9335 2023-10-09 17:59:22.000000 Piscis-0.1.0/piscis/networks/efficientnetv2.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    11811 2023-08-17 16:54:34.000000 Piscis-0.1.0/piscis/networks/efficientnetv2_defaults.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     9260 2023-11-22 06:28:34.000000 Piscis-0.1.0/piscis/networks/fpn.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)     2828 2023-09-26 19:44:48.000000 Piscis-0.1.0/piscis/optimizers.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      309 2023-09-28 16:24:14.000000 Piscis-0.1.0/piscis/paths.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    20729 2024-01-12 09:02:36.000000 Piscis-0.1.0/piscis/training.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    14889 2024-01-12 08:27:04.000000 Piscis-0.1.0/piscis/transforms.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)    21611 2023-11-12 05:01:04.000000 Piscis-0.1.0/piscis/utils.py
--rw-rw-r--   0 wniu      (1003) wniu      (1003)      941 2024-02-01 04:55:34.000000 Piscis-0.1.0/pyproject.toml
--rw-rw-r--   0 wniu      (1003) wniu      (1003)       38 2024-02-01 04:56:19.943832 Piscis-0.1.0/setup.cfg
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-05-02 19:20:09.874933 piscis-0.1.1/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     1068 2023-08-17 16:54:34.000000 piscis-0.1.1/LICENSE
+-rw-r--r--   0 wniu      (1003) wniu      (1003)     3461 2024-05-02 19:20:09.874933 piscis-0.1.1/PKG-INFO
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-05-02 19:20:09.874933 piscis-0.1.1/Piscis.egg-info/
+-rw-r--r--   0 wniu      (1003) wniu      (1003)     3461 2024-05-02 19:20:09.000000 piscis-0.1.1/Piscis.egg-info/PKG-INFO
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      631 2024-05-02 19:20:09.000000 piscis-0.1.1/Piscis.egg-info/SOURCES.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        1 2024-05-02 19:20:09.000000 piscis-0.1.1/Piscis.egg-info/dependency_links.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)       48 2024-05-02 19:20:09.000000 piscis-0.1.1/Piscis.egg-info/entry_points.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      102 2024-05-02 19:20:09.000000 piscis-0.1.1/Piscis.egg-info/requires.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        7 2024-05-02 19:20:09.000000 piscis-0.1.1/Piscis.egg-info/top_level.txt
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     2721 2023-11-14 17:43:48.000000 piscis-0.1.1/README.md
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-05-02 19:20:09.874933 piscis-0.1.1/piscis/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)       31 2023-09-28 16:19:28.000000 piscis-0.1.1/piscis/__init__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     8154 2024-01-12 09:02:36.000000 piscis-0.1.1/piscis/__main__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    19103 2024-04-04 06:28:12.000000 piscis-0.1.1/piscis/core.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     8186 2024-04-10 04:44:37.000000 piscis-0.1.1/piscis/data.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     2679 2023-10-21 05:34:40.000000 piscis-0.1.1/piscis/downloads.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    20618 2024-01-12 03:19:45.000000 piscis-0.1.1/piscis/losses.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     7164 2023-10-22 04:11:27.000000 piscis-0.1.1/piscis/metrics.py
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-05-02 19:20:09.874933 piscis-0.1.1/piscis/models/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-08-17 16:54:34.000000 piscis-0.1.1/piscis/models/__init__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     3264 2023-11-14 16:39:21.000000 piscis-0.1.1/piscis/models/spots.py
+drwxrwxr-x   0 wniu      (1003) wniu      (1003)        0 2024-05-02 19:20:09.874933 piscis-0.1.1/piscis/networks/
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)        0 2023-08-17 16:54:34.000000 piscis-0.1.1/piscis/networks/__init__.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     7402 2023-10-09 18:04:26.000000 piscis-0.1.1/piscis/networks/conv.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     9335 2023-10-09 17:59:22.000000 piscis-0.1.1/piscis/networks/efficientnetv2.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    11811 2023-08-17 16:54:34.000000 piscis-0.1.1/piscis/networks/efficientnetv2_defaults.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     9260 2023-11-22 06:28:34.000000 piscis-0.1.1/piscis/networks/fpn.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)     2816 2024-03-31 15:10:55.000000 piscis-0.1.1/piscis/optimizers.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      309 2023-09-28 16:24:14.000000 piscis-0.1.1/piscis/paths.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    21503 2024-05-01 20:38:41.000000 piscis-0.1.1/piscis/training.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    14889 2024-01-12 08:27:04.000000 piscis-0.1.1/piscis/transforms.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)    21611 2023-11-12 05:01:04.000000 piscis-0.1.1/piscis/utils.py
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)      941 2024-05-02 17:15:20.000000 piscis-0.1.1/pyproject.toml
+-rw-rw-r--   0 wniu      (1003) wniu      (1003)       38 2024-05-02 19:20:09.874933 piscis-0.1.1/setup.cfg
```

### Comparing `Piscis-0.1.0/LICENSE` & `piscis-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/PKG-INFO` & `piscis-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Piscis
-Version: 0.1.0
+Version: 0.1.1
 Summary: An automatic deep learning algorithm for spot detection in fluorescence microscopy images.
 Author: William Niu
 Author-email: wniu721@gmail.com
 Keywords: machine learning,deep learning,spot detection,fluorescence microscopy
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: <4,>=3.7
```

### Comparing `Piscis-0.1.0/Piscis.egg-info/PKG-INFO` & `piscis-0.1.1/Piscis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Piscis
-Version: 0.1.0
+Version: 0.1.1
 Summary: An automatic deep learning algorithm for spot detection in fluorescence microscopy images.
 Author: William Niu
 Author-email: wniu721@gmail.com
 Keywords: machine learning,deep learning,spot detection,fluorescence microscopy
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: <4,>=3.7
```

### Comparing `Piscis-0.1.0/Piscis.egg-info/SOURCES.txt` & `piscis-0.1.1/Piscis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/README.md` & `piscis-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/__main__.py` & `piscis-0.1.1/piscis/__main__.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/core.py` & `piscis-0.1.1/piscis/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,39 +46,35 @@
         Compiled model apply function.
     """
 
     def __init__(
             self,
             model_name: str = '20230905',
             batch_size: int = 4,
-            cache: bool = True,
             input_size: Optional[Tuple[int, int]] = None
     ) -> None:
 
         """Initialize a Piscis object and compile the model.
 
         Parameters
         ----------
         model_name : str, optional
             Model name. Default is '20230905'.
         batch_size : int, optional
             Batch size for the CNN. Default is 4.
-        cache : bool, optional
-            Whether to use compilation cache. Default is True.
         input_size : Optional[Tuple[int, int]], optional
             Input size for the CNN. If None, it is obtained from the model dictionary. Default is None.
         """
 
         # Set the batch size to 1 if running on CPU.
         if xla_bridge.get_backend().platform == 'cpu':
             batch_size = 1
 
-        # Initialize the compilation cache.
-        if cache:
-            compilation_cache.initialize_cache(CACHE_DIR)
+        # Set the compilation cache directory.
+        compilation_cache.set_cache_dir(CACHE_DIR)
 
         # Load the model.
         self.model_name = model_name
         self.batch_size = batch_size
         model_path = MODELS_DIR / model_name
         if not model_path.is_file():
             download_pretrained_model(model_name)
```

### Comparing `Piscis-0.1.0/piscis/data.py` & `piscis-0.1.1/piscis/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     # Create a DeepTile object and get tiles.
     images = np.stack(images)
     dt = deeptile.load(images)
     tiles1 = dt.get_tiles(tile_size, (0, 0))
     tiles2 = tiles1.import_data(coords, 'coords')
     nonempty_tiles = [(image.compute(), coord)
                       for tile1, tile2 in zip(tiles1[tiles1.nonempty_indices], tiles2[tiles2.nonempty_indices])
-                      for image, coord in zip(tile1, tile2) if len(coord) > min_spots]
+                      for image, coord in zip(tile1, tile2) if len(coord) >= min_spots]
     tiled_images_list, tiled_coords_list = zip(*nonempty_tiles)
     tiled_images = np.empty(len(tiled_images_list), dtype=object)
     tiled_coords = np.empty(len(tiled_coords_list), dtype=object)
     tiled_images[:] = tiled_images_list
     tiled_coords[:] = tiled_coords_list
 
     # Randomly shuffle the tiles.
```

### Comparing `Piscis-0.1.0/piscis/downloads.py` & `piscis-0.1.1/piscis/downloads.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/losses.py` & `piscis-0.1.1/piscis/losses.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/metrics.py` & `piscis-0.1.1/piscis/metrics.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/models/spots.py` & `piscis-0.1.1/piscis/models/spots.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/networks/conv.py` & `piscis-0.1.1/piscis/networks/conv.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/networks/efficientnetv2.py` & `piscis-0.1.1/piscis/networks/efficientnetv2.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/networks/efficientnetv2_defaults.py` & `piscis-0.1.1/piscis/networks/efficientnetv2_defaults.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/networks/fpn.py` & `piscis-0.1.1/piscis/networks/fpn.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/optimizers.py` & `piscis-0.1.1/piscis/optimizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,11 +55,11 @@
             optax.trace(
                 decay=momentum, nesterov=nesterov, accumulator_dtype=accumulator_dtype
             )
             if momentum is not None
             else optax.identity()
         ),
         optax.add_decayed_weights(weight_decay, mask),
-        optax._src.alias._scale_by_learning_rate(learning_rate),
+        optax.scale_by_learning_rate(learning_rate),
     )
 
     return tx
```

### Comparing `Piscis-0.1.0/piscis/training.py` & `piscis-0.1.1/piscis/training.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 import optax
-import orbax.checkpoint
+import orbax.checkpoint as ocp
 
 from abc import ABC
 from flax import serialization
-from flax.core import frozen_dict
-from flax.training import orbax_utils, train_state
+from flax.training import train_state
 from functools import partial
 from jax import jit, random, value_and_grad
+from jax._src import compilation_cache
 from tqdm.auto import tqdm
 from typing import Any, Dict, List, Optional, Tuple
 
 from piscis.data import load_datasets, transform_batch, transform_subdataset
 from piscis.losses import (dice_loss, masked_l2_loss, smoothf1_loss, weighted_bce_loss, weighted_binary_focal_loss,
                            wrap_loss_fn)
 from piscis.models.spots import round_input_size, SpotsModel
 from piscis.optimizers import sgdw
-from piscis.paths import CHECKPOINTS_DIR, MODELS_DIR
+from piscis.paths import CACHE_DIR, CHECKPOINTS_DIR, MODELS_DIR
 
 
 class TrainState(train_state.TrainState, ABC):
 
     """TrainState class used to store the current state of the model during training.
     Inherits from the train_state.TrainState class provided by Flax and adds additional attributes.
 
@@ -37,14 +37,15 @@
     """
 
     batch_stats: Any
     key: Any
     epoch: Any
 
 
+@partial(jit, static_argnums=(1, 2, 3))
 def create_train_state(
         key: jax.Array,
         input_size: Tuple[int, int],
         dropout_rate: float,
         tx: optax.GradientTransformation,
         variables: Optional[Dict] = None
 ) -> TrainState:
@@ -75,16 +76,14 @@
 
     # Initialize the model.
     model = SpotsModel(dropout_rate=dropout_rate)
 
     # Initialize parameters.
     if variables is None:
         variables = model.init(subkey, np.ones((1, *input_size, 1)), train=False)
-    else:
-        variables = frozen_dict.freeze(variables)
 
     # Create a TrainState object.
     state = TrainState.create(
         apply_fn=model.apply,
         params=variables['params'],
         tx=tx,
         batch_stats=variables['batch_stats'],
@@ -310,23 +309,30 @@
     key = random.fold_in(state.key, state.epoch)
     subkeys = random.split(key, 3)
     train_ds = transform_subdataset(dataset['train'], input_size, key=subkeys[0])
     valid_ds = dataset['valid']
 
     train_ds_size = len(train_ds['images'])
     valid_ds_size = len(valid_ds['images'])
-    n_steps = train_ds_size // batch_size
+    small_train_ds = train_ds_size < batch_size
+    if small_train_ds:
+        n_steps = 1
+    else:
+        n_steps = train_ds_size // batch_size
 
     # Initialize the progress bar.
     pbar = tqdm(total=n_steps)
 
     # Shuffle the training set.
-    perms = random.permutation(subkeys[1], train_ds_size)
-    perms = perms[:n_steps * batch_size]
-    perms = perms.reshape((n_steps, batch_size))
+    if small_train_ds:
+        perms = random.randint(subkeys[1], (n_steps, batch_size), 0, train_ds_size)
+    else:
+        perms = random.permutation(subkeys[1], train_ds_size)
+        perms = perms[:n_steps * batch_size]
+        perms = perms.reshape((n_steps, batch_size))
 
     batch_metrics = []
     epoch_metrics = {}
     summary = None
     for perm in perms:
 
         # Extract and transform the current training batch.
@@ -341,84 +347,93 @@
         # Compute mean training metrics across each batch in epoch.
         epoch_metrics = {
             k: np.mean([metrics[k] for metrics in batch_metrics]).astype(float)
             for k in batch_metrics[0]}
         epoch_metrics['n_steps'] = n_steps
 
         # Update the progress bar.
-        summary = f'''(train) loss: {epoch_metrics['loss']:> 6.4f}, 
-                      {', '.join([f'{k}: {epoch_metrics[k]:> 6.4f}' for k in loss_weights])}'''
+        summary = (
+            f'''(train) loss: {epoch_metrics['loss']:> 6.4f}, '''
+            f'''{', '.join([f'{k}: {epoch_metrics[k]:> 6.4f}' for k in loss_weights])}'''
+        )
         pbar.update(1)
         pbar.set_postfix_str(summary)
 
-    val_batch_metrics = []
-    val_epoch_metrics = []
-    for i in range(valid_ds_size):
-
-        # Extract and transform the current validation batch.
-        val_batch = {k: v[i:i + 1] for k, v in valid_ds.items()}
-        val_batch = transform_batch(val_batch, dilation_iterations, coords_max_length)
-
-        # Compute and update validation metrics.
-        _, (val_metrics, _) = loss_fn(state.params, state, val_batch, None,
-                                      dilation_iterations, max_distance, loss_weights, train=False)
-        val_metrics = {f'val_{k}': float(v) for k, v in val_metrics.items()}
-        val_batch_metrics.append(val_metrics)
-
-        # Compute mean validation metrics.
-        val_epoch_metrics = {
-            k: np.mean([metrics[k] for metrics in val_batch_metrics]).astype(float)
-            for k in val_batch_metrics[0]}
+    if valid_ds_size:
+        val_batch_metrics = []
+        val_epoch_metrics = []
+        for i in range(valid_ds_size):
+
+            # Extract and transform the current validation batch.
+            val_batch = {k: v[i:i + 1] for k, v in valid_ds.items()}
+            val_batch = transform_batch(val_batch, dilation_iterations, coords_max_length)
+
+            # Compute and update validation metrics.
+            _, (val_metrics, _) = loss_fn(state.params, state, val_batch, None,
+                                          dilation_iterations, max_distance, loss_weights, train=False)
+            val_metrics = {f'val_{k}': float(v) for k, v in val_metrics.items()}
+            val_batch_metrics.append(val_metrics)
+
+            # Compute mean validation metrics.
+            val_epoch_metrics = {
+                k: np.mean([metrics[k] for metrics in val_batch_metrics]).astype(float)
+                for k in val_batch_metrics[0]}
+
+            # Update the progress bar.
+            val_summary = (
+                f'''(valid) loss: {val_epoch_metrics['val_loss']: > 6.4f}, '''
+                f'''{', '.join([f"val_{k}: {val_epoch_metrics[f'val_{k}']: > 6.4f}" for k in loss_weights])} | '''
+                f'''{summary}'''
+            )
+            pbar.set_postfix_str(val_summary)
 
-        # Update the progress bar.
-        val_summary = f'''(valid) loss: {val_epoch_metrics['val_loss']:> 6.4f}, 
-                          {', '.join([f"val_{k}: {val_epoch_metrics[f'val_{k}']:> 6.4f}" for k in loss_weights])} | 
-                          {summary}'''
-        pbar.set_postfix_str(val_summary)
+        epoch_metrics = epoch_metrics | val_epoch_metrics
 
     pbar.close()
 
-    # Compute mean training and validation metrics.
-    epoch_metrics = epoch_metrics | val_epoch_metrics
     epoch_metrics['learning_rate'] = epoch_learning_rate
 
     # Update the training state.
     state = state.replace(epoch=state.epoch + 1)
 
     return state, batch_metrics, epoch_metrics
 
 
 def train_model(
         model_name: str,
         dataset_path: str,
+        pretrained_model_name: Optional[str] = None,
         adjustment: Optional[str] = 'standardize',
         input_size: Tuple[int, int] = (256, 256),
         random_seed: int = 0,
         batch_size: int = 4,
         learning_rate: float = 0.2,
         weight_decay: float = 1e-4,
         dropout_rate: float = 0.2,
         epochs: int = 400,
         warmup_fraction: float = 0.05,
         decay_fraction: float = 0.5,
         decay_transitions: int = 10,
         decay_factor: float = 0.5,
         dilation_iterations: int = 1,
         max_distance: float = 3.0,
-        loss_weights: Optional[Dict[str, float]] = None
+        loss_weights: Optional[Dict[str, float]] = None,
+        save_checkpoints: bool = True
 ) -> None:
 
     """Train a SpotsModel.
 
     Parameters
     ----------
     model_name: str
         Name of a new or existing model.
     dataset_path : str
         Path to the directory containing training and validation datasets.
+    pretrained_model_name : Optional[str], optional
+        Name of a pretrained model to initialize the weights. Default is None.
     adjustment : Optional[str], optional
         Adjustment type applied to images. Supported types are 'normalize' and 'standardize'. Default is 'standardize'.
     input_size : Tuple[int, int], optional
         Size of the input images used for training. Default is (256, 256).
     random_seed : int, optional
         Random seed used for initialization and training. Default is 0.
     batch_size : int, optional
@@ -443,28 +458,34 @@
         Number of iterations to dilate ground truth labels to minimize class imbalance and misclassifications due to
         minor offsets. Default is 1.
     max_distance : float, optional
         Maximum distance for matching predicted and ground truth displacement vectors. Default is 3.0.
     loss_weights : Optional[Dict[str, float]], optional
         Weights for terms in the overall loss function. Supported terms are 'l2', 'bce', 'focal', 'dice', and
         'smoothf1'. If None, the loss weights {'l2': 0.25, 'smoothf1': 1.0} will be used. Default is None.
+    save_checkpoints : bool, optional
+        Whether to save checkpoints during training. Default is True.
 
     Raises
     ------
     ValueError
         If warmup_fraction + decay_fraction is greater than 1.
     """
 
     if warmup_fraction + decay_fraction > 1:
         raise ValueError("warmup_fraction + decay_fraction cannot be greater 1.")
 
+    # Set the compilation cache directory.
+    compilation_cache.set_cache_dir(CACHE_DIR)
+
     # Load datasets.
     print('Loading datasets...')
     dataset = load_datasets(dataset_path, adjustment, load_train=True, load_valid=True, load_test=False)
-    dataset['valid'] = transform_subdataset(dataset['valid'], input_size)
+    if len(dataset['valid']['images']):
+        dataset['valid'] = transform_subdataset(dataset['valid'], input_size)
     coords_max_length = max([len(coords) for coords in dataset['train']['coords']] +
                             [len(coords) for coords in dataset['valid']['coords']])
 
     # Round the input size.
     input_size = round_input_size(input_size)
 
     # Create the random key.
@@ -488,31 +509,31 @@
         loss_weights = {'l2': 0.25, 'smoothf1': 1.0}
 
     # Define directories for storing checkpoints and the model.
     checkpoint_path = CHECKPOINTS_DIR / model_name
     model_path = MODELS_DIR / model_name
 
     # Create a checkpoint manager.
-    mgr_options = orbax.checkpoint.CheckpointManagerOptions(max_to_keep=2)
-    checkpointers = {
-        'state': orbax.checkpoint.PyTreeCheckpointer(),
-        'batch_metrics_log': orbax.checkpoint.Checkpointer(orbax.checkpoint.JsonCheckpointHandler()),
-        'epoch_metrics_log': orbax.checkpoint.Checkpointer(orbax.checkpoint.JsonCheckpointHandler())
-    }
+    mgr_options = ocp.CheckpointManagerOptions(max_to_keep=2)
     checkpoint_path.mkdir(parents=True, exist_ok=True)
-    ckpt_mgr = orbax.checkpoint.CheckpointManager(
+    ckpt_mgr = ocp.CheckpointManager(
         directory=checkpoint_path,
-        checkpointers=checkpointers,
+        item_names=('state', 'batch_metrics_log', 'epoch_metrics_log'),
         options=mgr_options
     )
 
     # Load existing model weights.
-    if (next(checkpoint_path.iterdir(), None) is None) and model_path.is_file():
-        print(f'Loading existing model weights from {model_path}...')
-        with open(model_path, 'rb') as f_model:
+    if pretrained_model_name is None:
+        existing_model_path = model_path
+    else:
+        existing_model_path = MODELS_DIR / pretrained_model_name
+
+    if (next(checkpoint_path.iterdir(), None) is None) and existing_model_path.is_file():
+        print(f'Loading existing model weights from {existing_model_path}...')
+        with open(existing_model_path, 'rb') as f_model:
             variables = serialization.from_bytes(target=None, encoded_bytes=f_model.read())['variables']
     else:
         variables = None
 
     # Create a new training state.
     print('Creating new TrainState...')
     state = create_train_state(key, input_size, dropout_rate, tx, variables)
@@ -521,19 +542,21 @@
     batch_metrics_log = []
     epoch_metrics_log = []
 
     # Load the latest checkpoint.
     latest_epoch = ckpt_mgr.latest_step()
     if latest_epoch is not None:
         print(f'Loading latest checkpoint from {checkpoint_path}...')
-        restore_args = orbax_utils.restore_args_from_target(state, mesh=None)
         checkpoint = ckpt_mgr.restore(
             step=latest_epoch,
-            items={'state': state, 'batch_metrics_log': batch_metrics_log, 'epoch_metrics_log': epoch_metrics_log},
-            restore_kwargs={'state': {'restore_args': restore_args}}
+            args=ocp.args.Composite(
+                state=ocp.args.StandardRestore(state),
+                batch_metrics_log=ocp.args.JsonRestore(),
+                epoch_metrics_log=ocp.args.JsonRestore()
+            )
         )
         state = checkpoint['state']
         batch_metrics_log = checkpoint['batch_metrics_log']
         epoch_metrics_log = checkpoint['epoch_metrics_log']
 
     for epoch_learning_rate in learning_rate_schedule:
 
@@ -542,21 +565,25 @@
             train_epoch(state, dataset, input_size, batch_size, epoch_learning_rate,
                         dilation_iterations, max_distance, loss_weights, coords_max_length)
 
         # Update batch metrics and epoch metrics logs.
         batch_metrics_log += batch_metrics
         epoch_metrics_log += [epoch_metrics]
 
-        # Save a checkpoint.
-        save_args = orbax_utils.save_args_from_target(state)
-        ckpt_mgr.save(
-            step=state.epoch,
-            items={'state': state, 'batch_metrics_log': batch_metrics_log, 'epoch_metrics_log': epoch_metrics_log},
-            save_kwargs={'state': {'save_args': save_args}}
-        )
+        # Save a checkpoint if necessary.
+        if save_checkpoints:
+            ckpt_mgr.save(
+                step=state.epoch,
+                args=ocp.args.Composite(
+                    state=ocp.args.StandardSave(state),
+                    batch_metrics_log=ocp.args.JsonSave(batch_metrics_log),
+                    epoch_metrics_log=ocp.args.JsonSave(epoch_metrics_log)
+                )
+            )
+            ckpt_mgr.wait_until_finished()
 
     # Save the model.
     model_dict = {
         'variables': {
             'params': state.params,
             'batch_stats': state.batch_stats
         },
```

### Comparing `Piscis-0.1.0/piscis/transforms.py` & `piscis-0.1.1/piscis/transforms.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/piscis/utils.py` & `piscis-0.1.1/piscis/utils.py`

 * *Files identical despite different names*

### Comparing `Piscis-0.1.0/pyproject.toml` & `piscis-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = 'Piscis'
-version = '0.1.0'
+version = '0.1.1'
 description = "An automatic deep learning algorithm for spot detection in fluorescence microscopy images."
 readme = 'README.md'
 requires-python = '>=3.7, <4'
 authors = [
     {email = 'wniu721@gmail.com'},
     {name = 'William Niu'}
 ]
```

