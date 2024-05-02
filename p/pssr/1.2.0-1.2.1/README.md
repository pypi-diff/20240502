# Comparing `tmp/pssr-1.2.0.tar.gz` & `tmp/pssr-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pssr-1.2.0.tar", max compression
+gzip compressed data, was "pssr-1.2.1.tar", max compression
```

## Comparing `pssr-1.2.0.tar` & `pssr-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.2.0/LICENSE
--rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.2.0/pssr/__init__.py
--rw-r--r--   0        0        0     4934 2024-05-01 03:00:25.746754 pssr-1.2.0/pssr/__main__.py
--rw-r--r--   0        0        0     4510 2024-04-26 04:19:02.573621 pssr-1.2.0/pssr/crappifiers.py
--rw-r--r--   0        0        0    32491 2024-05-01 00:39:30.861136 pssr-1.2.0/pssr/data.py
--rw-r--r--   0        0        0     2595 2024-04-27 20:27:44.061746 pssr-1.2.0/pssr/loss.py
--rw-r--r--   0        0        0       84 2024-05-01 02:54:05.539283 pssr-1.2.0/pssr/models/__init__.py
--rw-r--r--   0        0        0     4482 2024-04-30 02:37:25.112937 pssr-1.2.0/pssr/models/_blocks.py
--rw-r--r--   0        0        0     8121 2024-05-01 03:09:21.643561 pssr-1.2.0/pssr/models/_rdnet.py
--rw-r--r--   0        0        0     7617 2024-05-01 03:09:33.671764 pssr-1.2.0/pssr/models/rdresunet.py
--rw-r--r--   0        0        0     6955 2024-05-01 03:02:41.421290 pssr-1.2.0/pssr/models/resunet.py
--rw-r--r--   0        0        0    11090 2024-05-01 02:20:11.913442 pssr-1.2.0/pssr/predict.py
--rw-r--r--   0        0        0    12990 2024-04-27 20:27:14.761332 pssr-1.2.0/pssr/train.py
--rw-r--r--   0        0        0     1197 2024-05-01 03:14:42.305162 pssr-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     2691 1970-01-01 00:00:00.000000 pssr-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-16 23:21:24.739071 pssr-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-28 22:05:02.396223 pssr-1.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-03-07 21:39:47.125640 pssr-1.2.1/pssr/__init__.py
+-rw-r--r--   0        0        0     4934 2024-05-01 03:00:25.746754 pssr-1.2.1/pssr/__main__.py
+-rw-r--r--   0        0        0     4678 2024-05-02 02:57:56.749173 pssr-1.2.1/pssr/crappifiers.py
+-rw-r--r--   0        0        0    32730 2024-05-01 17:09:11.249481 pssr-1.2.1/pssr/data.py
+-rw-r--r--   0        0        0     2662 2024-05-02 00:48:45.425156 pssr-1.2.1/pssr/loss.py
+-rw-r--r--   0        0        0       84 2024-05-02 16:17:46.536616 pssr-1.2.1/pssr/models/__init__.py
+-rw-r--r--   0        0        0     4671 2024-05-02 16:04:40.293835 pssr-1.2.1/pssr/models/_blocks.py
+-rw-r--r--   0        0        0     8046 2024-05-01 15:20:32.105611 pssr-1.2.1/pssr/models/_rdnet.py
+-rw-r--r--   0        0        0     7617 2024-05-02 16:03:50.417239 pssr-1.2.1/pssr/models/rdresunet.py
+-rw-r--r--   0        0        0     6955 2024-05-01 03:02:41.421290 pssr-1.2.1/pssr/models/resunet.py
+-rw-r--r--   0        0        0    11138 2024-05-02 01:49:54.825731 pssr-1.2.1/pssr/predict.py
+-rw-r--r--   0        0        0    13435 2024-05-02 16:31:42.218290 pssr-1.2.1/pssr/train.py
+-rw-r--r--   0        0        0     1132 2024-05-02 16:16:58.819917 pssr-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2549 1970-01-01 00:00:00.000000 pssr-1.2.1/PKG-INFO
```

### Comparing `pssr-1.2.0/LICENSE` & `pssr-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pssr-1.2.0/README.md` & `pssr-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pssr-1.2.0/pssr/__main__.py` & `pssr-1.2.1/pssr/__main__.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.0/pssr/crappifiers.py` & `pssr-1.2.1/pssr/crappifiers.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,25 +19,30 @@
         """
         raise NotImplementedError('"crappify" method not implemented.')
     
     def __call__(self, image : np.ndarray):
         return self.crappify(image)
 
 class MultiCrappifier(Crappifier):
-    def __init__(self, crappifiers : list[Crappifier]):
+    def __init__(self, *args : Crappifier, clip : bool = True):
         r"""Chains multiple crappifiers sequentially for degrading low resolution images.
 
         Args:
