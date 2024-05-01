# Comparing `tmp/magvit2-pytorch-0.4.0.tar.gz` & `tmp/magvit2_pytorch-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magvit2-pytorch-0.4.0.tar", last modified: Thu Jan 18 16:14:07 2024, max compression
+gzip compressed data, was "magvit2_pytorch-0.4.1.tar", last modified: Wed May  1 23:11:17 2024, max compression
```

## Comparing `magvit2-pytorch-0.4.0.tar` & `magvit2_pytorch-0.4.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:14:07.069565 magvit2-pytorch-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-18 16:14:07.069565 magvit2-pytorch-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:14:07.065565 magvit2-pytorch-0.4.0/magvit2_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/magvit2_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/optimizer.py
--rw-r--r--   0 runner    (1001) docker     (127)    16703 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/trainer.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/magvit2_pytorch/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-18 16:14:07.069565 magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-01-18 16:14:07.000000 magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-18 16:14:07.000000 magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-18 16:14:07.000000 magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-01-18 16:14:07.000000 magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-18 16:14:07.000000 magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-18 16:14:07.069565 magvit2-pytorch-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-01-18 16:13:58.000000 magvit2-pytorch-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6561 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:11:17.403495 magvit2_pytorch-0.4.1/magvit2_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8412 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56410 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/magvit2_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16704 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/magvit2_pytorch/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-01 23:11:17.000000 magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:11:17.407495 magvit2_pytorch-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-01 23:11:13.000000 magvit2_pytorch-0.4.1/setup.py
```

### Comparing `magvit2-pytorch-0.4.0/LICENSE` & `magvit2_pytorch-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `magvit2-pytorch-0.4.0/PKG-INFO` & `magvit2_pytorch-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `magvit2-pytorch-0.4.0/README.md` & `magvit2_pytorch-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `magvit2-pytorch-0.4.0/magvit2_pytorch/attend.py` & `magvit2_pytorch-0.4.1/magvit2_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `magvit2-pytorch-0.4.0/magvit2_pytorch/data.py` & `magvit2_pytorch-0.4.1/magvit2_pytorch/data.py`

 * *Files identical despite different names*

### Comparing `magvit2-pytorch-0.4.0/magvit2_pytorch/magvit2_pytorch.py` & `magvit2_pytorch-0.4.1/magvit2_pytorch/magvit2_pytorch.py`

 * *Files identical despite different names*

### Comparing `magvit2-pytorch-0.4.0/magvit2_pytorch/optimizer.py` & `magvit2_pytorch-0.4.1/magvit2_pytorch/optimizer.py`

 * *Files identical despite different names*

### Comparing `magvit2-pytorch-0.4.0/magvit2_pytorch/trainer.py` & `magvit2_pytorch-0.4.1/magvit2_pytorch/trainer.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,16 @@
 
         self.num_train_steps = num_train_steps
         self.grad_accum_every = grad_accum_every
         self.max_grad_norm = max_grad_norm
 
         self.apply_gradient_penalty_every = apply_gradient_penalty_every
 
+        self.has_multiscale_discrs = self.model.has_multiscale_discrs
+
         # prepare for maybe distributed
 
         (
             self.model,
             self.dataloader,
             self.optimizer,
             self.discr_optimizer
@@ -196,15 +198,14 @@
 
         # only use adversarial training after a certain number of steps
 
         self.discr_start_after_step = discr_start_after_step
 
         # multiscale discr losses
 
-        self.has_multiscale_discrs = self.model.has_multiscale_discrs
         self.multiscale_discr_optimizers = []
 
         for ind, discr in enumerate(self.model.multiscale_discrs):
             multiscale_optimizer = get_optimizer(discr.parameters(), lr = learning_rate, **optimizer_kwargs)
 
             self.multiscale_discr_optimizers.append(multiscale_optimizer)
```

### Comparing `magvit2-pytorch-0.4.0/magvit2_pytorch.egg-info/PKG-INFO` & `magvit2_pytorch-0.4.1/magvit2_pytorch.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: magvit2-pytorch
-Version: 0.4.0
+Version: 0.4.1
 Summary: MagViT2 - Pytorch
 Home-page: https://github.com/lucidrains/magvit2-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformer,attention mechanisms,generative video model
 Classifier: Development Status :: 4 - Beta
```

### Comparing `magvit2-pytorch-0.4.0/setup.py` & `magvit2_pytorch-0.4.1/setup.py`

 * *Files identical despite different names*

