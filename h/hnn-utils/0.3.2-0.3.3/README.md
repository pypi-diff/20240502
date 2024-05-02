# Comparing `tmp/hnn_utils-0.3.2.tar.gz` & `tmp/hnn_utils-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hnn_utils-0.3.2.tar", max compression
+gzip compressed data, was "hnn_utils-0.3.3.tar", max compression
```

## Comparing `hnn_utils-0.3.2.tar` & `hnn_utils-0.3.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1068 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/LICENSE
--rw-r--r--   0        0        0      137 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/README.md
--rw-r--r--   0        0        0        0 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/__init__.py
--rw-r--r--   0        0        0       48 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/callbacks/__init__.py
--rw-r--r--   0        0        0     6566 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/callbacks/ema.py
--rw-r--r--   0        0        0      178 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/__init__.py
--rw-r--r--   0        0        0     2219 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/guacamol.py
--rw-r--r--   0        0        0     3119 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/utils.py
--rw-r--r--   0        0        0     1730 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac.json
--rw-r--r--   0        0        0     1843 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac_random.json
--rw-r--r--   0        0        0     5297 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/vocab/zinc20.json
--rw-r--r--   0        0        0     3133 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/datasets/zinc.py
--rw-r--r--   0        0        0     1370 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/ALiBi.py
--rw-r--r--   0        0        0     1677 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/RotaryEmbedding.py
--rw-r--r--   0        0        0    14366 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/Transformer.py
--rw-r--r--   0        0        0      164 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/__init__.py
--rw-r--r--   0        0        0     1247 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/ffn.py
--rw-r--r--   0        0        0     2000 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/functional.py
--rw-r--r--   0        0        0      800 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/hnn_utils/nn/normalization.py
--rw-r--r--   0        0        0      516 2024-04-30 14:27:37.916646 hnn_utils-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 hnn_utils-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/LICENSE
+-rw-r--r--   0        0        0      137 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/__init__.py
+-rw-r--r--   0        0        0       48 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/callbacks/__init__.py
+-rw-r--r--   0        0        0     6566 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/callbacks/ema.py
+-rw-r--r--   0        0        0      178 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/__init__.py
+-rw-r--r--   0        0        0     2219 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/guacamol.py
+-rw-r--r--   0        0        0     3119 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/utils.py
+-rw-r--r--   0        0        0     1730 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/vocab/guac.json
+-rw-r--r--   0        0        0     1843 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/vocab/guac_random.json
+-rw-r--r--   0        0        0     5297 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/vocab/zinc20.json
+-rw-r--r--   0        0        0     3133 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/datasets/zinc.py
+-rw-r--r--   0        0        0     1370 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/ALiBi.py
+-rw-r--r--   0        0        0     1677 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/RotaryEmbedding.py
+-rw-r--r--   0        0        0    15836 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/Transformer.py
+-rw-r--r--   0        0        0      164 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/__init__.py
+-rw-r--r--   0        0        0     1247 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/ffn.py
+-rw-r--r--   0        0        0     2000 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/functional.py
+-rw-r--r--   0        0        0      800 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/hnn_utils/nn/normalization.py
+-rw-r--r--   0        0        0      516 2024-05-02 14:26:03.177676 hnn_utils-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      803 1970-01-01 00:00:00.000000 hnn_utils-0.3.3/PKG-INFO
```

### Comparing `hnn_utils-0.3.2/LICENSE` & `hnn_utils-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/callbacks/ema.py` & `hnn_utils-0.3.3/hnn_utils/callbacks/ema.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/datasets/guacamol.py` & `hnn_utils-0.3.3/hnn_utils/datasets/guacamol.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/datasets/utils.py` & `hnn_utils-0.3.3/hnn_utils/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac.json` & `hnn_utils-0.3.3/hnn_utils/datasets/vocab/guac.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/datasets/vocab/guac_random.json` & `hnn_utils-0.3.3/hnn_utils/datasets/vocab/guac_random.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/datasets/vocab/zinc20.json` & `hnn_utils-0.3.3/hnn_utils/datasets/vocab/zinc20.json`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/datasets/zinc.py` & `hnn_utils-0.3.3/hnn_utils/datasets/zinc.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/nn/ALiBi.py` & `hnn_utils-0.3.3/hnn_utils/nn/ALiBi.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/nn/RotaryEmbedding.py` & `hnn_utils-0.3.3/hnn_utils/nn/RotaryEmbedding.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/nn/Transformer.py` & `hnn_utils-0.3.3/hnn_utils/nn/Transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 from einops import rearrange
 from torch import Tensor
 
 from hnn_utils.nn.ALiBi import ALiBi
-from hnn_utils.nn.normalization import LayerNorm
 from hnn_utils.nn.ffn import FFNSwiGLU
+from hnn_utils.nn.normalization import LayerNorm
 
 try:
     from flash_attn import flash_attn_kvpacked_func, flash_attn_qkvpacked_func
 
     FLASH_AVAILABLE = True
 except ImportError as e:
     print("Flash not available, using PyTorch implementation: ", e)
@@ -291,39 +291,61 @@
         self,
         query: Tensor,
         kv: Tensor,
         pad_mask: Optional[Tensor] = None,
         attn_mask: Optional[Tensor] = None,
         is_causal: bool = False,
     ) -> Tensor:
+        assert not is_causal or (
+            pad_mask is None and attn_mask is None
+        ), "is_causal not supported with padding or attention masks."
+
         if can_flash(query, pad_mask, attn_mask):
             return self.flash_forward(query, kv, is_causal)
+        else:
+            return self.torch_forward(query, kv, pad_mask, attn_mask, is_causal)
 
+    def torch_forward(
+        self,
+        query: Tensor,
+        kv: Tensor,
+        pad_mask: Optional[Tensor] = None,
+        attn_mask: Optional[Tensor] = None,
+        is_causal: bool = False,
+    ) -> Tensor:
         q = self.q_proj(query)
         k, v = self.kv_proj(kv).chunk(2, dim=-1)
 
         q = rearrange(q, "... n (h d) -> ... h n d", h=self.num_heads)
         k = rearrange(k, "... n (h d) -> ... h n d", h=self.num_heads)
         v = rearrange(v, "... n (h d) -> ... h n d", h=self.num_heads)
 
         mask = combine_masks(attn_mask, pad_mask, self.num_heads, query.dtype)
 
         if hasattr(self, "alibi"):
             bias = self.alibi(q, k)
             mask = mask + bias if mask is not None else bias
 
+        if is_causal:
+            cm = causal_mask(query)
+            mask = mask + cm if mask is not None else cm
+
         dropout = self.dropout if self.training else 0.0
-        attn = F.scaled_dot_product_attention(
-            q, k, v, mask, is_causal=is_causal, dropout_p=dropout
-        )
+        attn = F.scaled_dot_product_attention(q, k, v, mask, dropout_p=dropout)
 
         attn = rearrange(attn, "... h n d -> ... n (h d)")
         return self.out_proj(attn)
 
     def flash_forward(self, query: Tensor, kv: Tensor, is_causal: bool) -> Tensor:
+        qshape, kvshape = query.shape, kv.shape
+        qseq_dims, kvseq_dims = qshape[-2:], kvshape[-2:]
+
+        query = query.reshape(-1, *qseq_dims)
+        kv = kv.reshape(-1, *kvseq_dims)
+
         q = self.q_proj(query)
         kv = self.kv_proj(kv)
 
         q = rearrange(q, "... (h d) -> ... h d", h=self.num_heads)
         kv = rearrange(kv, "... (n h d) -> ... n h d", h=self.num_heads, n=2)
 
         slopes = self.alibi.slopes.float().squeeze() if hasattr(self, "alibi") else None
@@ -334,15 +356,15 @@
             q=q.bfloat16(),
             kv=kv.bfloat16(),
             causal=is_causal,
             alibi_slopes=slopes,
         ).type(dtype)
 
         attn = rearrange(attn, "... h d -> ... (h d)")
-        return self.out_proj(attn)
+        return self.out_proj(attn).reshape(qshape)
 
 
 class SelfAttention(nn.Module):
     def __init__(
         self,
         embed_dim: int,
         heads: int,
@@ -370,53 +392,72 @@
     def forward(
         self,
         x: Tensor,
         pad_mask: Optional[Tensor] = None,
         attn_mask: Optional[Tensor] = None,
         is_causal: bool = False,
     ) -> Tensor:
+        assert not is_causal or (
+            pad_mask is None and attn_mask is None
+        ), "is_causal not supported with padding or attention masks."
+
         if can_flash(x, pad_mask, attn_mask):
             return self.flash_forward(x, is_causal)
+        else:
+            return self.torch_forward(x, pad_mask, attn_mask, is_causal)
 
+    def torch_forward(
+        self,
+        x: Tensor,
+        pad_mask: Optional[Tensor] = None,
+        attn_mask: Optional[Tensor] = None,
+        is_causal: bool = False,
+    ) -> Tensor:
         q, k, v = self.qkv_proj(x).chunk(3, dim=-1)
 
         q = rearrange(q, "... n (h d) -> ... h n d", h=self.num_heads)
         k = rearrange(k, "... n (h d) -> ... h n d", h=self.num_heads)
         v = rearrange(v, "... n (h d) -> ... h n d", h=self.num_heads)
 
         mask = combine_masks(attn_mask, pad_mask, self.num_heads, q.dtype)
 
         if hasattr(self, "alibi"):
             bias = self.alibi(q, k)
             mask = mask + bias if mask is not None else bias
 
+        if is_causal:
+            cm = causal_mask(x)
+            mask = mask + cm if mask is not None else cm
+
         dropout = self.dropout if self.training else 0.0
-        attn = F.scaled_dot_product_attention(
-            q, k, v, mask, is_causal=is_causal, dropout_p=dropout
-        )
+        attn = F.scaled_dot_product_attention(q, k, v, mask, dropout_p=dropout)
 
         attn = rearrange(attn, "... h n d -> ... n (h d)")
         return self.out_proj(attn)
 
     def flash_forward(self, x: Tensor, is_causal: bool) -> Tensor:
+        shape = x.shape
+        seq_dims = shape[-2:]
+        x = x.reshape(-1, *seq_dims)
+
         qkv = self.qkv_proj(x)
         qkv = rearrange(qkv, "... (n h d) -> ... n h d", h=self.num_heads, n=3)
 
         slopes = None
         if hasattr(self, "alibi"):
             slopes = self.alibi.slopes.float().squeeze()
 
         dtype = x.dtype
 
         attn = flash_attn_qkvpacked_func(
             qkv=qkv.bfloat16(), causal=is_causal, alibi_slopes=slopes
         ).type(dtype)
 
         attn = rearrange(attn, "... h d -> ... (h d)")
-        return self.out_proj(attn)
+        return self.out_proj(attn).reshape(shape)
 
 
 def combine_masks(
     attn_mask: Optional[Tensor],
     pad_mask: Optional[Tensor],
     heads: int = 1,
     dtype: Optional[torch.dtype] = None,
@@ -449,25 +490,27 @@
         nn.init.xavier_uniform_(mod.weight)
         if mod.bias is not None:
             nn.init.zeros_(mod.bias)
 
 
 def causal_mask(embed: Tensor) -> Tensor:
     """
-    Creates a causal mask for self-attention.
+    Creates a causal mask for self-attention. Expects sequence length to be the 2nd to last dimension.
     """
-    mask = torch.full((embed.shape[1], embed.shape[1]), -torch.inf, device=embed.device, dtype=embed.dtype)  # fmt: skip
+    # Sequence length is 2nd to last dimension
+    SL = embed.shape[-2]
+    mask = torch.full((SL, SL), -torch.inf, device=embed.device, dtype=embed.dtype)  # fmt: skip
     mask = torch.triu(mask, diagonal=1)
     return mask
 
 
 def can_flash(
     x: Tensor,
     pad_mask: Optional[Tensor] = None,
     attn_mask: Optional[Tensor] = None,
 ):
     return (
         pad_mask is None
         and attn_mask is None
         and FLASH_AVAILABLE
-        and x.device.type == "gpu"
+        and x.device.type == "cuda"
     )
```

### Comparing `hnn_utils-0.3.2/hnn_utils/nn/ffn.py` & `hnn_utils-0.3.3/hnn_utils/nn/ffn.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/nn/functional.py` & `hnn_utils-0.3.3/hnn_utils/nn/functional.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/hnn_utils/nn/normalization.py` & `hnn_utils-0.3.3/hnn_utils/nn/normalization.py`

 * *Files identical despite different names*

### Comparing `hnn_utils-0.3.2/pyproject.toml` & `hnn_utils-0.3.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hnn_utils"
-version = "0.3.2"
+version = "0.3.3"
 description = "Various utilities used throughout my research"
 authors = ["Haydn Jones <haydnjonest@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "hnn_utils" }]
 
 include = ["hnn_utils/datasets/vocab/*.json"]
```

### Comparing `hnn_utils-0.3.2/PKG-INFO` & `hnn_utils-0.3.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hnn_utils
-Version: 0.3.2
+Version: 0.3.3
 Summary: Various utilities used throughout my research
 Author: Haydn Jones
 Author-email: haydnjonest@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

