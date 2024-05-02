# Comparing `tmp/torch_sparse_tensor-0.1.1.tar.gz` & `tmp/torch_sparse_tensor-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_sparse_tensor-0.1.1.tar", max compression
+gzip compressed data, was "torch_sparse_tensor-0.2.0.tar", max compression
```

## Comparing `torch_sparse_tensor-0.1.1.tar` & `torch_sparse_tensor-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1517 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/README.md
--rw-r--r--   0        0        0      550 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       83 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/__init__.py
--rw-r--r--   0        0        0     7203 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/base.py
--rw-r--r--   0        0        0     3647 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/cat.py
--rw-r--r--   0        0        0      456 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/indexing.py
--rw-r--r--   0        0        0      513 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/mask.py
--rw-r--r--   0        0        0     8257 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/ops.py
--rw-r--r--   0        0        0     3252 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/scatter.py
--rw-r--r--   0        0        0     3545 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/shape.py
--rw-r--r--   0        0        0      482 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/sparse.py
--rw-r--r--   0        0        0      784 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/type.py
--rw-r--r--   0        0        0       71 2024-04-29 13:57:25.988310 torch_sparse_tensor-0.1.1/sparse/typing.py
--rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 torch_sparse_tensor-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/README.md
+-rw-r--r--   0        0        0      556 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      123 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/__init__.py
+-rw-r--r--   0        0        0     7669 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/base.py
+-rw-r--r--   0        0        0     3648 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/cat.py
+-rw-r--r--   0        0        0      776 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/indexing.py
+-rw-r--r--   0        0        0     3672 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/mapping.py
+-rw-r--r--   0        0        0      519 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/mask.py
+-rw-r--r--   0        0        0     9306 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/ops.py
+-rw-r--r--   0        0        0     3876 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/scatter.py
+-rw-r--r--   0        0        0     3555 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/shape.py
+-rw-r--r--   0        0        0      482 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/sparse.py
+-rw-r--r--   0        0        0      787 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/type.py
+-rw-r--r--   0        0        0       71 2024-05-02 13:36:01.690930 torch_sparse_tensor-0.2.0/sparse/typing.py
+-rw-r--r--   0        0        0     2012 1970-01-01 00:00:00.000000 torch_sparse_tensor-0.2.0/PKG-INFO
```

### Comparing `torch_sparse_tensor-0.1.1/README.md` & `torch_sparse_tensor-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `torch_sparse_tensor-0.1.1/pyproject.toml` & `torch_sparse_tensor-0.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "torch-sparse-tensor"
-version = "0.1.1"
+version = "0.2.0"
 description = "A sparse tensor framework for Pytorch."
 authors = ["Astrid Klipfel <astridklipfel@gmail.com>"]
 readme = "README.md"
 
-packages = [
-    { include = "sparse" }
-]
+packages = [{ include = "sparse" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
+numpy = "*"
 torch = "^2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7"
```

### Comparing `torch_sparse_tensor-0.1.1/sparse/base.py` & `torch_sparse_tensor-0.2.0/sparse/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,22 +10,27 @@
     def __init__(
         self,
         indices: torch.LongTensor,
         values: torch.Tensor = None,
         shape: tuple = None,
         sort: bool = True,
     ):
-        self.indices = BaseSparse._process_indices(indices, values)
-        self.values = BaseSparse._process_values(values)
+        self._indices = BaseSparse._process_indices(indices, values)
+        self._values = BaseSparse._process_values(values)
         self.__shape = BaseSparse._process_shape(indices, shape)
 
         if sort and (not self._is_sorted()):
             self._sort_by_indices_()
             self._remove_sorted_duplicate_()
 
+    def create_shared(self, values: torch.Tensor | None = None) -> Self:
+        assert values is None or values.shape[0] == self._indices.shape[1]
+
+        return self.__class__(self._indices, values, self.shape, sort=False)
+
     @staticmethod
     def _process_shape(indices: torch.LongTensor, shape: tuple) -> tuple:
         assert (shape is None and indices.shape[1] != 0) or isinstance(shape, tuple)
 
         if shape is None:
             shape = tuple((indices.amax(dim=1) + 1).tolist())
         else:
