# Comparing `tmp/infini_transformer_pytorch-0.0.3.tar.gz` & `tmp/infini_transformer_pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.3.tar", last modified: Wed May  1 21:15:04 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.0.4.tar", last modified: Wed May  1 21:16:21 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.3.tar` & `infini_transformer_pytorch-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:04.493473 infini_transformer_pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 21:15:00.000000 infini_transformer_pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:15:04.493473 infini_transformer_pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 21:15:00.000000 infini_transformer_pytorch-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:04.489473 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 21:15:00.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2024-05-01 21:15:00.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:15:04.493473 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:15:04.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 21:15:04.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:15:04.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 21:15:04.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 21:15:04.000000 infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:15:04.493473 infini_transformer_pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 21:15:00.000000 infini_transformer_pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:21.231561 infini_transformer_pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:16:21.227561 infini_transformer_pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:21.227561 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/infini_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:21.227561 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:16:21.231561 infini_transformer_pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.3/LICENSE` & `infini_transformer_pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.3/PKG-INFO` & `infini_transformer_pytorch-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.3/README.md` & `infini_transformer_pytorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.3/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/infini_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,19 +97,18 @@
         """
 
         x = self.norm(x)
 
         x = self.to_qkv(x)
         q, k, v = self.split_heads(x)
 
-        q = q * self.scale
-
         # similarity
 
-        q_rotated = self.rotary_emb.rotate_queries_or_keys(q)
+        q_scaled = q * self.scale
+        q_rotated = self.rotary_emb.rotate_queries_or_keys(q_scaled)
         k_rotated = self.rotary_emb.rotate_queries_or_keys(k)
 
         sim = einsum(q_rotated, k_rotated, '... i d, ... j d -> ... i j')
 
         # causal mask
 
         i, j = sim.shape[-2:]
```

### Comparing `infini_transformer_pytorch-0.0.3/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.3/setup.py` & `infini_transformer_pytorch-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
```