-            crappifiers (list[Crappifier]) : Crappifiers to be applied in order from first to last.
+            args (Crappifier) : Crappifiers to be applied in order from first to last.
+
+            clip (bool) : Clip values to image range between each crappifier step. Default is True.
         """
-        self.crappifiers = list(crappifiers) if type(crappifiers) is not list else crappifiers
+        self.crappifiers = args
+        self.clip = clip
     
     def crappify(self, image : np.ndarray):
         for crappifier in self.crappifiers:
             image = crappifier.crappify(image)
+            if self.clip:
+                image = np.clip(image, 0, 255)
         return image
 
 class AdditiveGaussian(Crappifier):
     def __init__(self, intensity : float = 13, gain : float = 0, spread : float = 0):
         r"""Crappifier using additive Gaussian noise sampling (normally distributed noise). Adds additive Gaussian noise to a low resolution image.
 
         Approximates :class:`Poisson` noise at high samples.
@@ -69,15 +74,15 @@
             spread (float) : Standard deviation of crappifier intensity for training on a range of crappifications. Default is 0.
         """
         self.intensity = intensity
         self.gain = gain
         self.spread = spread
         
     def crappify(self, image : np.ndarray):
-        return self._interpolate(image, np.random.poisson(image)) + self.gain
+        return self._interpolate(image, np.random.poisson(np.clip(image, 0, np.inf))) + self.gain
     
     def _interpolate(self, x, y):
         intensity = max(np.random.normal(self.intensity, self.spread), 0) if self.spread > 0 else self.intensity
         return x * (1 - intensity) + y * intensity
     
 class SaltPepper(Crappifier):
     def __init__(self, intensity : float = 0.5, gain : float = 0, spread : float = 0):
@@ -92,8 +97,8 @@
         """
         self.intensity = intensity / 100
         self.gain = gain
         self.spread = spread
         
     def crappify(self, image : np.ndarray):
         intensity = max(np.random.normal(self.intensity, self.spread), 0) if self.spread > 0 else self.intensity
-        return random_noise(image/255, mode="s&p", amount=intensity) * 255 + self.gain
+        return random_noise(np.clip(image, 0, 255)/255, mode="s&p", amount=intensity) * 255 + self.gain
```

### Comparing `pssr-1.2.0/pssr/data.py` & `pssr-1.2.1/pssr/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
         if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
 
-        self.hr_files = sorted(glob.glob(Path(self.path, f"*.{extension}")))
+        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
         if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
 
         self.slices, max_size = [], 0
         for image_idx in range(len(self.hr_files)):
