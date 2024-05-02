# Comparing `tmp/infini_transformer_pytorch-0.0.7.tar.gz` & `tmp/infini_transformer_pytorch-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.7.tar", last modified: Thu May  2 14:17:27 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.0.8.tar", last modified: Thu May  2 16:29:45 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.7.tar` & `infini_transformer_pytorch-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/infini_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 16:29:45.000000 infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 16:29:45.349289 infini_transformer_pytorch-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 16:29:41.000000 infini_transformer_pytorch-0.0.8/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.7/LICENSE` & `infini_transformer_pytorch-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.7/PKG-INFO` & `infini_transformer_pytorch-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.7/README.md` & `infini_transformer_pytorch-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.0.8/infini_transformer_pytorch/infini_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,14 +18,20 @@
 
 def exists(v):
     return v
 
 def default(v, d):
     return v if exists(v) else d
 
+def detach_memories_(memories: Memories):
+    if detach_memories:
+        for (mem_kv, mem_norm) in memories:
+            mem_kv.detach_()
+            mem_norm.detach_()
+
 # classes
 
 class RMSNorm(Module):
     def __init__(self, dim):
         super().__init__()
         self.scale = dim ** 0.5
         self.gamma = nn.Parameter(torch.ones(dim))
@@ -251,12 +257,10 @@
 
         logits = self.to_logits(embed)
 
         if not return_memories:
             return logits
 
         if detach_memories:
-            for (mem_kv, mem_norm) in new_memories:
-                mem_kv.detach_()
-                mem_norm.detach_()
+            detach_memories_(new_memories)
 
         return logits, new_memories
```

### Comparing `infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.0.8/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.7
+Version: 0.0.8
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.7/setup.py` & `infini_transformer_pytorch-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.7',
+  version = '0.0.8',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
```