@@ -50,78 +55,86 @@
     def _process_values(values: torch.Tensor) -> torch.Tensor:
         if values is not None and values.ndim == 1:
             values.unsqueeze_(1)
 
         return values
 
     @property
+    def indices(self) -> torch.LongTensor:
+        return self._indices
+
+    @property
+    def values(self) -> torch.Tensor:
+        return self._values
+
+    @property
     def shape(self) -> tuple:
         return self.__shape
 
     @property
     def ndim(self) -> int:
         return len(self.__shape)
 
     @property
     def dim(self) -> int:
         return len(self.__shape)
 
     @property
     def dtype(self) -> type:
-        if self.values is None:
+        if self._values is None:
             return torch.bool
 
-        return self.values.dtype
+        return self._values.dtype
 
     @property
     def device(self) -> torch.device:
-        return self.indices.device
+        return self._indices.device
 
     def to(self, device: torch.device) -> Self:
         return self.__class__(
-            indices=self.indices.to(device),
-            values=None if self.values is None else self.values.to(device),
+            indices=self._indices.to(device),
+            values=None if self._values is None else self._values.to(device),
             shape=self.shape,
         )
 
     def clone(self) -> Self:
         return self.__class__(
-            indices=self.indices.clone(),
-            values=None if self.values is None else self.values.clone(),
+            indices=self._indices.clone(),
+            values=None if self._values is None else self._values.clone(),
             shape=self.shape,
         )
 
     def detach(self) -> Self:
         return self.__class__(
-            indices=self.indices.detach(),
-            values=None if self.values is None else self.values.detach(),
+            indices=self._indices.detach(),
+            values=None if self._values is None else self._values.detach(),
             shape=self.shape,
         )
 
     def __repr__(self) -> str:
         return f"""{self.__class__.__name__}(shape={self.shape},
-  indices={self.indices},
-  values={self.values},
+  indices={self._indices},
+  values={self._values},
   device=\"{self.device}\")"""
 
     def to_dense(self) -> torch.Tensor:
-        if self.values is None or self.values.shape[1] == 1:
+        if self._values is None or self._values.shape[1] == 1:
             shape = self.shape
         else:
-            shape = self.shape + self.values.shape[1:]
+            shape = self.shape + self._values.shape[1:]
 
         dense_matrix = torch.zeros(shape, dtype=self.dtype, device=self.device)
-        indices = [self.indices[i] for i in range(self.indices.shape[0])]
+        indices = [self._indices[i] for i in range(self._indices.shape[0])]
 
-        if self.values is None:
+        if self._values is None:
             dense_matrix[indices] = 1
-        elif self.values.shape[1] == 1:
-            dense_matrix[indices] = self.values.flatten()
+        elif self._values.shape[1] == 1:
+            dense_matrix[indices] = self._values.flatten()
         else:
-            dense_matrix[indices] = self.values
+            dense_matrix[indices] = self._values
 
         return dense_matrix
 
     @property
     def dims(self) -> tuple:
         return tuple(range(len(self.__shape)))
 
@@ -129,15 +142,15 @@
     def _get_ptr(idx: torch.LongTensor) -> torch.LongTensor:
         # pylint: disable=not-callable
         return F.pad(idx.cumsum(0), (1, 0), value=0)
 
     def index_sorted(self, except_dim: int | Iterable = None) -> torch.LongTensor:
         dims = self._included_dims(except_dim)
 
-        diff = (self.indices[dims, 1:] != self.indices[dims, :-1]).any(dim=0)
+        diff = (self._indices[dims, 1:] != self._indices[dims, :-1]).any(dim=0)
 
         return self._get_ptr(diff)
 
     def _set_shape_(self, shape: tuple) -> Self:
         self.__shape = shape
         return self
 