@@ -126,17 +126,18 @@
 
             transforms (list[nn.Module]) : Additional final data transforms to apply. Default is None.
         """
         super().__init__()
         self.path = Path(path) if type(path) is str else path
         if not self.path.exists(): raise FileNotFoundError(f'Path "{self.path}" does not exist.')
         
-        self.hr_files = sorted(glob.glob(Path(self.path, f"*.{extension}")))
+        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.path))
         if not len(self.hr_files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{self.path}".')
 
+        overlap = 0 if overlap is None else overlap
         if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
         self.stack = stack.upper()
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
         
         self.preload = _preload(preload, [self.path], [self.hr_files], self.mode, self.stack)
@@ -161,15 +162,15 @@
     
     def __getitem__(self, idx, pp=False):
         if idx >= len(self): raise IndexError(f"Tried to retrieve invalid image. Index {idx} is not less than {len(self)} total image frame slices.")
 
         is_val = idx in self.val_idx or pp
         image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
 
-        hr = _sliding_window(self.preload[image_idx] if self.preload else _load_sheet(self.path, self.hr_files[image_idx], self.stack, self.mode), self.hr_res, self.stride, self.n_frames[0], self.slices[image_idx], idx)
+        hr = _sliding_window(self.preload[image_idx] if self.preload else _load_sheet(self.path, self.hr_files[image_idx], self.stack, self.mode), self.hr_res, self.stride, self.n_frames[0] if self.n_frames is not None else None, self.slices[image_idx], idx)
 
         if self.is_lr:
             return _ready_lr(hr, self.hr_res, self.transforms)
 
         return _gen_pair(hr, self.hr_res, self.lr_scale, False if is_val else self.rotation, self.crappifier, self.transforms, self.n_frames)
     
     def __len__(self):
@@ -212,16 +213,16 @@
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         for path in [self.hr_path, self.lr_path]:
             if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
         if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using ImageDataset instead.", stacklevel=2)
 
-        self.hr_files = sorted(glob.glob(Path(self.hr_path, f"*.{extension}")))
-        self.lr_files = sorted(glob.glob(Path(self.lr_path, f"*.{extension}")))
+        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
+        self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
             if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
         if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
 
@@ -299,20 +300,21 @@
         super().__init__()
         self.hr_path = Path(hr_path) if type(hr_path) is str else hr_path
         self.lr_path = Path(lr_path) if type(lr_path) is str else lr_path
         for path in [self.hr_path, self.lr_path]:
             if not path.exists(): raise FileNotFoundError(f'Path "{path}" does not exist.')
         if self.hr_path == self.lr_path: warnings.warn("hr_path is equal to lr_path! Consider using SlidingDataset instead.", stacklevel=2)
         
-        self.hr_files = sorted(glob.glob(Path(self.hr_path, f"*.{extension}")))
-        self.lr_files = sorted(glob.glob(Path(self.lr_path, f"*.{extension}")))
+        self.hr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.hr_path))
+        self.lr_files = sorted(glob.glob(f"*.{extension}", root_dir=self.lr_path))
         for files, path in zip([self.hr_files, self.lr_files], [self.hr_path, self.lr_path]):
             if not len(files) > 0: raise FileNotFoundError(f'No .{extension} files exist in path "{path}".')
         if len(self.hr_files) != len(self.lr_files): raise FileNotFoundError(f"Mismatch between amounts of high-low-resolution images. Found {len(self.hr_files)} high-resolution and {len(self.lr_files)} low-resolution images.")
 
+        overlap = 0 if overlap is None else overlap
         if not hr_res > overlap: raise ValueError(f"hr_res must be greater than overlap. Given values are {hr_res} and {overlap} respectively.")
         self.stride = hr_res - overlap
         self.stack = stack.upper()
         self.mode = mode.upper()
         self.n_frames = _get_n_frames(n_frames, self.mode)
 
         self.preload = _preload(preload, [self.hr_path, self.lr_path], [self.hr_files, self.lr_files], self.mode, self.stack)
@@ -335,16 +337,16 @@
     
     def __getitem__(self, idx, pp=False):
         if idx >= len(self): raise IndexError(f"Tried to retrieve invalid image. Index {idx} is not less than {len(self)} total image frame slices.")
 
         is_val = idx in self.val_idx or pp
         image_idx, idx = _get_image_idx(idx, self.slices, self.tiles)
 
-        hr = _sliding_window(self.preload[0][image_idx] if self.preload else _load_sheet(self.hr_path, self.hr_files[image_idx], self.stack, self.mode), self.hr_res, self.stride, self.n_frames[0], self.slices[image_idx], idx)
-        lr = _sliding_window(self.preload[1][image_idx] if self.preload else _load_sheet(self.lr_path, self.lr_files[image_idx], self.stack, self.mode), self.hr_res//self.lr_scale, self.stride//self.lr_scale, self.n_frames[0], self.slices[image_idx], idx)
+        hr = _sliding_window(self.preload[0][image_idx] if self.preload else _load_sheet(self.hr_path, self.hr_files[image_idx], self.stack, self.mode), self.hr_res, self.stride, self.n_frames[0] if self.n_frames is not None else None, self.slices[image_idx], idx)
+        lr = _sliding_window(self.preload[1][image_idx] if self.preload else _load_sheet(self.lr_path, self.lr_files[image_idx], self.stack, self.mode), self.hr_res//self.lr_scale, self.stride//self.lr_scale, self.n_frames[0] if self.n_frames is not None else None, self.slices[image_idx], idx)
 
         return _transform_pair(hr, lr, self.hr_res, self.hr_res//self.lr_scale, False if is_val else self.rotation, self.transforms, self.n_frames)
     
     def __len__(self):
         return sum([self.tiles[idx] * self.slices[idx] for idx in range(len(self.hr_files))])
     
     def __repr__(self):
```

### Comparing `pssr-1.2.0/pssr/loss.py` & `pssr-1.2.1/pssr/loss.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,16 @@
         self.win_size = win_size
         self.mix = mix
 
     def forward(self, input, target):
         x = 1 - self.ssim(input, target)
         if self.mix < 1:
             # Combine SSIM with L1 loss with applied Gaussian window for elementwise multiplication against non-reduced L1 loss
-            l1 = F.conv2d(F.l1_loss(input, target, reduction="none"), self.gaussian.to(input.get_device()), groups=self.channels, padding=(self.win_size-1)//2).mean()  # F.conv2d with Gaussian filter
+            device = "cpu" if input.get_device() == -1 else input.get_device()
+            l1 = F.conv2d(F.l1_loss(input, target, reduction="none"), self.gaussian.to(device), groups=self.channels, padding=(self.win_size-1)//2).mean()  # F.conv2d with Gaussian filter
             x = self.mix*x + (1-self.mix)*l1
         return x
 
 def pixel_metric(mse : float, image_range : int = 255):
     r"""Simple metric for calculating average pixel error.
     
     Args:
```

### Comparing `pssr-1.2.0/pssr/models/_blocks.py` & `pssr-1.2.1/pssr/models/_blocks.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,17 +55,19 @@
                 conv.append(nn.ReLU(inplace=True))
 
                 conv.append(nn.Conv2d(in_channels if layer_idx == 0 else out_channels, out_channels, kernel_size=3, padding="same", dilation=dilation))
             self.dilations.append(conv)
 
         self.respass = nn.Conv2d(in_channels, out_channels, kernel_size=1)
 
+        self.min_size = max(dilations) * 2 + 1
         self.depth = depth
 
     def forward(self, x):
+        if x.shape[-1] < self.min_size: raise ValueError(f"Tensor size {x.shape} is smaller than than dilation kernel size {self.min_size}.")
         x = F.relu(sum([conv(x) for conv in self.dilations]) + self.respass(x))
         return x
 
 class PSP_Pooling(nn.Module):
     def __init__(self, channels, sizes):
         super().__init__()
```

### Comparing `pssr-1.2.0/pssr/models/_rdnet.py` & `pssr-1.2.1/pssr/models/_rdnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 Apache-2.0
 
 Source code of RDNet has been modified for use in PSSR.
 """
 
 import torch
 import torch.nn as nn
-from timm.layers.squeeze_excite import EffectiveSEModule
+from timm.layers import DropPath, LayerNorm2d, EffectiveSEModule
 from timm.models import named_apply
-from timm.models.layers import DropPath
-from timm.models.layers import LayerNorm2d
 from functools import partial
 
 class RDNet(nn.Module):
     def __init__(
         self,
         in_channels=1,
         n_init_features=128,
```

### Comparing `pssr-1.2.0/pssr/models/rdresunet.py` & `pssr-1.2.1/pssr/models/rdresunet.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 
 class RDResUNetA():
     def __new__(cls,
             channels : int = 1,
             hidden : list[int] = [1024, 1024, 512, 256],
             scale : int = 4,
             depth : int = 3,
-            dilations : list[list[int]] = [[1,3,15],[1,3],[1],[1]],
+            dilations : list[list[int]] = [[1],[1],[1,3],[1,3,15]],
             pool_sizes : list[int] = [1, 2, 4, 8],
             encoder_pool : bool = False,
             rdnet_kwargs = None
         ):
         r""":class:`RDResUNet` wrapper of Atrous Residual UNet as detailed in Diakogiannis et al., 2019.
         Provides alternative default arguments for an atrous network.
