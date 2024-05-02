# Comparing `tmp/infini_transformer_pytorch-0.0.6.tar.gz` & `tmp/infini_transformer_pytorch-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infini_transformer_pytorch-0.0.6.tar", last modified: Thu May  2 14:07:57 2024, max compression
+gzip compressed data, was "infini_transformer_pytorch-0.0.7.tar", last modified: Thu May  2 14:17:27 2024, max compression
```

## Comparing `infini_transformer_pytorch-0.0.6.tar` & `infini_transformer_pytorch-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:07:57.388857 infini_transformer_pytorch-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 14:07:53.000000 infini_transformer_pytorch-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:07:57.388857 infini_transformer_pytorch-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 14:07:53.000000 infini_transformer_pytorch-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:07:57.384857 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 14:07:53.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-05-02 14:07:53.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch/infini_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:07:57.388857 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:07:57.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 14:07:57.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:07:57.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 14:07:57.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 14:07:57.000000 infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:07:57.388857 infini_transformer_pytorch-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 14:07:53.000000 infini_transformer_pytorch-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/infini_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-02 14:17:27.000000 infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 14:17:27.627999 infini_transformer_pytorch-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-02 14:17:22.000000 infini_transformer_pytorch-0.0.7/setup.py
```

### Comparing `infini_transformer_pytorch-0.0.6/LICENSE` & `infini_transformer_pytorch-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.6/PKG-INFO` & `infini_transformer_pytorch-0.0.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.6/README.md` & `infini_transformer_pytorch-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `infini_transformer_pytorch-0.0.6/infini_transformer_pytorch/infini_transformer.py` & `infini_transformer_pytorch-0.0.7/infini_transformer_pytorch/infini_transformer.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,15 +54,16 @@
     def __init__(
         self,
         dim,
         *,
         dim_head = 128,
         heads = 8,
         head_gate_init_value = 10.,
-        use_mem_delta_rule = False
+        use_mem_delta_rule = False,
+        rotary_emb_linear_attn = False    # unsure whether to apply rotary embeddings to linear attention, so make it an option
     ):
         super().__init__()
         dim_inner = dim_head * heads
         self.scale = dim_head ** -0.5
         self.norm = RMSNorm(dim)
 
         self.rotary_emb = RotaryEmbedding(dim_head)
@@ -72,14 +73,15 @@
 
         self.split_heads = Rearrange('b n (qkv h d) -> qkv b h n d', qkv = 3, h = heads)
         self.merge_heads = Rearrange('b h n d -> b n (h d)')
 
         self.head_gates = nn.Parameter(torch.ones(heads) * head_gate_init_value)
 
         self.use_mem_delta_rule = use_mem_delta_rule
+        self.rotary_emb_linear_attn = rotary_emb_linear_attn
 
     def forward(
         self,
         x,
         past_memories: Optional[Memories] = None,
         eps = 1e-10
     ) -> Tuple[Tensor, Memories]:
@@ -126,14 +128,19 @@
         # the main contribution of the paper
         # Katharopoulos linear attention to kv memory of shape (batch, heads, dim keys, dim values)
         # it makes sense the author would try this, as he is ex-shmidhuber lab (linear transformers are fast weights paper)
 
         q = F.elu(q) + 1
         k = F.elu(k) + 1
 
+        # maybe apply rotary embeddings to q, k for linear attention to past
+
+        if self.rotary_emb_linear_attn:
+            q, k = map(self.rotary_emb.rotate_queries_or_keys, (q, k))
+
         # retrieve from past memories
 
         def retrieve_from_kv_memories(t, past_memories: Memories):
             past_memories_kv, past_memories_norm = past_memories
 
             numer = einsum(t, past_memories_kv, 'b h n dk, b h dk dv -> b h n dv')
             denom = einsum(t, past_memories_norm, 'b h n d, b h d -> b h n')
@@ -186,29 +193,31 @@
         *,
         num_tokens,
         dim,
         depth,
         dim_head = 128,
         heads = 8,
         ff_mult = 4,
-        use_mem_delta_rule = False  # in the paper, the delta rule didn't seem to do that much, but will include for completeness
+        use_mem_delta_rule = False,     # in the paper, the delta rule didn't seem to do that much, but will include for completeness
+        rotary_emb_linear_attn = False
     ):
         super().__init__()
 
         self.token_emb = nn.Embedding(num_tokens, dim)
 
         self.layers = ModuleList([])
 
         for _ in range(depth):
 
             attn = CausalAttention(
                 dim = dim,
                 dim_head = dim_head,
                 heads = heads,
-                use_mem_delta_rule = use_mem_delta_rule
+                use_mem_delta_rule = use_mem_delta_rule,
+                rotary_emb_linear_attn = rotary_emb_linear_attn
             )
 
             ff = FeedForward(
                 dim = dim,
                 mult = ff_mult
             )
```

### Comparing `infini_transformer_pytorch-0.0.6/infini_transformer_pytorch.egg-info/PKG-INFO` & `infini_transformer_pytorch-0.0.7/infini_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: infini-transformer-pytorch
-Version: 0.0.6
+Version: 0.0.7
 Summary: Infini-Transformer in Pytorch
 Home-page: https://github.com/lucidrains/infini-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,long context,memory
 Classifier: Development Status :: 4 - Beta
```

### Comparing `infini_transformer_pytorch-0.0.6/setup.py` & `infini_transformer_pytorch-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'infini-transformer-pytorch',
   packages = find_packages(exclude = []),
-  version = '0.0.6',
+  version = '0.0.7',
   license='MIT',
   description = 'Infini-Transformer in Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/infini-transformer-pytorch',
   keywords = [
```

