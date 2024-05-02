# Comparing `tmp/knowledge_distillation_framework-0.1.0.tar.gz` & `tmp/knowledge_distillation_framework-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge_distillation_framework-0.1.0.tar", last modified: Fri Apr 26 18:55:43 2024, max compression
+gzip compressed data, was "knowledge_distillation_framework-0.1.1.tar", last modified: Thu May  2 02:29:41 2024, max compression
```

## Comparing `knowledge_distillation_framework-0.1.0.tar` & `knowledge_distillation_framework-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-26 18:55:43.411299 knowledge_distillation_framework-0.1.0/
--rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 19:26:24.000000 knowledge_distillation_framework-0.1.0/LICENSE
--rw-r--r--   0 carl      (1000) carl      (1000)      694 2024-04-26 18:55:43.407965 knowledge_distillation_framework-0.1.0/PKG-INFO
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-26 18:55:43.407965 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework/
--rw-r--r--   0 carl      (1000) carl      (1000)       48 2024-04-26 18:52:48.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework/__init__.py
--rw-r--r--   0 carl      (1000) carl      (1000)     3854 2024-04-26 18:45:38.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework/module.py
-drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-04-26 18:55:43.407965 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/
--rw-r--r--   0 carl      (1000) carl      (1000)      694 2024-04-26 18:55:43.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/PKG-INFO
--rw-r--r--   0 carl      (1000) carl      (1000)      389 2024-04-26 18:55:43.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/SOURCES.txt
--rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-04-26 18:55:43.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/dependency_links.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-26 18:55:43.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/requires.txt
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-26 18:55:43.000000 knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/top_level.txt
--rw-r--r--   0 carl      (1000) carl      (1000)      961 2024-04-26 18:53:23.000000 knowledge_distillation_framework-0.1.0/pyproject.toml
--rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-04-26 18:55:43.411299 knowledge_distillation_framework-0.1.0/setup.cfg
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-02 02:29:41.370948 knowledge_distillation_framework-0.1.1/
+-rw-r--r--   0 carl      (1000) carl      (1000)     1079 2024-04-25 19:26:24.000000 knowledge_distillation_framework-0.1.1/LICENSE
+-rw-r--r--   0 carl      (1000) carl      (1000)      694 2024-05-02 02:29:41.370948 knowledge_distillation_framework-0.1.1/PKG-INFO
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-02 02:29:41.370948 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework/
+-rw-r--r--   0 carl      (1000) carl      (1000)       48 2024-04-26 18:52:48.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework/__init__.py
+-rw-r--r--   0 carl      (1000) carl      (1000)     4254 2024-05-02 02:29:01.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework/module.py
+drwxr-xr-x   0 carl      (1000) carl      (1000)        0 2024-05-02 02:29:41.370948 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/
+-rw-r--r--   0 carl      (1000) carl      (1000)      694 2024-05-02 02:29:41.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/PKG-INFO
+-rw-r--r--   0 carl      (1000) carl      (1000)      389 2024-05-02 02:29:41.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)        1 2024-05-02 02:29:41.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-02 02:29:41.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/requires.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-02 02:29:41.000000 knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/top_level.txt
+-rw-r--r--   0 carl      (1000) carl      (1000)      961 2024-05-02 02:29:32.000000 knowledge_distillation_framework-0.1.1/pyproject.toml
+-rw-r--r--   0 carl      (1000) carl      (1000)       38 2024-05-02 02:29:41.370948 knowledge_distillation_framework-0.1.1/setup.cfg
```

### Comparing `knowledge_distillation_framework-0.1.0/LICENSE` & `knowledge_distillation_framework-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledge_distillation_framework-0.1.0/PKG-INFO` & `knowledge_distillation_framework-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge_distillation_framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/knowledge-distillation-framework
 Project-URL: Issues, https://github.com/carlschader/knowledge-distillation-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knowledge_distillation_framework-0.1.0/knowledge_distillation_framework/module.py` & `knowledge_distillation_framework-0.1.1/knowledge_distillation_framework/module.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,16 +10,14 @@
     TODO: TEST
     '''
     return F.kl_div(F.log_softmax(student_logits / temperature, dim=1), F.softmax(teacher_logits / temperature, dim=1))
 
 class KnowledgeDistillationModule(L.LightningModule):
     '''
     A PyTorch Lightning module for knowledge distillation.