```

### Comparing `pssr-1.2.0/pssr/models/resunet.py` & `pssr-1.2.1/pssr/models/resunet.py`

 * *Files identical despite different names*

### Comparing `pssr-1.2.0/pssr/predict.py` & `pssr-1.2.1/pssr/predict.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,17 +170,17 @@
         pmax (float) : Percentile maximum image intensity. Default is 99.9.
     
     Returns:
         hr_norm (ndarray) : Normalized high-resolution ground truth image.
 
         hr_hat_norm (ndarray) : Normalized high-resolution prediction image.
     """
+    hr, hr_hat = np.asarray(hr), np.asarray(hr_hat)
     if len(hr.shape) != len(hr_hat.shape): raise ValueError(f"hr and hr_hat must have the same number of dimensions. Dimension lengths are {hr.shape} and {hr_hat.shape} respectively.")
-    hr_shape = hr.shape
-    hr_hat_shape = hr_hat.shape
+    hr_shape, hr_hat_shape = hr.shape, hr_hat.shape
 
     if len(hr.shape) < 3:
         hr, hr_hat = hr[np.newaxis, ...], hr_hat[np.newaxis, ...]
     hr, hr_hat = hr.reshape(-1, *hr.shape[-2:]), hr_hat.reshape(-1, *hr_hat.shape[-2:])
     if len(hr) != len(hr_hat): raise ValueError(f"hr and hr_hat must have the same number of images. Received {len(hr)} and {len(hr_hat)} images respectively.")
 
     hr_norms, hr_hat_norms = [], []
```

### Comparing `pssr-1.2.0/pssr/train.py` & `pssr-1.2.1/pssr/train.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,23 +14,24 @@
 from .predict import _collage_preds
 from .models._blocks import GradHist
 
 Image.MAX_IMAGE_PIXELS = None
 
 def train_paired(
         model : nn.Module,
-        dataset : Dataset, 
-        batch_size : int, 
-        loss_fn : nn.Module, 
-        optim : torch.optim.Optimizer, 
-        epochs : int, 
-        device : str = "cpu", 
-        scheduler : torch.optim.lr_scheduler.LRScheduler = None, 
-        clamp : bool = False, 
-        log_frequency : int = 50, 
+        dataset : Dataset,
+        batch_size : int,
+        loss_fn : nn.Module,
+        optim : torch.optim.Optimizer,
+        epochs : int,
+        device : str = "cpu",
+        scheduler : torch.optim.lr_scheduler = None,
+        clamp : bool = False,
+        log_frequency : int = 50,
+        collage_dir : str = "preds",
         dataloader_kwargs = None
     ):
     r"""Trains model on paired high-low-resolution crappified data.
 
     Args:
         model (nn.Module) : Model to train on paired data.
 
@@ -48,14 +49,16 @@
 
         scheduler (LRScheduler) : Optional learning rate scheduler for training. Default is None.
 
         clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         log_frequency (int) : Frequency to log losses and recalculate metrics in steps. Default is 50.
 
+        collage_dir (str) : Directory to save validation collages. A value of None skips the collage. Default is "preds".
+
         dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
     Returns:
         losses (list[float]) : List of losses during training.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
@@ -65,14 +68,15 @@
 
     model.to(device)
 
     losses = []
     for epoch in range(epochs):
         # Train
         model.train()
+        print(f"Epoch {epoch}:")
 
         progress = tqdm(train_dataloader)
         for batch_idx, (hr, lr) in enumerate(progress):
             hr, lr = hr.to(device), lr.to(device)
 
             hr_hat = model(lr)
             if clamp:
@@ -111,33 +115,35 @@
         print(f"Epoch {epoch} validation loss: {val_loss:4f}\n")
 
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
                 scheduler.step()
-  
-        collage = _collage_preds(lr, hr_hat, hr, crop_res=dataset.crop_res)
-        os.makedirs("preds", exist_ok=True)
-        collage.save(f"preds/epoch{epoch}_loss{val_loss:.3f}.png")
+        
+        if collage_dir:
+            collage = _collage_preds(lr, hr_hat, hr, crop_res=dataset.crop_res)
+            os.makedirs(collage_dir, exist_ok=True)
+            collage.save(f"{collage_dir}/epoch{epoch}_loss{val_loss:.3f}.png")
 
     return losses
 
 def train_crappifier(
-        model : nn.Module, 
-        dataset : Dataset, 
-        batch_size : int, 
-        optim : torch.optim.Optimizer, 
-        epochs : int, 
-        sigma : int = 5, 
-        clip : float = 3, 
-        device : str = "cpu", 
-        scheduler : torch.optim.lr_scheduler.LRScheduler = None, 
-        clamp : bool = False, 
-        log_frequency : int = 50, 
+        model : nn.Module,
+        dataset : Dataset,
+        batch_size : int,
+        optim : torch.optim.Optimizer,
+        epochs : int,
+        sigma : int = 5,
+        clip : float = 3,
+        device : str = "cpu",
+        scheduler : torch.optim.lr_scheduler = None,
+        clamp : bool = False,
+        log_frequency : int = 50,
+        collage_dir : str = "preds",
         dataloader_kwargs = None
     ):
     r"""EXPERIMENTAL, NOT CURRENTLY RECOMMENDED FOR MOST WORKFLOWS!
     
     Trains an :class:`nn.Module` model as a crappifier on high-low-resolution paired data.
     The model must output an image the same size as the input/have a `scale` value of 1.
     This is not necessary if you are using a :class:`Crappifier` instance as your crappifier.
@@ -161,14 +167,16 @@
 
         scheduler (LRScheduler) : Optional learning rate scheduler for training. Default is None.
 
         clamp (bool) : Whether to clamp model image output before weight calculation. Default is False.
 
         log_frequency (int) : Frequency to log losses and recalculate metrics in steps. Default is 50.
 
+        collage_dir (str) : Directory to save validation collages. A value of None skips the collage. Default is "preds".
+
         dataloader_kwargs (dict[str, Any]) : Keyword arguments for pytorch ``Dataloader``. Default is None.
 
     Returns:
         losses (list[float]) : List of losses during training.
     """
     dataloader_kwargs = {} if dataloader_kwargs is None else dataloader_kwargs
     train_dataloader = DataLoader(dataset, batch_size, sampler=_RandomIterIdx(_invert_idx(dataset.val_idx, len(dataset))), **dataloader_kwargs)
@@ -182,14 +190,15 @@
     hist_fn = GradHist(sigma=sigma)
     ssim_loss = SSIMLoss(ms=False)
 
     losses = []
     for epoch in range(epochs):
         # Train
         model.train()
+        print(f"Epoch {epoch}:")
 
         progress = tqdm(train_dataloader)
         for batch_idx, (hr, lr) in enumerate(progress):
             scale = int(hr.shape[-1]/lr.shape[-1])
             ds_hr = hr[:, :, ::scale, ::scale]
             ds_hr = ds_hr.to(device)
 
@@ -236,17 +245,19 @@
 
         if scheduler:
             if include_metric:
                 scheduler.step(val_loss)
             else:
                 scheduler.step()
 
