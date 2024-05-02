# Comparing `tmp/labeled_contrastive_framework-0.2.5.tar.gz` & `tmp/labeled_contrastive_framework-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "labeled_contrastive_framework-0.2.5.tar", last modified: Thu Apr 25 19:16:24 2024, max compression
+gzip compressed data, was "labeled_contrastive_framework-0.2.6.tar", last modified: Thu May  2 12:21:52 2024, max compression
```

## Comparing `labeled_contrastive_framework-0.2.5.tar` & `labeled_contrastive_framework-0.2.6.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:16:24.931170 labeled_contrastive_framework-0.2.5/
--rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 18:44:05.000000 labeled_contrastive_framework-0.2.5/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      749 2024-04-25 19:16:24.931170 labeled_contrastive_framework-0.2.5/PKG-INFO
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:16:24.931170 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework/
--rw-r--r--   0 carl      (1000) carl      (1000)        0 2024-04-25 19:06:11.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     5647 2024-04-25 19:14:27.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework/module.py
--rw-r--r--   0 carl      (1000) carl      (1000)     2786 2024-04-24 00:16:10.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework/transform.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-25 19:16:24.931170 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      749 2024-04-25 19:16:09.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      411 2024-04-25 19:16:24.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-25 19:16:09.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       72 2024-04-25 19:16:09.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       80 2024-04-25 19:16:09.000000 labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)     1004 2024-04-25 19:15:19.000000 labeled_contrastive_framework-0.2.5/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-25 19:16:24.931170 labeled_contrastive_framework-0.2.5/setup.cfg
+drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:21:52.642734 labeled_contrastive_framework-0.2.6/
+-rw-r--r--   0 carlschader   (501) staff       (20)     1079 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.6/LICENSE
+-rw-r--r--   0 carlschader   (501) staff       (20)      749 2024-05-02 12:21:52.642523 labeled_contrastive_framework-0.2.6/PKG-INFO
+drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:21:52.641682 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/
+-rw-r--r--   0 carlschader   (501) staff       (20)        0 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/__init__.py
+-rw-r--r--   0 carlschader   (501) staff       (20)     7999 2024-05-02 12:19:25.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/module.py
+-rw-r--r--   0 carlschader   (501) staff       (20)     2786 2024-05-02 12:14:11.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/transform.py
+-rw-r--r--   0 carlschader   (501) staff       (20)        0 2024-05-02 12:18:39.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/utils.py
+drwxr-xr-x   0 carlschader   (501) staff       (20)        0 2024-05-02 12:21:52.642351 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/
+-rw-r--r--   0 carlschader   (501) staff       (20)      749 2024-05-02 12:21:52.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carlschader   (501) staff       (20)      450 2024-05-02 12:21:52.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)        1 2024-05-02 12:21:52.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)       72 2024-05-02 12:21:52.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/requires.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)       50 2024-05-02 12:21:52.000000 labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/top_level.txt
+-rw-r--r--   0 carlschader   (501) staff       (20)     1004 2024-05-02 12:20:46.000000 labeled_contrastive_framework-0.2.6/pyproject.toml
+-rw-r--r--   0 carlschader   (501) staff       (20)       38 2024-05-02 12:21:52.642771 labeled_contrastive_framework-0.2.6/setup.cfg
```

### Comparing `labeled_contrastive_framework-0.2.5/LICENSE` & `labeled_contrastive_framework-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.5/PKG-INFO` & `labeled_contrastive_framework-0.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.5
+Version: 0.2.6
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/labeled-contrastive-framework
 Project-URL: Issues, https://github.com/carlschader/labeled-contrastive-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.5/labeled_contrastive_framework/module.py` & `labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/module.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # Attempting to implement ArcFace without needing to compare 
 # the embeddings against the class centers across all classes,
 # but instead just against the class centers within the batch.
 
 import torch, multiprocessing
 import torch.nn as nn
 import torch.nn.functional as F
+from torch.utils.data import DataLoader, random_split
 import pytorch_lightning as L
 from torch import optim
 from fiblat import sphere_lattice
+from knowledge_distillation_framework import KnowledgeDistillationModule
 
-cross_entropy = nn.CrossEntropyLoss()
+
+# cross_entropy = nn.CrossEntropyLoss()
 
 # arcface loss function (centers are pre-normalized on a sphere of radius 1)
 def arcface_loss(embeddings, targets, centers, m=0.5, s=64.0):
     normalized_embeddings = F.normalize(embeddings, p=2, dim=1)
     cos_sims = torch.mm(normalized_embeddings, centers.t())
     angles = torch.acos(cos_sims)
     angles = angles + m # add margin
     margin_distances = s*torch.cos(angles)
-    return cross_entropy(margin_distances, targets)
+    return F.cross_entropy(margin_distances, targets)
+    # return cross_entropy(margin_distances, targets)
 
 class SphereNormalization(nn.Module):
     def __init__(self):
         super().__init__()
 
     def forward(self, X):
         return torch.nn.functional.normalize(X, p=2, dim=1)
@@ -43,16 +47,15 @@
         super().__init__()
         self.encoder = nn.Sequential( # add an embedding head
             backbone,
             nn.Linear(backbone_out_dim, embedding_dim),
             nn.ReLU(),
             nn.Linear(embedding_dim, embedding_dim),
         )
-        self.lodd_fn = loss_fn
-        self.loss_fn = arcface_loss
+        self.loss_fn = loss_fn
         self.margin = margin
         self.scale = scale
         self.learning_rate = learning_rate
         self.weight_decay = weight_decay
 
         # initialize class centers on a sphere
         self.centers = torch.tensor(sphere_lattice(embedding_dim, num_classes), dtype=torch.float32)