-    Based on the paper "Improving Knowledge Distillation via Regularizing Feature 
-    Norm and Direction."
 
     The student encoder and teacher encoder should output the same feature dimension.
     
     The task loss function takes arguments (zs, zt, qs, qt, y) where zs and zt 
     are the student and teacher embeddings, qs and qt are the student and teacher
     head outputs, and y is the targets for the dataset.
 
@@ -47,57 +45,78 @@
 
         self.teacher_encoder = teacher_encoder
         self.student_encoder = student_encoder
 
         self.teacher_head = teacher_head
         self.student_head = student_head
 
+        for param in self.teacher_encoder.parameters():
+            param.requires_grad = False
+
+        for param in self.teacher_head.parameters():
+            param.requires_grad = False
+
         self.task_loss_fn = task_loss_fn
         self.kd_loss_fn = kd_loss_fn
         self.learning_rate = learning_rate
         self.weight_decay = weight_decay
        
         # freeze the teacher model
         self.teacher_encoder.eval()
         self.teacher_head.eval()
 
-        self.save_hyperparameters(ignore=['teacher_encoder', 'teacher_head'])
+        self.save_hyperparameters(ignore=['teacher_encoder', 'teacher_head', 'student_encoder', 'student_head'])
 
     def training_step(self, batch, batch_idx):
         x, y = batch
-        with torch.no_grad():
-            zt = self.teacher_encoder(x)
-            qt = self.teacher_head(zt)
+        zt = self.teacher_encoder(x)
+        qt = self.teacher_head(zt)
+
         zs = self.student_encoder(x)
         qs = self.student_head(zs)
-        loss = self.task_loss_fn(zs, zt, qs, qt, y) + self.kd_loss_fn(zs, zt, qs, qt, y)
+        
+        task_loss = self.task_loss_fn(zs, zt, qs, qt, y)
+        kd_loss = self.kd_loss_fn(zs, zt, qs, qt, y)
+
+        self.log('task_loss', task_loss, prog_bar=True)
+        self.log('kd_loss', kd_loss, prog_bar=True)
+
+        loss = task_loss + kd_loss
         self.log('train_loss', loss, prog_bar=True)
+
         return loss
 
     def validation_step(self, batch, batch_idx):
         x, y = batch
-        with torch.no_grad():
-            zt = self.teacher_encoder(x)
-            qt = self.teacher_head(zt)
+        zt = self.teacher_encoder(x)
+        qt = self.teacher_head(zt)
+
         zs = self.student_encoder(x)
         qs = self.student_head(zs)
-        loss = self.task_loss_fn(zs, zt, qs, qt, y) + self.kd_loss_fn(zs, zt, qs, qt, y)
+
+        task_loss = self.task_loss_fn(zs, zt, qs, qt, y)
+        kd_loss = self.kd_loss_fn(zs, zt, qs, qt, y)
+        self.log('val_task_loss', task_loss, prog_bar=True)
+        self.log('val_kd_loss', kd_loss, prog_bar=True)
+
+        loss = task_loss + kd_loss
         self.log('val_loss', loss, prog_bar=True)
+
         return loss
 
     def configure_optimizers(self):
         optimizer = optim.AdamW(self.parameters(), lr=self.learning_rate, weight_decay=self.weight_decay)
         # scheduler = optim.lr_scheduler.SequentialLR(optimizer, schedulers=[
         #     optim.lr_scheduler.LinearLR(optimizer, 0.33, 1.0, total_iters=5),
         #     optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=3, factor=0.5),
         # ],
         # milestones=[1])
         scheduler = optim.lr_scheduler.ReduceLROnPlateau(optimizer, patience=3, factor=0.5)
         return {
             'optimizer': optimizer,
             'lr_scheduler': {
                 'scheduler': scheduler,
-                "monitor": "val_loss",
+                "monitor": "val_task_loss",
             }
         }
```

### Comparing `knowledge_distillation_framework-0.1.0/knowledge_distillation_framework.egg-info/PKG-INFO` & `knowledge_distillation_framework-0.1.1/knowledge_distillation_framework.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: knowledge_distillation_framework
-Version: 0.1.0
+Version: 0.1.1
 Summary: Framework for training contrastive models with labeled data using arcface loss.
 Author-email: Carl Schader <carlschader@gmail.com>
 Project-URL: Homepage, https://github.com/carlschader/knowledge-distillation-framework
 Project-URL: Issues, https://github.com/carlschader/knowledge-distillation-framework/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `knowledge_distillation_framework-0.1.0/pyproject.toml` & `knowledge_distillation_framework-0.1.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "knowledge_distillation_framework"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Carl Schader", email="carlschader@gmail.com" },
 ]
 description = "Framework for training contrastive models with labeled data using arcface loss."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

