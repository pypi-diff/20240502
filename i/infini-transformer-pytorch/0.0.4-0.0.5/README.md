# Comparing `tmp/infini_transformer_pytorch-0.0.4.tar.gz` & `tmp/infini_transformer_pytorch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.4.tar", last modified: Wed May  1 21:16:21 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.0.5.tar", last modified: Thu May  2 14:04:46 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.4.tar` & `infini_transformer_pytorch-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:21.231561 infini_transformer_pytorch-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:16:21.227561 infini_transformer_pytorch-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:21.227561 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 21:16:21.227561 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-01 21:16:21.000000 infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 21:16:21.231561 infini_transformer_pytorch-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-01 21:16:14.000000 infini_transformer_pytorch-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:04:46.976706 infini_transformer_pytorch-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 14:04:43.000000 infini_transformer_pytorch-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:04:46.976706 infini_transformer_pytorch-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 14:04:43.000000 infini_transformer_pytorch-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:04:46.972706 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 14:04:43.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-05-02 14:04:43.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch/infini_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:04:46.976706 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:04:46.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 14:04:46.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:04:46.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 14:04:46.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 14:04:46.000000 infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:04:46.976706 infini_transformer_pytorch-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 14:04:43.000000 infini_transformer_pytorch-0.0.5/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.4/LICENSE` & `infini_transformer_pytorch-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.4/PKG-INFO` & `infini_transformer_pytorch-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.4/README.md` & `infini_transformer_pytorch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.4/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.0.5/infini_transformer_pytorch/infini_transformer.py`

 * *Files 9% similar despite different names*

```diff
@@ -128,41 +128,39 @@
         # it makes sense the author would try this, as he is ex-shmidhuber lab (linear transformers are fast weights paper)
 
         q = F.elu(q) + 1
         k = F.elu(k) + 1
 
         # retrieve from past memories if present
 
-        if exists(past_memories):
-            past_memories_kv, past_memories_norm = past_memories
+        def retrieve_from_kv_memories(t, kv, z_norm):
+            numer = einsum(t, past_memories_kv, 'b h n dk, b h dk dv -> b h n dv')
+            denom = einsum(t, past_memories_norm, 'b h n d, b h d -> b h n')
 
-            mem_out_unnormed = einsum(q, past_memories_kv, 'b h n dk, b h dk dv -> b h n dv')
-            mem_norm = einsum(q, past_memories_norm, 'b h n d, b h d -> b h n')
+            denom = rearrange(denom, '... -> ... 1')
+            return numer / denom.clamp(min = eps) # eq (3)
 
-            mem_norm = rearrange(mem_norm, '... -> ... 1')
-            mem_out = mem_out_unnormed / mem_norm.clamp(min = eps) # eq (3)
+        if exists(past_memories):
+            past_memories_kv, past_memories_norm = past_memories
+            mem_out = retrieve_from_kv_memories(q, past_memories_kv, past_memories_norm)
 
             # now combine the present output of queries with the outputs querying the past compressed key/value memories
             # in paper, they use a sigmoid gating scheme with learned gate per head
 
             gates = rearrange(self.head_gates, 'h -> h 1 1')
             gates = gates.sigmoid()
 
             out = out * gates + mem_out * (1. - gates)  # eq (6)
 
         # create the next memories
 
         if exists(past_memories) and self.use_mem_delta_rule:
-            # eq (5) - the delta rule
-            v_unnormed = einsum(k, past_memories_kv, 'b h n dk, b h dk dv -> b h n dv')
-            v_norm = einsum(k, past_memories_norm, 'b h n d, b h d -> b h n')
-
-            v_norm = rearrange(v_norm, '... -> ... 1')
-            delta_v = v_unnormed / v_norm.clamp(min = eps)
+            delta_v = retrieve_from_kv_memories(k, past_memories_kv, past_memories_norm)
 
+            # eq (5) - the delta rule
             v = v - delta_v
 
         new_memories_kv = einsum(k, v, '... n dk, ... n dv -> ... dk dv')
         new_memories_norm = reduce(k, 'b h n d -> b h d', 'sum')
 
         if exists(past_memories):
             new_memories_kv = new_memories_kv + past_memories_kv          # eq (4)
```

### Comparing `infini_transformer_pytorch-0.0.4/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.0.5/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.4
+Version: 0.0.5
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.4/setup.py` & `infini_transformer_pytorch-0.0.5/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.4',
+  version = '0.0.5',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
```