@@ -187,41 +200,43 @@
                 perm = perm[current_perm]
 
         return perm
 
     def _sort_by_indices_(self, except_dim: int | Iterable = None):
         """Sort indices and values"""
         dims = self._included_dims(except_dim)
-        perm = self._argsort_indices(self.indices, dims)
+        perm = self._argsort_indices(self._indices, dims)
 
         # apply reindexing
-        self.indices = self.indices[:, perm]
+        self._indices = self._indices[:, perm]
 
-        if self.values is not None:
-            self.values = self.values[perm]
+        if self._values is not None:
+            self._values = self._values[perm]
 
     def _remove_sorted_duplicate_(self):
         # pylint: disable=not-callable
         mask = F.pad(
-            (self.indices[:, 1:] != self.indices[:, :-1]).any(dim=0), (1, 0), value=True
+            (self._indices[:, 1:] != self._indices[:, :-1]).any(dim=0),
+            (1, 0),
+            value=True,
         )
 
-        self.indices = self.indices[:, mask]
+        self._indices = self._indices[:, mask]
 
-        if self.values is not None:
+        if self._values is not None:
             batch = self._get_ptr(mask)[:-1, None]
-            self.values = torch.zeros(
-                (batch[-1] + 1, self.values.shape[1]),
-                dtype=self.values.dtype,
-                device=self.values.device,
-            ).scatter_add_(dim=0, index=batch.expand_as(self.values), src=self.values)
+            self._values = torch.zeros(
+                (batch[-1] + 1, self._values.shape[1]),
+                dtype=self._values.dtype,
+                device=self._values.device,
+            ).scatter_add_(dim=0, index=batch.expand_as(self._values), src=self._values)
 
     def _is_sorted(self) -> bool:
-        sorted_mask = self.indices.diff(dim=1) <= 0
-        unsorted_mask = self.indices.diff(dim=1) >= 0
+        sorted_mask = self._indices.diff(dim=1) <= 0
+        unsorted_mask = self._indices.diff(dim=1) >= 0
 
         dims = torch.tensor([self.dims], device=self.device).t()
         dims = dims.repeat(1, sorted_mask.shape[1])
 
         min_sorted = dims.clone()
         min_sorted[sorted_mask] = len(self.__shape)
         min_sorted = min_sorted.amin(dim=0)
```

### Comparing `torch_sparse_tensor-0.1.1/sparse/cat.py` & `torch_sparse_tensor-0.2.0/sparse/cat.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,12 +111,12 @@
 
     def _reindex_cat_dim_(
         self,
         dim: List[int],
         ptr: torch.LongTensor,
         cat_size: torch.LongTensor,
     ) -> Self:
-        self.indices[dim] += (
+        self._indices[dim] += (
             ptr[: cat_size.shape[0]].repeat_interleave(cat_size, dim=0).t()
         )
 
         return self
```

### Comparing `torch_sparse_tensor-0.1.1/sparse/ops.py` & `torch_sparse_tensor-0.2.0/sparse/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 def _intersection_mask(indices: torch.LongTensor, n_tensors: int) -> torch.BoolTensor:
     equal = (indices[:, 1:] != indices[:, :-1]).any(dim=0)
     equal_batch = BaseSparse._get_ptr(equal)
     mask = equal_batch[: -(n_tensors - 1)] == equal_batch[n_tensors - 1 :]
     return F.pad(mask, (0, n_tensors - 1), value=False)
 
 
-def _union_mask(indices: torch.LongTensor, n_tensors: int) -> torch.BoolTensor:
+def _union_mask(indices: torch.LongTensor, _: int) -> torch.BoolTensor:
     equal = (indices[:, 1:] != indices[:, :-1]).any(dim=0)
     return F.pad(equal, (1, 0), value=True)
 
 
 class SparseOpsMixin(SparseScatterMixin):
 
     def __and__(self, other: Self):
@@ -58,14 +58,17 @@
         cls,
         tensors: List[Self],
         indices_mask: Callable[[torch.LongTensor, int], torch.BoolTensor],
         ops: Callable[[torch.Tensor], torch.Tensor] = None,
     ) -> Self:
         assert len(tensors) > 1
 
