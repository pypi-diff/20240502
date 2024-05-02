# Comparing `tmp/dillwave-1.0.2-py3-none-any.whl.zip` & `tmp/dillwave-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 18106 bytes, number of entries: 13
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 15:51 dillwave/__init__.py
--rw-r--r--  2.0 unx     2103 b- defN 24-May-02 15:51 dillwave/__main__.py
--rw-r--r--  2.0 unx     5753 b- defN 24-May-02 15:51 dillwave/dataset.py
--rw-r--r--  2.0 unx     4317 b- defN 24-May-02 15:51 dillwave/inference.py
--rw-r--r--  2.0 unx     7795 b- defN 24-May-02 15:51 dillwave/learner.py
--rw-r--r--  2.0 unx     5495 b- defN 24-May-02 15:51 dillwave/model.py
--rw-r--r--  2.0 unx     1720 b- defN 24-May-02 15:51 dillwave/params.py
--rw-r--r--  2.0 unx     2164 b- defN 24-May-02 15:51 dillwave/preprocess.py
--rw-r--r--  2.0 unx    11356 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     2613 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1004 b- defN 24-May-02 15:52 dillwave-1.0.2.dist-info/RECORD
-13 files, 44421 bytes uncompressed, 16448 bytes compressed:  63.0%
+Zip file size: 18065 bytes, number of entries: 13
+-rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:42 dillwave/__init__.py
+-rw-r--r--  2.0 unx     2103 b- defN 24-May-02 16:42 dillwave/__main__.py
+-rw-r--r--  2.0 unx     5753 b- defN 24-May-02 16:42 dillwave/dataset.py
+-rw-r--r--  2.0 unx     4317 b- defN 24-May-02 16:42 dillwave/inference.py
+-rw-r--r--  2.0 unx     7706 b- defN 24-May-02 16:43 dillwave/learner.py
+-rw-r--r--  2.0 unx     5495 b- defN 24-May-02 16:42 dillwave/model.py
+-rw-r--r--  2.0 unx     1720 b- defN 24-May-02 16:42 dillwave/params.py
+-rw-r--r--  2.0 unx     2164 b- defN 24-May-02 16:42 dillwave/preprocess.py
+-rw-r--r--  2.0 unx    11356 b- defN 24-May-02 16:47 dillwave-1.0.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     2613 b- defN 24-May-02 16:47 dillwave-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-02 16:47 dillwave-1.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 24-May-02 16:47 dillwave-1.0.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1004 b- defN 24-May-02 16:47 dillwave-1.0.3.dist-info/RECORD
+13 files, 44332 bytes uncompressed, 16407 bytes compressed:  63.0%
```

## zipnote {}

```diff
@@ -18,23 +18,23 @@
 
 Filename: dillwave/params.py
 Comment: 
 
 Filename: dillwave/preprocess.py
 Comment: 
 
-Filename: dillwave-1.0.2.dist-info/LICENSE.txt
+Filename: dillwave-1.0.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: dillwave-1.0.2.dist-info/METADATA
+Filename: dillwave-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: dillwave-1.0.2.dist-info/WHEEL
+Filename: dillwave-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: dillwave-1.0.2.dist-info/top_level.txt
+Filename: dillwave-1.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: dillwave-1.0.2.dist-info/RECORD
+Filename: dillwave-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dillwave/learner.py

```diff
@@ -115,17 +115,16 @@
               features = _nested_map(features, lambda x: x.to(device) if isinstance(x, torch.Tensor) else x)
               loss = self.train_step(features)
               if torch.isnan(loss).any():
                   raise RuntimeError(f'Detected NaN loss at step {self.step}.')
               if self.is_master:
                   if self.step % 50 == 0:
                       self._write_summary(self.step, features, loss)
-                  # Remove the following line to prevent saving initial weights file
-                  # if self.step % len(self.dataset) == 0:
-                  #     self.save_to_checkpoint()
+                  if self.step % len(self.dataset) == 0:
+                      self.save_to_checkpoint()
               self.step += 1
 
   def train_step(self, features):
     for param in self.model.parameters():
       param.grad = None
 
     audio = features['audio']
```

## Comparing `dillwave-1.0.2.dist-info/LICENSE.txt` & `dillwave-1.0.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `dillwave-1.0.2.dist-info/METADATA` & `dillwave-1.0.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dillwave
-Version: 1.0.2
+Version: 1.0.3
 Summary: dillwave
 Home-page: https://dill.moe
 Author: Cross Nastasi
 Author-email: cross@dill.moe
 License: Apache 2.0
 Keywords: dillwave machine learning neural vocoder tts speech
 Classifier: Development Status :: 4 - Beta
```

