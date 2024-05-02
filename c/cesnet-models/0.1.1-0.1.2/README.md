# Comparing `tmp/cesnet-models-0.1.1.tar.gz` & `tmp/cesnet_models-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cesnet-models-0.1.1.tar", last modified: Tue Apr  9 16:36:10 2024, max compression
+gzip compressed data, was "cesnet_models-0.1.2.tar", last modified: Thu May  2 07:30:41 2024, max compression
```

## Comparing `cesnet-models-0.1.1.tar` & `cesnet_models-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.208320 cesnet-models-0.1.1/
--rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet-models-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     3232 2024-04-09 16:36:10.208320 cesnet-models-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1875 2024-04-09 16:32:38.000000 cesnet-models-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.185074 cesnet-models-0.1.1/cesnet_models/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.1/cesnet_models/__init__.py
--rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet-models-0.1.1/cesnet_models/_models_meta.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.205309 cesnet-models-0.1.1/cesnet_models/architectures/
--rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet-models-0.1.1/cesnet_models/architectures/__init__.py
--rw-rw-rw-   0        0        0     8085 2024-04-04 12:12:16.000000 cesnet-models-0.1.1/cesnet_models/architectures/multimodal_cesnet.py
--rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet-models-0.1.1/cesnet_models/helpers.py
--rw-rw-rw-   0        0        0    11866 2024-04-09 15:28:32.000000 cesnet-models-0.1.1/cesnet_models/models.py
--rw-rw-rw-   0        0        0    14235 2024-04-09 15:13:45.000000 cesnet-models-0.1.1/cesnet_models/transforms.py
-drwxrwxrwx   0        0        0        0 2024-04-09 16:36:10.206314 cesnet-models-0.1.1/cesnet_models.egg-info/
--rw-rw-rw-   0        0        0     3232 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      438 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      149 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-04-09 16:36:10.000000 cesnet-models-0.1.1/cesnet_models.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1448 2024-04-09 16:34:58.000000 cesnet-models-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-09 16:36:10.208320 cesnet-models-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.565347 cesnet_models-0.1.2/
+-rw-rw-rw-   0        0        0     1541 2023-09-18 09:03:44.000000 cesnet_models-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     3557 2024-05-02 07:30:41.564345 cesnet_models-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2200 2024-04-10 08:36:57.000000 cesnet_models-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.538796 cesnet_models-0.1.2/cesnet_models/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.2/cesnet_models/__init__.py
+-rw-rw-rw-   0        0        0     5949 2024-04-08 09:20:47.000000 cesnet_models-0.1.2/cesnet_models/_models_meta.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.562348 cesnet_models-0.1.2/cesnet_models/architectures/
+-rw-rw-rw-   0        0        0        0 2023-01-18 16:43:04.000000 cesnet_models-0.1.2/cesnet_models/architectures/__init__.py
+-rw-rw-rw-   0        0        0     2131 2024-04-30 13:12:57.000000 cesnet_models-0.1.2/cesnet_models/architectures/cnn_resblock.py
+-rw-rw-rw-   0        0        0     8583 2024-04-30 15:07:58.000000 cesnet_models-0.1.2/cesnet_models/architectures/multimodal_cesnet.py
+-rw-rw-rw-   0        0        0     9979 2024-04-30 15:51:58.000000 cesnet_models-0.1.2/cesnet_models/architectures/multimodal_cesnet_enhanced.py
+-rw-rw-rw-   0        0        0       71 2024-04-29 12:31:20.000000 cesnet_models-0.1.2/cesnet_models/constants.py
+-rw-rw-rw-   0        0        0     1112 2024-03-18 11:22:51.000000 cesnet_models-0.1.2/cesnet_models/helpers.py
+-rw-rw-rw-   0        0        0    11966 2024-04-30 13:57:45.000000 cesnet_models-0.1.2/cesnet_models/models.py
+-rw-rw-rw-   0        0        0    14604 2024-04-30 12:17:48.000000 cesnet_models-0.1.2/cesnet_models/transforms.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:30:41.563346 cesnet_models-0.1.2/cesnet_models.egg-info/
+-rw-rw-rw-   0        0        0     3557 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      567 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      149 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-05-02 07:30:41.000000 cesnet_models-0.1.2/cesnet_models.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1448 2024-05-02 07:30:07.000000 cesnet_models-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-02 07:30:41.565347 cesnet_models-0.1.2/setup.cfg
```

### Comparing `cesnet-models-0.1.1/LICENCE` & `cesnet_models-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.1/PKG-INFO` & `cesnet_models-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
@@ -35,19 +35,19 @@
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
 [![](https://img.shields.io/badge/docs-cesnet--models-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
 [![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
-The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights. The weights were trained using public datasets available in the [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) package.
+The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights.
 
 The newest network architecture is named Multi-modal CESNET v2 (mm-CESNET-v2) and is visualized in the following picture. See the [getting started](https://cesnet.github.io/cesnet-models/getting_started/) page and [models](https://cesnet.github.io/cesnet-models/reference_models/) reference for more information.
 
-:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing three large network traffic datasets. :frog: :frog:
+:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing large TLS and QUIC traffic datasets. :frog: :frog:
 
 :notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
 
 ### Multi-modal CESNET v2
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/model-mm-cesnet-v2.png" width="450">
 </p>
@@ -61,7 +61,19 @@
 ```
 
 or for editable install with:
 
 ```bash
 pip install -e git+https://github.com/CESNET/cesnet-models
 ```
+
+## Papers
+
+Models from the following papers are included:
+
+* [Fine-grained TLS services classification with reject option](https://doi.org/10.1016/j.comnet.2022.109467) <br>
+Jan Luxemburk and Tomáš Čejka <br>
+Computer Networks, 2023
+
+* [Encrypted traffic classification: the QUIC case](https://doi.org/10.23919/TMA58422.2023.10199052) <br>
+Jan Luxemburk and Karel Hynek <br>
+2023 7th Network Traffic Measurement and Analysis Conference (TMA)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cesnet-models-0.1.1/README.md` & `cesnet_models-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
 [![](https://img.shields.io/badge/docs-cesnet--models-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
 [![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
-The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights. The weights were trained using public datasets available in the [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) package.
+The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights.
 
 The newest network architecture is named Multi-modal CESNET v2 (mm-CESNET-v2) and is visualized in the following picture. See the [getting started](https://cesnet.github.io/cesnet-models/getting_started/) page and [models](https://cesnet.github.io/cesnet-models/reference_models/) reference for more information.
 
-:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing three large network traffic datasets. :frog: :frog:
+:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing large TLS and QUIC traffic datasets. :frog: :frog:
 
 :notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
 
 ### Multi-modal CESNET v2
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/model-mm-cesnet-v2.png" width="450">
 </p>
@@ -29,8 +29,20 @@
 pip install cesnet-models
 ```
 
 or for editable install with:
 
 ```bash
 pip install -e git+https://github.com/CESNET/cesnet-models
-```
+```
+
+## Papers
+
+Models from the following papers are included:
+
+* [Fine-grained TLS services classification with reject option](https://doi.org/10.1016/j.comnet.2022.109467) <br>
+Jan Luxemburk and Tomáš Čejka <br>
+Computer Networks, 2023
+
+* [Encrypted traffic classification: the QUIC case](https://doi.org/10.23919/TMA58422.2023.10199052) <br>
+Jan Luxemburk and Karel Hynek <br>
+2023 7th Network Traffic Measurement and Analysis Conference (TMA)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cesnet-models-0.1.1/cesnet_models/_models_meta.py` & `cesnet_models-0.1.2/cesnet_models/_models_meta.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.1/cesnet_models/architectures/multimodal_cesnet.py` & `cesnet_models-0.1.2/cesnet_models/architectures/multimodal_cesnet.py`

 * *Files 23% similar despite different names*

```diff
@@ -4,22 +4,25 @@
 import torch
 import torch.nn.functional as F
 from torch import Tensor, nn
 
 
 class NormalizationEnum(Enum):
     BATCH_NORM = "batch-norm"
+    GROUP_NORM = "group-norm"
     LAYER_NORM = "layer-norm"
     INSTANCE_NORM = "instance-norm"
     NO_NORM = "no-norm"
     def __str__(self): return self.value
 
-def conv_norm_from_enum(size: int, norm_enum: NormalizationEnum):
+def conv_norm_from_enum(size: int, norm_enum: NormalizationEnum, group_norm_groups: int = 8):
     if norm_enum == NormalizationEnum.BATCH_NORM:
         return [nn.BatchNorm1d(size)]
+    elif norm_enum == NormalizationEnum.GROUP_NORM:
+        return [nn.GroupNorm(num_groups=group_norm_groups, num_channels=size)]
     elif norm_enum == NormalizationEnum.INSTANCE_NORM:
         return [nn.InstanceNorm1d(size)]
     elif norm_enum == NormalizationEnum.NO_NORM:
         return []
     else:
         raise ValueError(f"Bad normalization for nn.Conv1d: {str(norm_enum)}")
 
@@ -40,138 +43,138 @@
     def __init__(self, kernel_size, p=3, eps=1e-6):
         super(GeM, self).__init__()
         self.p = nn.Parameter(torch.ones(1) * p)
         self.kernel_size = kernel_size
         self.eps = eps
 
     def forward(self, x):
-        return self.gem(x, p=self.p, eps=self.eps)
+        return self.gem(x, p=self.p, eps=self.eps) # type: ignore
 
     def gem(self, x, p: int | nn.Parameter = 3, eps=1e-6):
         return F.avg_pool1d(x.clamp(min=eps).pow(p), self.kernel_size).pow(1./p)
 
     def __repr__(self):
         return self.__class__.__name__ + \
                 "(" + "kernel_size=" + str(self.kernel_size) + ", p=" + "{:.4f}".format(self.p.data.tolist()[0]) + \
                 ", eps=" + str(self.eps) + ")"
 
 class Multimodal_CESNET(nn.Module):
     def __init__(self, num_classes: int,
                        flowstats_input_size: int,
                        ppi_input_channels: int,
-                       use_flowstats: bool = True, add_ppi_to_flowstats: bool = False,
+                       use_flowstats: bool = True, add_ppi_to_mlp_flowstats: bool = False,
                        conv_normalization: NormalizationEnum = NormalizationEnum.BATCH_NORM, linear_normalization: NormalizationEnum = NormalizationEnum.BATCH_NORM,
-                       cnn_channels1: int = 200, cnn_channels2: int = 300, cnn_channels3: int = 300, cnn_num_hidden: int = 3, cnn_depthwise: bool = False,
-                       cnn_use_pooling: bool = True, cnn_dropout_rate: float = 0.1,
-                       flowstats_size: int = 225, flowstats_out_size: int = 225, flowstats_num_hidden: int = 2, flowstats_dropout_rate: float = 0.1,
-                       latent_size: int = 600, latent_num_hidden: int = 0, latent_dropout_rate: float = 0.2,
+                       cnn_ppi_channels1: int = 200, cnn_ppi_channels2: int = 300, cnn_ppi_channels3: int = 300, cnn_ppi_num_blocks: int = 3, cnn_ppi_depthwise: bool = False,
+                       cnn_ppi_use_pooling: bool = True, cnn_ppi_dropout_rate: float = 0.1,
+                       mlp_flowstats_size1: int = 225, mlp_flowstats_size2: int = 225, mlp_flowstats_num_hidden: int = 2, mlp_flowstats_dropout_rate: float = 0.1,
+                       mlp_shared_size: int = 600, mlp_shared_num_hidden: int = 0, mlp_shared_dropout_rate: float = 0.2,
                        ):
         super().__init__()
-        if add_ppi_to_flowstats and not use_flowstats:
-            raise ValueError("add_ppi_to_flowstats requires use_flowstats")
-        if cnn_depthwise and cnn_channels1 % ppi_input_channels != 0:
-            raise ValueError(f"cnn_channels1 ({cnn_channels1}) must be divisible by ppi_input_channels ({ppi_input_channels}) when using cnn_depthwise")
+        if add_ppi_to_mlp_flowstats and not use_flowstats:
+            raise ValueError("add_ppi_to_mlp_flowstats requires use_flowstats")
+        if cnn_ppi_depthwise and cnn_ppi_channels1 % ppi_input_channels != 0:
+            raise ValueError(f"cnn_ppi_channels1 ({cnn_ppi_channels1}) must be divisible by ppi_input_channels ({ppi_input_channels}) when using cnn_ppi_depthwise")
 
         self.num_classes = num_classes
         self.flowstats_input_size = flowstats_input_size
         self.ppi_input_channels = ppi_input_channels
         self.use_flowstats = use_flowstats
-        self.add_ppi_to_flowstats = add_ppi_to_flowstats
-        self.latent_size = latent_size
-        self.cnn_use_pooling = cnn_use_pooling
+        self.add_ppi_to_mlp_flowstats = add_ppi_to_mlp_flowstats
+        self.mlp_shared_size = mlp_shared_size
+        self.cnn_ppi_use_pooling = cnn_ppi_use_pooling
 
         CNN_PPI_OUTPUT_LEN = 10
         PPI_LEN = 30
         conv_norm = partial(conv_norm_from_enum, norm_enum=conv_normalization)
         linear_norm = partial(linear_norm_from_enum, norm_enum=linear_normalization)
-        conv1d_groups = ppi_input_channels if cnn_depthwise else 1
-        mlp_flowstats_input_size = flowstats_input_size + (ppi_input_channels * PPI_LEN) if add_ppi_to_flowstats else flowstats_input_size
-        mlp_shared_input_size = flowstats_out_size if use_flowstats else 0
-        if cnn_use_pooling:
-            mlp_shared_input_size += cnn_channels3
+        conv1d_groups = ppi_input_channels if cnn_ppi_depthwise else 1
+        mlp_flowstats_input_size = flowstats_input_size + (ppi_input_channels * PPI_LEN) if add_ppi_to_mlp_flowstats else flowstats_input_size
+        mlp_shared_input_size = mlp_flowstats_size2 if use_flowstats else 0
+        if cnn_ppi_use_pooling:
+            mlp_shared_input_size += cnn_ppi_channels3
         else:
-            mlp_shared_input_size += cnn_channels3 * CNN_PPI_OUTPUT_LEN
+            mlp_shared_input_size += cnn_ppi_channels3 * CNN_PPI_OUTPUT_LEN
 
         self.cnn_ppi = nn.Sequential(
             # [(W−K+2P)/S]+1
             # Input: 30 * 3
-            nn.Conv1d(self.ppi_input_channels, cnn_channels1, kernel_size=7, stride=1, groups=conv1d_groups, padding=3),
+            nn.Conv1d(self.ppi_input_channels, cnn_ppi_channels1, kernel_size=7, stride=1, groups=conv1d_groups, padding=3),
             nn.ReLU(inplace=False),
-            *conv_norm(cnn_channels1),
+            *conv_norm(cnn_ppi_channels1),
 
             # 30 x channels1
             *(nn.Sequential(
-                nn.Conv1d(cnn_channels1, cnn_channels1, kernel_size=5, stride=1, groups=conv1d_groups, padding=2),
+                nn.Conv1d(cnn_ppi_channels1, cnn_ppi_channels1, kernel_size=5, stride=1, groups=conv1d_groups, padding=2),
                 nn.ReLU(inplace=False),
-                *conv_norm(cnn_channels1),) for _ in range(cnn_num_hidden)),
+                *conv_norm(cnn_ppi_channels1),) for _ in range(cnn_ppi_num_blocks)),
 
             # 30 x channels1
-            nn.Conv1d(cnn_channels1, cnn_channels2, kernel_size=5, stride=1),
+            nn.Conv1d(cnn_ppi_channels1, cnn_ppi_channels2, kernel_size=5, stride=1),
             nn.ReLU(inplace=False),
-            *conv_norm(cnn_channels2),
+            *conv_norm(cnn_ppi_channels2),
             # 26 * channels2
-            nn.Conv1d(cnn_channels2, cnn_channels2, kernel_size=5, stride=1),
+            nn.Conv1d(cnn_ppi_channels2, cnn_ppi_channels2, kernel_size=5, stride=1),
             nn.ReLU(inplace=False),
-            *conv_norm(cnn_channels2),
+            *conv_norm(cnn_ppi_channels2),
             # 22 * channels2
-            nn.Conv1d(cnn_channels2, cnn_channels3, kernel_size=4, stride=2),
+            nn.Conv1d(cnn_ppi_channels2, cnn_ppi_channels3, kernel_size=4, stride=2),
             nn.ReLU(inplace=False),
             # 10 * channels3
             # CNN_PPI_OUTPUT_LEN = 10
         )
-        if cnn_use_pooling:
+        if cnn_ppi_use_pooling:
             self.cnn_global_pooling = nn.Sequential(
                 GeM(kernel_size=CNN_PPI_OUTPUT_LEN),
                 nn.Flatten(),
-                *linear_norm(cnn_channels3),
-                nn.Dropout(cnn_dropout_rate),
+                *linear_norm(cnn_ppi_channels3),
+                nn.Dropout(cnn_ppi_dropout_rate),
             )
         else:
             self.cnn_flatten_without_pooling = nn.Sequential(
                 nn.Flatten(),
-                *linear_norm(cnn_channels3 * CNN_PPI_OUTPUT_LEN),
-                nn.Dropout(cnn_dropout_rate),
+                *linear_norm(cnn_ppi_channels3 * CNN_PPI_OUTPUT_LEN),
+                nn.Dropout(cnn_ppi_dropout_rate),
             )
         self.mlp_flowstats = nn.Sequential(
-            nn.Linear(mlp_flowstats_input_size, flowstats_size),
+            nn.Linear(mlp_flowstats_input_size, mlp_flowstats_size1),
             nn.ReLU(inplace=False),
-            *linear_norm(flowstats_size),
+            *linear_norm(mlp_flowstats_size1),
 
             *(nn.Sequential(
-                nn.Linear(flowstats_size, flowstats_size),
+                nn.Linear(mlp_flowstats_size1, mlp_flowstats_size1),
                 nn.ReLU(inplace=False),
-                *linear_norm(flowstats_size)) for _ in range(flowstats_num_hidden)),
+                *linear_norm(mlp_flowstats_size1)) for _ in range(mlp_flowstats_num_hidden)),
 
-            nn.Linear(flowstats_size, flowstats_out_size),
+            nn.Linear(mlp_flowstats_size1, mlp_flowstats_size2),
             nn.ReLU(inplace=False),
-            *linear_norm(flowstats_out_size),
-            nn.Dropout(flowstats_dropout_rate),
+            *linear_norm(mlp_flowstats_size2),
+            nn.Dropout(mlp_flowstats_dropout_rate),
         )
         self.mlp_shared = nn.Sequential(
-            nn.Linear(mlp_shared_input_size, latent_size),
+            nn.Linear(mlp_shared_input_size, mlp_shared_size),
             nn.ReLU(inplace=False),
-            *linear_norm(latent_size),
-            nn.Dropout(latent_dropout_rate),
+            *linear_norm(mlp_shared_size),
+            nn.Dropout(mlp_shared_dropout_rate),
 
             *(nn.Sequential(
-                nn.Linear(latent_size, latent_size),
+                nn.Linear(mlp_shared_size, mlp_shared_size),
                 nn.ReLU(inplace=False),
-                *linear_norm(latent_size),
-                nn.Dropout(latent_dropout_rate)) for _ in range(latent_num_hidden)),
+                *linear_norm(mlp_shared_size),
+                nn.Dropout(mlp_shared_dropout_rate)) for _ in range(mlp_shared_num_hidden)),
         )
-        self.classifier = nn.Linear(latent_size, num_classes)
+        self.classifier = nn.Linear(mlp_shared_size, num_classes)
 
     def _forward_impl(self, ppi, flowstats):
         out = self.cnn_ppi(ppi)
-        if self.cnn_use_pooling:
+        if self.cnn_ppi_use_pooling:
             out = self.cnn_global_pooling(out)
         else:
             out = self.cnn_flatten_without_pooling(out)
         if self.use_flowstats:
-            if self.add_ppi_to_flowstats:
+            if self.add_ppi_to_mlp_flowstats:
                 flowstats_input = torch.column_stack([torch.flatten(ppi, 1), flowstats])
             else:
                 flowstats_input = flowstats
             out_flowstats = self.mlp_flowstats(flowstats_input)
             out = torch.column_stack([out, out_flowstats])
         out = self.mlp_shared(out)
         logits = self.classifier(out)
```

### Comparing `cesnet-models-0.1.1/cesnet_models/helpers.py` & `cesnet_models-0.1.2/cesnet_models/helpers.py`

 * *Files identical despite different names*

### Comparing `cesnet-models-0.1.1/cesnet_models/models.py` & `cesnet_models-0.1.2/cesnet_models/models.py`

 * *Files 5% similar despite different names*

```diff
@@ -110,27 +110,27 @@
         num_classes: Number of classes.
         flowstats_input_size: Size of the flow statistics input.
         ppi_input_channels: Number of channels in the PPI input.
     """
     v2_model_configuration = {
         "conv_normalization": NormalizationEnum.BATCH_NORM,
         "linear_normalization": NormalizationEnum.BATCH_NORM,
-        "cnn_num_hidden": 3,
-        "cnn_channels1": 200,
-        "cnn_channels2": 300,
-        "cnn_channels3": 300,
-        "cnn_use_pooling": True,
-        "cnn_dropout_rate": 0.1,
-        "flowstats_num_hidden": 2,
-        "flowstats_size": 225,
-        "flowstats_out_size": 225,
-        "flowstats_dropout_rate": 0.1,
-        "latent_num_hidden":  0,
-        "latent_size": 600,
-        "latent_dropout_rate": 0.2,
+        "cnn_ppi_num_blocks": 3,
+        "cnn_ppi_channels1": 200,
+        "cnn_ppi_channels2": 300,
+        "cnn_ppi_channels3": 300,
+        "cnn_ppi_use_pooling": True,
+        "cnn_ppi_dropout_rate": 0.1,
+        "mlp_flowstats_num_hidden": 2,
+        "mlp_flowstats_size1": 225,
+        "mlp_flowstats_size2": 225,
+        "mlp_flowstats_dropout_rate": 0.1,
+        "mlp_shared_num_hidden":  0,
+        "mlp_shared_size": 600,
+        "mlp_shared_dropout_rate": 0.2,
     }
     return _multimodal_cesnet(model_configuration=v2_model_configuration,
                               weights=weights,
                               model_dir=model_dir,
                               num_classes=num_classes,
                               flowstats_input_size=flowstats_input_size,
                               ppi_input_channels=ppi_input_channels)
@@ -194,27 +194,27 @@
         num_classes: Number of classes.
         flowstats_input_size: Size of the flow statistics input.
         ppi_input_channels: Number of channels in the PPI input.
     """
     v1_model_configuration = {
         "conv_normalization": NormalizationEnum.BATCH_NORM,
         "linear_normalization": NormalizationEnum.BATCH_NORM,
-        "cnn_num_hidden": 2,
-        "cnn_channels1": 72,
-        "cnn_channels2": 128,
-        "cnn_channels3": 128,
-        "cnn_use_pooling": False,
-        "cnn_dropout_rate": 0.2,
-        "flowstats_num_hidden": 2,
-        "flowstats_size": 64,
-        "flowstats_out_size": 32,
-        "flowstats_dropout_rate": 0.2,
-        "latent_num_hidden": 1,
-        "latent_size": 480,
-        "latent_dropout_rate": 0.2,
+        "cnn_ppi_num_blocks": 2,
+        "cnn_ppi_channels1": 72,
+        "cnn_ppi_channels2": 128,
+        "cnn_ppi_channels3": 128,
+        "cnn_ppi_use_pooling": False,
+        "cnn_ppi_dropout_rate": 0.2,
+        "mlp_flowstats_num_hidden": 2,
+        "mlp_flowstats_size1": 64,
+        "mlp_flowstats_size2": 32,
+        "mlp_flowstats_dropout_rate": 0.2,
+        "mlp_shared_num_hidden": 1,
+        "mlp_shared_size": 480,
+        "mlp_shared_dropout_rate": 0.2,
     }
     return _multimodal_cesnet(model_configuration=v1_model_configuration,
                               weights=weights,
                               model_dir=model_dir,
                               num_classes=num_classes,
                               flowstats_input_size=flowstats_input_size,
                               ppi_input_channels=ppi_input_channels)
```

### Comparing `cesnet-models-0.1.1/cesnet_models/transforms.py` & `cesnet_models-0.1.2/cesnet_models/transforms.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 from typing import Optional
 
 import numpy as np
 from sklearn.preprocessing import MinMaxScaler, RobustScaler, StandardScaler
 from torch import nn
 from typing_extensions import assert_never
 
-IPT_POS = 0
-DIR_POS = 1
-SIZE_POS = 2
-PHIST_BIN_COUNT = 8
+from cesnet_models.constants import PHIST_BIN_COUNT, PPI_DIR_POS, PPI_IPT_POS, PPI_SIZE_POS
 
 
 def get_scaler_attrs(scaler: StandardScaler | RobustScaler | MinMaxScaler) -> dict[str, list[float]]:
     if isinstance(scaler, StandardScaler):
         assert hasattr(scaler, "mean_") and scaler.mean_ is not None and hasattr(scaler, "scale_") and scaler.scale_ is not None
         scaler_attrs = {"mean_": scaler.mean_.tolist(), "scale_": scaler.scale_.tolist()}
     elif isinstance(scaler, RobustScaler):
@@ -44,14 +41,15 @@
     """Available scalers for flow statistics, packet sizes, and inter-packet times."""
     STANDARD = "standard"
     """Standardize features by removing the mean and scaling to unit variance - [`StandardScaler`](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.StandardScaler.html)."""
     ROBUST = "robust"
     """Robust scaling with the median and the interquartile range - [`RobustScaler`](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.RobustScaler.html)."""
     MINMAX = "minmax"
     """Scaling to a (0, 1) range - [`MinMaxScaler`](https://scikit-learn.org/stable/modules/generated/sklearn.preprocessing.MinMaxScaler.html)."""
+    NO_SCALING = "no-scaling"
     def __str__(self): return self.value
 
 class ClipAndScalePPI(nn.Module):
     """
     Transform class for scaling of per-packet information (PPI) sequences. This transform clips packet sizes and inter-packet times and scales them using a specified scaler.
     This class inherits from `nn.Module`, and the data transformation is implemented in the `forward` method.
 
@@ -64,25 +62,25 @@
 
     Expected format of input PPI sequences: `(batch_size, ppi_length, ppi_channels)`
 
     !!! info Padding
         The zero padding in PPI sequences is preserved during scaling, i.e., the padding zeroes are kept in the output.
 
     Parameters:
-        psizes_scaler_enum: What scaler should be used for packet sizes. Options are standard, robust, and minmax.
-        ipt_scaler_enum: What scaler should be used for inter-packet times. Options are standard, robust, and minmax.
+        psizes_scaler_enum: What scaler should be used for packet sizes. Options are standard, robust, minmax, and no-scaling.
+        ipt_scaler_enum: What scaler should be used for inter-packet times. Options are standard, robust, minmax, and no-scaling.
         pszies_min: Clip packet sizes to this minimum value.
         psizes_max: Clip packet sizes to this maximum value.
         ipt_min: Clip inter-packet times to this minimum value.
         ipt_max: Clip inter-packet times to this maximum value.
         psizes_scaler_attrs: To use a pre-fitted packet sizes scaler, provide its attributes here.
         ipt_scaler_attrs: To use a pre-fitted inter-packet times scaler, provide its attributes here.
     """
-    psizes_scaler: StandardScaler | RobustScaler | MinMaxScaler
-    ipt_scaler: StandardScaler | RobustScaler | MinMaxScaler
+    psizes_scaler: StandardScaler | RobustScaler | MinMaxScaler | None
+    ipt_scaler: StandardScaler | RobustScaler | MinMaxScaler | None
     pszies_min: int
     psizes_max: int
     ipt_min: int
     ipt_max: int
 
     def __init__(self,
                  psizes_scaler_enum: ScalerEnum | str = ScalerEnum.STANDARD,
@@ -96,65 +94,68 @@
         super().__init__()
         if psizes_scaler_enum == ScalerEnum.STANDARD:
             self.psizes_scaler = StandardScaler()
         elif psizes_scaler_enum == ScalerEnum.ROBUST:
             self.psizes_scaler = RobustScaler()
         elif psizes_scaler_enum == ScalerEnum.MINMAX:
             self.psizes_scaler = MinMaxScaler()
+        elif psizes_scaler_enum == ScalerEnum.NO_SCALING:
+            self.psizes_scaler = None
         else:
             raise ValueError(f"psizes_scaler_enum must be one of {ScalerEnum.__members__}")
         if ipt_scaler_enum == ScalerEnum.STANDARD:
             self.ipt_scaler = StandardScaler()
         elif ipt_scaler_enum == ScalerEnum.ROBUST:
             self.ipt_scaler = RobustScaler()
         elif ipt_scaler_enum == ScalerEnum.MINMAX:
             self.ipt_scaler = MinMaxScaler()
+        elif ipt_scaler_enum == ScalerEnum.NO_SCALING:
+            self.ipt_scaler = None
         else:
             raise ValueError(f"ipt_scaler_enum must be one of {ScalerEnum.__members__}")
         self.pszies_min = pszies_min
         self.psizes_max = psizes_max
         self.ipt_max = ipt_max
         self.ipt_min = ipt_min
         self._psizes_scaler_enum = psizes_scaler_enum
         self._ipt_scaler_enum = ipt_scaler_enum
 
-        if psizes_scaler_attrs is None and ipt_scaler_attrs is None:
-            self.needs_fitting = True
-        elif psizes_scaler_attrs is not None and ipt_scaler_attrs is not None:
+        if self.psizes_scaler and psizes_scaler_attrs is not None:
             set_scaler_attrs(scaler=self.psizes_scaler, scaler_attrs=psizes_scaler_attrs)
+        if self.ipt_scaler and ipt_scaler_attrs is not None:
             set_scaler_attrs(scaler=self.ipt_scaler, scaler_attrs=ipt_scaler_attrs)
-            self.needs_fitting = False
-        else:
-            raise ValueError("psizes_scaler_attrs and ipt_scaler_attrs must be both set or both None")
+        self.needs_fitting = (self.ipt_scaler and ipt_scaler_attrs is None) or (self.psizes_scaler and psizes_scaler_attrs is None)
 
     def forward(self, x_ppi: np.ndarray) -> np.ndarray:
         if self.needs_fitting:
             raise ValueError("Scalers need to be fitted before using the ClipAndScalePPI transform")
         x_ppi = x_ppi.transpose(0, 2, 1)
         orig_shape = x_ppi.shape
         ppi_channels = x_ppi.shape[-1]
         x_ppi = x_ppi.reshape(-1, ppi_channels)
-        x_ppi[:, IPT_POS] = x_ppi[:, IPT_POS].clip(max=self.ipt_max, min=self.ipt_min)
-        x_ppi[:, SIZE_POS] = x_ppi[:, SIZE_POS].clip(max=self.psizes_max, min=self.pszies_min)
-        padding_mask = x_ppi[:, DIR_POS] == 0 # Mask of zero padding
-        x_ppi[:, IPT_POS] = self.ipt_scaler.transform(x_ppi[:, IPT_POS].reshape(-1, 1)).reshape(-1) # type: ignore
-        x_ppi[:, SIZE_POS] = self.psizes_scaler.transform(x_ppi[:, SIZE_POS].reshape(-1, 1)).reshape(-1) # type: ignore
-        x_ppi[padding_mask, IPT_POS] = 0
-        x_ppi[padding_mask, SIZE_POS] = 0
+        x_ppi[:, PPI_IPT_POS] = x_ppi[:, PPI_IPT_POS].clip(max=self.ipt_max, min=self.ipt_min)
+        x_ppi[:, PPI_SIZE_POS] = x_ppi[:, PPI_SIZE_POS].clip(max=self.psizes_max, min=self.pszies_min)
+        padding_mask = x_ppi[:, PPI_DIR_POS] == 0 # Mask of zero padding
+        if self.ipt_scaler is not None:
+            x_ppi[:, PPI_IPT_POS] = self.ipt_scaler.transform(x_ppi[:, PPI_IPT_POS].reshape(-1, 1)).reshape(-1) # type: ignore
+        if self.psizes_scaler is not None:
+            x_ppi[:, PPI_SIZE_POS] = self.psizes_scaler.transform(x_ppi[:, PPI_SIZE_POS].reshape(-1, 1)).reshape(-1) # type: ignore
+        x_ppi[padding_mask, PPI_IPT_POS] = 0
+        x_ppi[padding_mask, PPI_SIZE_POS] = 0
         x_ppi = x_ppi.reshape(orig_shape).transpose(0, 2, 1)
         return x_ppi
-    
+
     def to_dict(self) -> dict:
         d = {
             "psizes_scaler_enum": str(self._psizes_scaler_enum),
-            "psizes_scaler_attrs": get_scaler_attrs(self.psizes_scaler),
+            "psizes_scaler_attrs": get_scaler_attrs(self.psizes_scaler) if self.psizes_scaler is not None else None,
             "pszies_min": self.pszies_min,
             "psizes_max": self.psizes_max,
             "ipt_scaler_enum": str(self._ipt_scaler_enum),
-            "ipt_scaler_attrs": get_scaler_attrs(self.ipt_scaler),
+            "ipt_scaler_attrs": get_scaler_attrs(self.ipt_scaler) if self.ipt_scaler is not None else None,
             "ipt_min": self.ipt_min,
             "ipt_max": self.ipt_max,
         }
         return d
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}(psizes_scaler={self._psizes_scaler_enum}, ipt_scaler={self._ipt_scaler_enum}, pszies_min={self.pszies_min}, psizes_max={self.psizes_max}, ipt_min={self.ipt_min}, ipt_max={self.ipt_max})"
@@ -203,15 +204,15 @@
         if flowstats_scaler_attrs is None and flowstats_quantiles is None:
             self.needs_fitting = True
         elif flowstats_scaler_attrs is not None and flowstats_quantiles is not None:
             set_scaler_attrs(scaler=self.flowstats_scaler, scaler_attrs=flowstats_scaler_attrs)
             self.flowstats_quantiles = flowstats_quantiles
             self.needs_fitting = False
         else:
-            raise ValueError("flowstats_quantiles and scaler_attrs must be both set or both None")
+            raise ValueError("flowstats_quantiles and flowstats_scaler_attrs must be both set or both None")
 
     def forward(self, x_flowstats: np.ndarray) -> np.ndarray:
         if self.needs_fitting:
             raise ValueError("Scalers and quantiles need to be fitted before using this transform")
         x_flowstats = x_flowstats.clip(min=0, max=self.flowstats_quantiles)
         x_flowstats = self.flowstats_scaler.transform(x_flowstats) # type: ignore
         return x_flowstats
@@ -235,19 +236,20 @@
 
     Expected format of input packet histograms: `(batch_size, 4 * PHIST_BIN_COUNT)`.
     The input histograms are expected to be in the following order: source packet sizes, destination packet sizes, source inter-packet times, and destination inter-packet times.
     Each of the four histograms is expected to have `PHIST_BIN_COUNT` bins, which is 8 in the current implementation.
     """
     def __init__(self) -> None:
         super().__init__()
+        self.bins = PHIST_BIN_COUNT
 
     def forward(self, x_flowstats_phist: np.ndarray) -> np.ndarray:
-        src_sizes_pkt_count = x_flowstats_phist[:, :PHIST_BIN_COUNT].sum(axis=1)[:, np.newaxis]
-        dst_sizes_pkt_count = x_flowstats_phist[:, PHIST_BIN_COUNT:(2*PHIST_BIN_COUNT)].sum(axis=1)[:, np.newaxis]
-        np.divide(x_flowstats_phist[:, :PHIST_BIN_COUNT], src_sizes_pkt_count, out=x_flowstats_phist[:, :PHIST_BIN_COUNT], where=src_sizes_pkt_count != 0)
-        np.divide(x_flowstats_phist[:, PHIST_BIN_COUNT:(2*PHIST_BIN_COUNT)], dst_sizes_pkt_count, out=x_flowstats_phist[:, PHIST_BIN_COUNT:(2*PHIST_BIN_COUNT)], where=dst_sizes_pkt_count != 0)
-        np.divide(x_flowstats_phist[:, (2*PHIST_BIN_COUNT):(3*PHIST_BIN_COUNT)], src_sizes_pkt_count - 1, out=x_flowstats_phist[:, (2*PHIST_BIN_COUNT):(3*PHIST_BIN_COUNT)], where=src_sizes_pkt_count > 1)
-        np.divide(x_flowstats_phist[:, (3*PHIST_BIN_COUNT):(4*PHIST_BIN_COUNT)], dst_sizes_pkt_count - 1, out=x_flowstats_phist[:, (3*PHIST_BIN_COUNT):(4*PHIST_BIN_COUNT)], where=dst_sizes_pkt_count > 1)
+        src_sizes_pkt_count = x_flowstats_phist[:, :self.bins].sum(axis=1)[:, np.newaxis]
+        dst_sizes_pkt_count = x_flowstats_phist[:, self.bins:(2*self.bins)].sum(axis=1)[:, np.newaxis]
+        np.divide(x_flowstats_phist[:, :self.bins], src_sizes_pkt_count, out=x_flowstats_phist[:, :self.bins], where=src_sizes_pkt_count != 0)
+        np.divide(x_flowstats_phist[:, self.bins:(2*self.bins)], dst_sizes_pkt_count, out=x_flowstats_phist[:, self.bins:(2*self.bins)], where=dst_sizes_pkt_count != 0)
+        np.divide(x_flowstats_phist[:, (2*self.bins):(3*self.bins)], src_sizes_pkt_count - 1, out=x_flowstats_phist[:, (2*self.bins):(3*self.bins)], where=src_sizes_pkt_count > 1)
+        np.divide(x_flowstats_phist[:, (3*self.bins):(4*self.bins)], dst_sizes_pkt_count - 1, out=x_flowstats_phist[:, (3*self.bins):(4*self.bins)], where=dst_sizes_pkt_count > 1)
         return x_flowstats_phist
 
     def __repr__(self) -> str:
         return f"{self.__class__.__name__}()"
```

### Comparing `cesnet-models-0.1.1/cesnet_models.egg-info/PKG-INFO` & `cesnet_models-0.1.2/cesnet_models.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cesnet-models
-Version: 0.1.1
+Version: 0.1.2
 Summary: Pre-trained neural networks for encrypted traffic classification
 Author-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 Maintainer-email: Jan Luxemburk <luxemburk@cesnet.cz>, Karel Hynek <hynekkar@cesnet.cz>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/CESNET/cesnet-models
 Project-URL: Documentation, https://cesnet.github.io/cesnet-models/
 Project-URL: Bug Tracker, https://github.com/CESNET/cesnet-models/issues
@@ -35,19 +35,19 @@
 
 [![](https://img.shields.io/badge/license-BSD-blue.svg)](https://github.com/CESNET/cesnet-models/blob/main/LICENCE)
 [![](https://img.shields.io/badge/docs-cesnet--models-blue.svg)](https://cesnet.github.io/cesnet-models/)
 [![](https://img.shields.io/badge/python->=3.10-blue.svg)](https://pypi.org/project/cesnet-models/)
 [![](https://img.shields.io/pypi/v/cesnet-models)](https://pypi.org/project/cesnet-models/)
 
 
-The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights. The weights were trained using public datasets available in the [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) package.
+The goal of this project is to provide neural network architectures for traffic classification and their pre-trained weights.
 
 The newest network architecture is named Multi-modal CESNET v2 (mm-CESNET-v2) and is visualized in the following picture. See the [getting started](https://cesnet.github.io/cesnet-models/getting_started/) page and [models](https://cesnet.github.io/cesnet-models/reference_models/) reference for more information.
 
-:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing three large network traffic datasets. :frog: :frog:
+:frog: :frog: See a related project [CESNET DataZoo](https://github.com/CESNET/cesnet-datazoo) providing large TLS and QUIC traffic datasets. :frog: :frog:
 
 :notebook: :notebook: Example Jupyter notebooks are included in a separate [CESNET Traffic Classification Examples](https://github.com/CESNET/cesnet-tcexamples) repo. :notebook: :notebook:
 
 ### Multi-modal CESNET v2
 <p align="center">
     <img src="https://raw.githubusercontent.com/CESNET/cesnet-models/main/docs/images/model-mm-cesnet-v2.png" width="450">
 </p>
@@ -61,7 +61,19 @@
 ```
 
 or for editable install with:
 
 ```bash
 pip install -e git+https://github.com/CESNET/cesnet-models
 ```
+
+## Papers
+
+Models from the following papers are included:
+
+* [Fine-grained TLS services classification with reject option](https://doi.org/10.1016/j.comnet.2022.109467) <br>
+Jan Luxemburk and Tomáš Čejka <br>
+Computer Networks, 2023
+
+* [Encrypted traffic classification: the QUIC case](https://doi.org/10.23919/TMA58422.2023.10199052) <br>
+Jan Luxemburk and Karel Hynek <br>
+2023 7th Network Traffic Measurement and Analysis Conference (TMA)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `cesnet-models-0.1.1/pyproject.toml` & `cesnet_models-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cesnet-models"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
 ]
 maintainers = [
   {name = "Jan Luxemburk", email = "luxemburk@cesnet.cz"},
   {name = "Karel Hynek", email = "hynekkar@cesnet.cz"},
```

