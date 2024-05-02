# Comparing `tmp/labeled_contrastive_framework-0.2.8.tar.gz` & `tmp/labeled_contrastive_framework-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeled_contrastive_framework-0.2.8.tar", last modified: Thu May  2 12:50:03 2024, max compression
+gzip compressed data, was "labeled_contrastive_framework-0.2.9.tar", last modified: Thu May  2 12:54:30 2024, max compression
```

## Comparing `labeled_contrastive_framework-0.2.8.tar` & `labeled_contrastive_framework-0.2.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:50:03.951060 labeled_contrastive_framework-0.2.8/
--rw-r--r--   0 carlschader   (501) staff       (20)     1079 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.8/LICENSE
--rw-r--r--   0 carlschader   (501) staff       (20)      804 2024-05-02 12:50:03.950870 labeled_contrastive_framework-0.2.8/PKG-INFO
-drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:50:03.949968 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/
--rw-r--r--   0 carlschader   (501) staff       (20)        0 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/__init__.py
--rw-r--r--   0 carlschader   (501) staff       (20)     7999 2024-05-02 12:19:25.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/module.py
--rw-r--r--   0 carlschader   (501) staff       (20)     2786 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/transform.py
--rw-r--r--   0 carlschader   (501) staff       (20)        0 2024-05-02 12:18:39.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/utils.py
-drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:50:03.950675 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/
--rw-r--r--   0 carlschader   (501) staff       (20)      804 2024-05-02 12:50:03.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/PKG-INFO
--rw-r--r--   0 carlschader   (501) staff       (20)      450 2024-05-02 12:50:03.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carlschader   (501) staff       (20)        1 2024-05-02 12:50:03.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carlschader   (501) staff       (20)      112 2024-05-02 12:50:03.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/requires.txt
--rw-r--r--   0 carlschader   (501) staff       (20)       50 2024-05-02 12:50:03.000000 labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/top_level.txt
--rw-r--r--   0 carlschader   (501) staff       (20)     1052 2024-05-02 12:49:49.000000 labeled_contrastive_framework-0.2.8/pyproject.toml
--rw-r--r--   0 carlschader   (501) staff       (20)       38 2024-05-02 12:50:03.951096 labeled_contrastive_framework-0.2.8/setup.cfg
+drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:54:30.364856 labeled_contrastive_framework-0.2.9/
+-rw-r--r--   0 carlschader   (501) staff       (20)     1079 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.9/LICENSE
+-rw-r--r--   0 carlschader   (501) staff       (20)      804 2024-05-02 12:54:30.364647 labeled_contrastive_framework-0.2.9/PKG-INFO
+drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:54:30.363711 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/
+-rw-r--r--   0 carlschader   (501) staff       (20)        0 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/__init__.py
+-rw-r--r--   0 carlschader   (501) staff       (20)     7855 2024-05-02 12:54:09.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/module.py
+-rw-r--r--   0 carlschader   (501) staff       (20)     2786 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/transform.py
+-rw-r--r--   0 carlschader   (501) staff       (20)        0 2024-05-02 12:18:39.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/utils.py
+drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:54:30.364441 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/
+-rw-r--r--   0 carlschader   (501) staff       (20)      804 2024-05-02 12:54:30.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carlschader   (501) staff       (20)      450 2024-05-02 12:54:30.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)        1 2024-05-02 12:54:30.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)      112 2024-05-02 12:54:30.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/requires.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)       50 2024-05-02 12:54:30.000000 labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/top_level.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)     1052 2024-05-02 12:54:23.000000 labeled_contrastive_framework-0.2.9/pyproject.toml
+-rw-r--r--   0 carlschader   (501) staff       (20)       38 2024-05-02 12:54:30.364894 labeled_contrastive_framework-0.2.9/setup.cfg
```

### Comparing `labeled_contrastive_framework-0.2.8/LICENSE` & `labeled_contrastive_framework-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.8/PKG-INFO` & `labeled_contrastive_framework-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.8
+Version: 0.2.9
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/labeled-contrastive-framework
 Project-URL: Issues, https://github.com/carlschader/labeled-contrastive-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/module.py` & `labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/module.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,55 +7,52 @@
 import torch.nn.functional as F
 from torch.utils.data import DataLoader, random_split
 import pytorch_lightning as L
 from torch import optim
 from fiblat import sphere_lattice
 from knowledge_distillation_framework import KnowledgeDistillationModule
 
-
-# cross_entropy = nn.CrossEntropyLoss()
-
-# arcface loss function (centers are pre-normalized on a sphere of radius 1)
-def arcface_loss(embeddings, targets, centers, m=0.5, s=64.0):
-    normalized_embeddings = F.normalize(embeddings, p=2, dim=1)
-    cos_sims = torch.mm(normalized_embeddings, centers.t())
-    angles = torch.acos(cos_sims)
-    angles = angles + m # add margin
-    margin_distances = s*torch.cos(angles)
-    return F.cross_entropy(margin_distances, targets)
-    # return cross_entropy(margin_distances, targets)
-
 class SphereNormalization(nn.Module):
     def __init__(self):
         super().__init__()
 
     def forward(self, X):
         return torch.nn.functional.normalize(X, p=2, dim=1)
 
 class LabeledContrastiveEncoder(L.LightningModule):
     def __init__(
             self, 
             backbone, 
             backbone_out_dim,
             num_classes, 
-            loss_fn=arcface_loss, 
             embedding_dim=128, 
             margin=0.5, 
             scale=64.0,
             learning_rate=1e-4,
             weight_decay=0.01,
         ):
+
+        def arcface_loss(embeddings, targets, centers, m=0.5, s=64.0):
+            normalized_embeddings = F.normalize(embeddings, p=2, dim=1)
+            cos_sims = torch.mm(normalized_embeddings, centers.t())
+            angles = torch.acos(cos_sims)
+            angles = angles + m # add margin
+            margin_distances = s*torch.cos(angles)
+            return F.cross_entropy(margin_distances, targets)
+
+
+
         super().__init__()
         self.encoder = nn.Sequential( # add an embedding head
             backbone,
             nn.Linear(backbone_out_dim, embedding_dim),
             nn.ReLU(),
             nn.Linear(embedding_dim, embedding_dim),
         )
-        self.loss_fn = loss_fn
+        self.loss_fn = arcface_loss
         self.margin = margin
         self.scale = scale
         self.learning_rate = learning_rate
         self.weight_decay = weight_decay
 
         # initialize class centers on a sphere
         self.centers = torch.tensor(sphere_lattice(embedding_dim, num_classes), dtype=torch.float32)
```

### Comparing `labeled_contrastive_framework-0.2.8/labeled_contrastive_framework/transform.py` & `labeled_contrastive_framework-0.2.9/labeled_contrastive_framework/transform.py`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.8/labeled_contrastive_framework.egg-info/PKG-INFO` & `labeled_contrastive_framework-0.2.9/labeled_contrastive_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.8
+Version: 0.2.9
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/labeled-contrastive-framework
 Project-URL: Issues, https://github.com/carlschader/labeled-contrastive-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.8/pyproject.toml` & `labeled_contrastive_framework-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "labeled_contrastive_framework"
-version = "0.2.8"
+version = "0.2.9"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "Framework for training contrastive models with labeled data using arcface loss."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