+        if cls._is_shared_indices(tensors):
+            return cls._generic_shared_idx_ops(tensors, ops)
+
         tensors = cls._cast_sparse_tensors(tensors)
 
         shape = cls._get_shape(tensors)
         dims = tuple(range(len(shape)))
 
         # concatenating indices and values
         cat_indices, cat_values = cls._cat_values(tensors)
@@ -87,29 +90,57 @@
 
             batch = cls._cat_batch(tensors)[perm]
 
             values = cls._select_values(
                 cat_indices, cat_values, batch, mask, len(tensors)
             )
 
-            if ops is None:  # concatenation if no ops
-                values = values.reshape(values.shape[0], -1)
-            else:
-                values = ops(values).type(values.dtype)
-
-            # filter nul values
-            mask = (values != 0).all(dim=1)
-            indices, values = indices[:, mask], values[mask]
+            indices, values = cls._apply_ops_values(indices, values, ops)
         else:
             values = None
 
         # create a new sparse tensor containing the result
         return cls(indices, values=values, shape=shape)
 
     @classmethod
+    def _is_shared_indices(cls, tensors: List[Self]) -> bool:
+        return all(map(lambda x: id(x.indices) == id(tensors[0].indices), tensors[1:]))
+
+    @classmethod
+    def _generic_shared_idx_ops(
+        cls,
+        tensors: List[Self],
+        ops: Callable[[torch.Tensor], torch.Tensor] = None,
+    ) -> Self:
+        shape = tensors[0].shape
+        indices = tensors[0].indices
+        values = torch.stack([tensor.values for tensor in tensors], dim=1)
+        indices, values = cls._apply_ops_values(indices, values, ops)
+
+        return cls(indices, values=values, shape=shape, sort=False)
+
+    @classmethod
+    def _apply_ops_values(
+        cls,
+        indices: torch.LongTensor,
+        values: torch.Tensor,
+        ops: Callable[[torch.Tensor], torch.Tensor] = None,
+    ) -> Tuple[torch.LongTensor, torch.Tensor]:
+        if ops is None:  # concatenation if no ops
+            values = values.reshape(values.shape[0], -1)
+        else:
+            values = ops(values).type(values.dtype)
+
+        # filter nul values
+        mask = (values != 0).all(dim=1)
+        if (~mask).any():
+            return indices[:, mask], values[mask]
+        return indices, values
+
+    @classmethod
     def _select_values(
         cls,
         indices: torch.LongTensor,
         values: torch.Tensor,
         batch: torch.LongTensor,
         mask: torch.BoolTensor,
         n_tensors: int,
@@ -217,26 +248,26 @@
         self,
         indices: Iterable[torch.LongTensor],
         dims: Iterable[int],
         sizes: Iterable[int],
     ) -> Self:
         cart_prod = self._sparse_cart_prod(*indices)
 
-        repeated_dim = cart_prod.repeat_interleave(self.indices.shape[1], dim=1)
-        repeated_indices = self.indices.repeat(1, cart_prod.shape[1])
+        repeated_dim = cart_prod.repeat_interleave(self._indices.shape[1], dim=1)
+        repeated_indices = self._indices.repeat(1, cart_prod.shape[1])
         repeated_indices[list(dims)] = repeated_dim
 
         new_shape = list(self.shape)
         for dim, size in zip(dims, sizes):
             new_shape[dim] = size
 
-        if self.values is None:
+        if self._values is None:
             repeated_values = None
         else:
-            repeated_values = self.values.repeat(cart_prod.shape[1], 1)
+            repeated_values = self._values.repeat(cart_prod.shape[1], 1)
 
         return self.__class__(
             repeated_indices, values=repeated_values, shape=tuple(new_shape)
         )
 
     @classmethod
     def _sparse_cart_prod(cls, *tensors: torch.LongTensor) -> torch.LongTensor:
```

### Comparing `torch_sparse_tensor-0.1.1/sparse/shape.py` & `torch_sparse_tensor-0.2.0/sparse/shape.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,36 +10,36 @@
 
 class SparseShapeMixin(BaseSparse):
 
     def unsqueeze_(self, dim: int) -> Self:
         assert isinstance(dim, int)
 
         insert_zeros = torch.zeros(
-            (1, self.indices.shape[1]), dtype=torch.long, device=self.indices.device
+            (1, self._indices.shape[1]), dtype=torch.long, device=self._indices.device
         )
 
-        self.indices = torch.cat(
-            (self.indices[:dim], insert_zeros, self.indices[dim:]), dim=0
+        self._indices = torch.cat(
+            (self._indices[:dim], insert_zeros, self._indices[dim:]), dim=0
         )
         new_shape = list(self.shape)
         new_shape.insert(dim, 1)
         self._set_shape_(tuple(new_shape))
 
         return self
 
     def squeeze_(self, dim: int = None) -> Self:
         assert dim is None or isinstance(dim, int)
-        assert dim is None or dim <= self.indices.shape[0] and self.shape[dim] == 1
+        assert dim is None or dim <= self._indices.shape[0] and self.shape[dim] == 1
 
         if dim is None:
             keep_dim = [d for d, n in enumerate(self.shape) if n != 1]
         else:
             keep_dim = [d for d, _ in enumerate(self.shape) if d != dim]
 
-        self.indices = self.indices[keep_dim]
+        self._indices = self._indices[keep_dim]
         self._set_shape_(tuple(map(lambda d: self.shape[d], keep_dim)))
 
         return self
 
     def unsqueeze(self, dim: int) -> Self:
         sparse = self.clone()
         sparse.unsqueeze_(dim)
@@ -51,15 +51,15 @@
         sparse.squeeze_(dim)
 
         return sparse
 
     def reshape_(self, shape: int | Iterable[int]) -> Self:
         indices, shape = self._indices_to_shape(shape)
 
-        self.indices = indices
+        self._indices = indices
         self._set_shape_(shape)
 
         return self
 
     def reshape(self, shape: int | Iterable[int]) -> Self:
         cloned = self.clone()
         cloned.reshape_(shape)
@@ -111,11 +111,11 @@
             )
 
         shape = self._inferre_shape(shape)
 
         in_bases, _ = self._indexing_from_shape(self.shape)
         out_bases, out_shape = self._indexing_from_shape(shape)
 
-        global_index = (self.indices * in_bases[:, None]).sum(dim=0)
+        global_index = (self._indices * in_bases[:, None]).sum(dim=0)
         indices = (global_index[None, :] // out_bases[:, None]) % out_shape[:, None]
 
         return indices, shape
```

### Comparing `torch_sparse_tensor-0.1.1/sparse/type.py` & `torch_sparse_tensor-0.2.0/sparse/type.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from .typing import Self
 from .base import BaseSparse
 
 
 class SparseTypeMixin(BaseSparse):
 
     def type(self, dtype: type) -> Self:
-        if self.values is None:
+        if self._values is None:
             raise ValueError(
                 "Cannot convert the type of a sparse tensor without stored values."
             )
 
         return self.__class__(
-            self.indices.clone(),
-            self.values.type(dtype),
+            self._indices.clone(),
+            self._values.type(dtype),
             self.shape,
         )
 
     def float(self) -> Self:
         return self.type(torch.float32)
 
     def double(self) -> Self:
```

### Comparing `torch_sparse_tensor-0.1.1/PKG-INFO` & `torch_sparse_tensor-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: torch-sparse-tensor
-Version: 0.1.1
+Version: 0.2.0
 Summary: A sparse tensor framework for Pytorch.
 Author: Astrid Klipfel
 Author-email: astridklipfel@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: numpy
 Requires-Dist: torch (>=2,<3)
 Description-Content-Type: text/markdown
 
 # PyTorch Sparse Tensors
 
 A small package that implements the basic sparse tensor of any dimension.
```

