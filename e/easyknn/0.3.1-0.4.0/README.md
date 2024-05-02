# Comparing `tmp/easyknn-0.3.1.tar.gz` & `tmp/easyknn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easyknn-0.3.1.tar", max compression
+gzip compressed data, was "easyknn-0.4.0.tar", max compression
```

## Comparing `easyknn-0.3.1.tar` & `easyknn-0.4.0.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      217 2022-11-29 20:51:10.907081 easyknn-0.3.1/easyknn/__init__.py
--rw-r--r--   0        0        0     8323 2022-11-29 20:51:10.907081 easyknn-0.3.1/easyknn/knn.py
--rw-r--r--   0        0        0      486 2022-11-29 20:51:20.943097 easyknn-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      540 2022-11-29 20:51:22.288205 easyknn-0.3.1/setup.py
--rw-r--r--   0        0        0      439 2022-11-29 20:51:22.288480 easyknn-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      217 2024-05-02 14:21:27.296064 easyknn-0.4.0/easyknn/__init__.py
+-rw-r--r--   0        0        0     9585 2024-05-02 14:21:27.296064 easyknn-0.4.0/easyknn/knn.py
+-rw-r--r--   0        0        0      498 2024-05-02 14:21:36.480067 easyknn-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      392 1970-01-01 00:00:00.000000 easyknn-0.4.0/PKG-INFO
```

### Comparing `easyknn-0.3.1/easyknn/knn.py` & `easyknn-0.4.0/easyknn/knn.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import pickle
 from pathlib import Path
-from typing import Type
+from typing import Literal, Type
 
 
 class KNNBackend:
     def build(
         self, vectors, init_kwargs: dict | None = None, fit_kwargs: dict | None = None
     ):
         raise NotImplementedError()
@@ -251,7 +251,50 @@
                 f"Unsupported backed {backend}. Must be one of [annoy, sklearn]"
             )
 
         index = builder.build(
             init_kwargs=init_kwargs, fit_kwargs=fit_kwargs, backend_cls=backend_cls
         )
         return cls(index=index, item2idx=builder.item2idx)
+
+    @classmethod
+    def from_builder_with_sklearn(
+        cls,
+        builder: EmbeddingsIndexBuilder,
+        n_neighbors: int = 5,
+        metric: str = "cosine",
+        radius: float = 1.0,
+        algorithm: Literal["auto", "ball_tree", "kd_tree", "brute"] = "auto",
+        init_kwargs: dict | None = None,
+    ):
+        init_kwargs = (init_kwargs or {}).update(
+            {
+                "n_neighbors": n_neighbors,
+                "metric": metric,
+                "radius": radius,
+                "algorithm": algorithm,
+            }
+        )
+        return cls.from_builder(
+            builder=builder, init_kwargs=init_kwargs, fit_kwargs=None, backend="sklearn"
+        )
+
+    @classmethod
+    def from_builder_with_annoy(
+        cls,
+        builder: EmbeddingsIndexBuilder,
+        metric: Literal[
+            "angular", "euclidean", "manhattan", "hamming", "dot"
+        ] = "euclidean",
+        n_trees: int = 10,
+        n_jobs: int = -1,
+    ):
+
+        init_kwargs = {"metric": metric}
+        fit_kwargs = {"n_trees": n_trees, "n_jobs": n_jobs}
+
+        return cls.from_builder(
+            builder=builder,
+            init_kwargs=init_kwargs,
+            fit_kwargs=fit_kwargs,
+            backend="annoy",
+        )
```