@@ -90,19 +93,82 @@
             'optimizer': optimizer,
             'lr_scheduler': {
                 'scheduler': scheduler,
                 "monitor": "val_loss",
             }
         }
 
+
+class LabeledContrastiveDistillationModule(KnowledgeDistillationModule):
+    '''
+    A PyTorch Lightning module for knowledge distillation.
+    Based on the paper "Improving Knowledge Distillation via Regularizing Feature 
+    Norm and Direction."
+
+    The student encoder and teacher encoder should output the same feature dimension.
+    '''
+    def __init__(
+            self, 
+            teacher_encoder,
+            student_encoder,
+            centers, # fibonnaci centers
+            task_loss_weight=1.0,
+            kd_loss_weight=2.0,
+            nd_loss_weight=4.0,
+            margin=0.5,
+            scale=64.0,
+            learning_rate=1e-4,
+            weight_decay=0.01,
+        ):
+        
+        self.centers = centers
+        self.task_loss_weight = task_loss_weight
+        self.kd_loss_weight = kd_loss_weight
+        self.nd_loss_weight = nd_loss_weight
+        self.margin = margin
+        self.scale = scale
+    
+        def combined_kd_loss(zs, zt, qs, qt, y):
+            kd_loss = (qs - qt).norm(p=2, dim=1).mean()
+
+            class_counts = torch.bincount(y)
+            qs_norm = qs.norm(p=2, dim=1)
+            qt_norm = qt.norm(p=2, dim=1)
+            max_norms = torch.stack([qs_norm, qt_norm]).max(dim=0)[0]
+            nd_loss = (qs * self.centers[y]).sum(dim=1)
+            nd_loss = nd_loss / max_norms
+            nd_loss = nd_loss / class_counts[y]
+            nd_loss = nd_loss.sum()
+            nd_loss = -nd_loss / torch.count_nonzero(class_counts)
+            return self.kd_loss_weight * kd_loss + self.nd_loss_weight * nd_loss
+
+            # return self.kd_loss_weight * kd_loss
+
+        super().__init__(
+            teacher_encoder=teacher_encoder,
+            student_encoder=student_encoder,
+            task_loss_fn=lambda zs, zt, qs, qt, y: self.task_loss_weight*arcface_loss(qs, y, self.centers, self.margin, self.scale),
+            teacher_head=nn.Identity(),
+            student_head=nn.Identity(),
+            kd_loss_fn=combined_kd_loss,
+            learning_rate=learning_rate,
+            weight_decay=weight_decay,
+        )
+
+        self.save_hyperparameters(ignore=['teacher_encoder', 'student_encoder'])
+
+    def on_fit_start(self):
+        self.centers = self.centers.to(self.device)
+
+
 if __name__ == '__main__':
     import time, argparse
     from torchvision import datasets
     from transform import make_transform
-    from lightning.pytorch.callbacks import ModelCheckpoint, LearningRateMonitor
+    from pytorch_lightning.callbacks import ModelCheckpoint, LearningRateMonitor
 
     # from transformers import Dinov2Model
 
     parser = argparse.ArgumentParser()
     parser.add_argument('dataset_path', type=str, help='Path to the image dataset')
     args = parser.parse_args()
 
@@ -120,18 +186,18 @@
     dataloader_workers = max((multiprocessing.cpu_count() // 2) - 1, 0)
     print('num_workers:', dataloader_workers)
 
     train_set_size = int(len(dataset) * 0.98)
     valid_set_size = len(dataset) - train_set_size
 
     seed = torch.Generator().manual_seed(42)
-    train_set, valid_set = torch.utils.data.random_split(dataset, [train_set_size, valid_set_size], generator=seed)
+    train_set, valid_set = random_split(dataset, [train_set_size, valid_set_size], generator=seed)
 
-    train_loader = torch.utils.data.DataLoader(train_set, batch_size=batch_size, shuffle=True, num_workers=dataloader_workers)
-    valid_loader = torch.utils.data.DataLoader(valid_set, batch_size=batch_size, shuffle=False, num_workers=dataloader_workers)
+    train_loader = DataLoader(train_set, batch_size=batch_size, shuffle=True, num_workers=dataloader_workers)
+    valid_loader = DataLoader(valid_set, batch_size=batch_size, shuffle=False, num_workers=dataloader_workers)
 
     print('loading backbone')
     # backbone = Dinov2Model.from_pretrained("facebook/dinov2-base").base_model
     backbone = torch.hub.load('facebookresearch/dinov2', 'dinov2_vits14_reg')
 
     print('initializing lightining module')
     lightning_module = LabeledContrastiveEncoder(backbone, backbone_out_dim, num_classes, embedding_dim=embedding_dim)
```

### Comparing `labeled_contrastive_framework-0.2.5/labeled_contrastive_framework/transform.py` & `labeled_contrastive_framework-0.2.6/labeled_contrastive_framework/transform.py`

 * *Files identical despite different names*

### Comparing `labeled_contrastive_framework-0.2.5/labeled_contrastive_framework.egg-info/PKG-INFO` & `labeled_contrastive_framework-0.2.6/labeled_contrastive_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: labeled_contrastive_framework
-Version: 0.2.5
+Version: 0.2.6
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/labeled-contrastive-framework
 Project-URL: Issues, https://github.com/carlschader/labeled-contrastive-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `labeled_contrastive_framework-0.2.5/pyproject.toml` & `labeled_contrastive_framework-0.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "labeled_contrastive_framework"
-version = "0.2.5"
+version = "0.2.6"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "Framework for training contrastive models with labeled data using arcface loss."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