-        collage = _collage_preds(lr, lr_hat, hr, crop_res=dataset.crop_res)
-        os.makedirs("preds", exist_ok=True)
-        collage.save(f"preds/pred{epoch}_loss{val_loss:.3f}.png")
+        if collage_dir:
+            collage = _collage_preds(lr, lr_hat, hr, crop_res=dataset.crop_res)
+            os.makedirs(collage_dir, exist_ok=True)
+            collage.save(f"{collage_dir}/pred{epoch}_loss{val_loss:.3f}.png")
+
     return losses
 
 def approximate_crappifier(crappifier : Crappifier, space : list[Dimension], dataset : Dataset, max_images = None, opt_kwargs = None):
     r"""Approximates :class:`Crappifier` parameters from ground truth paired images. Uses Bayesian optimization because Crappifier functions are not differentiable.
 
     Args:
         crappifier (Crappifier) : Crappifier whose parameter space will be optimized.
```

### Comparing `pssr-1.2.0/pyproject.toml` & `pssr-1.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pssr"
-version = "1.2.0"
+version = "1.2.1"
 description = "Point-Scanning Super-Resolution"
 authors = ["Hayden Stites"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/ucsdmanorlab/PSSR"
 documentation = "https://ucsdmanorlab.github.io/PSSR/"
 classifiers = [
@@ -16,30 +16,26 @@
     "Environment :: GPU :: NVIDIA CUDA",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Image Processing",
     "Topic :: Documentation :: Sphinx",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.9"
-torch = "^2.0.0"
-numpy = "^1.26.4"
-pillow = "^10.2.0"
+python = "^3.10"
+torch = ">=1.11.0"
+numpy = "^1.22.4"
+pillow = ">=9.1.0"
 czifile = "^2019.7.2"
-tifffile = "^2024.4.24"
+tifffile = ">=2019.7.26"
 scikit-image = ">=0.18.0"
-scikit-optimize = "^0.9.0"
-tqdm = "^4.66.2"
+scikit-optimize = ">=0.9.0"
+tqdm = "^4.0.0"
 pytorch-msssim = "^1.0.0"
-psutil = "^5.9.8"
-
-timm = {version = "^0.9.12", optional = true}
-
-[tool.poetry.extras]
-models = ["timm"]
+psutil = ">=5.0.0"
+timm = ">=0.8.0"
 
 [tool.poetry.scripts]
 pssr = "pssr.__main__:run"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pssr-1.2.0/PKG-INFO` & `pssr-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 Metadata-Version: 2.1
 Name: pssr
-Version: 1.2.0
+Version: 1.2.1
 Summary: Point-Scanning Super-Resolution
 Home-page: https://github.com/ucsdmanorlab/PSSR
 License: MIT
 Author: Hayden Stites
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
-Provides-Extra: models
 Requires-Dist: czifile (>=2019.7.2,<2020.0.0)
-Requires-Dist: numpy (>=1.26.4,<2.0.0)
-Requires-Dist: pillow (>=10.2.0,<11.0.0)
-Requires-Dist: psutil (>=5.9.8,<6.0.0)
+Requires-Dist: numpy (>=1.22.4,<2.0.0)
+Requires-Dist: pillow (>=9.1.0)
+Requires-Dist: psutil (>=5.0.0)
 Requires-Dist: pytorch-msssim (>=1.0.0,<2.0.0)
 Requires-Dist: scikit-image (>=0.18.0)
-Requires-Dist: scikit-optimize (>=0.9.0,<0.10.0)
-Requires-Dist: tifffile (>=2024.4.24,<2025.0.0)
-Requires-Dist: timm (>=0.9.12,<0.10.0) ; extra == "models"
-Requires-Dist: torch (>=2.0.0,<3.0.0)
-Requires-Dist: tqdm (>=4.66.2,<5.0.0)
+Requires-Dist: scikit-optimize (>=0.9.0)
+Requires-Dist: tifffile (>=2019.7.26)
+Requires-Dist: timm (>=0.8.0)
+Requires-Dist: torch (>=1.11.0)
+Requires-Dist: tqdm (>=4.0.0,<5.0.0)
 Project-URL: Documentation, https://ucsdmanorlab.github.io/PSSR/
 Project-URL: Repository, https://github.com/ucsdmanorlab/PSSR
 Description-Content-Type: text/markdown
 
 # Point-Scanning Super-Resolution (**PSSR**)
 
 **PSSR** is a standardized [PyTorch](https://pytorch.org)-based workflow for super-resolution tasks using microscopy images.
```

