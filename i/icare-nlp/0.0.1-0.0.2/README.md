# Comparing `tmp/icare_nlp-0.0.1.tar.gz` & `tmp/icare_nlp-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icare_nlp-0.0.1.tar", last modified: Wed May  1 13:53:17 2024, max compression
+gzip compressed data, was "icare_nlp-0.0.2.tar", last modified: Thu May  2 04:47:02 2024, max compression
```

## Comparing `icare_nlp-0.0.1.tar` & `icare_nlp-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,26 @@
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-01 13:53:17.902936 icare_nlp-0.0.1/
--rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-01 13:53:17.902936 icare_nlp-0.0.1/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-01 12:45:45.000000 icare_nlp-0.0.1/README.md
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-01 13:53:17.902936 icare_nlp-0.0.1/icare_nlp/
--rw-rw-r--   0 yi        (1000) yi        (1000)       49 2024-05-01 13:47:31.000000 icare_nlp-0.0.1/icare_nlp/__init__.py
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 11:36:21.000000 icare_nlp-0.0.1/icare_nlp/object_desc.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     6547 2024-05-01 12:33:44.000000 icare_nlp-0.0.1/icare_nlp/object_qa.py
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 09:07:45.000000 icare_nlp-0.0.1/icare_nlp/receipt_desc.py
--rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 09:07:53.000000 icare_nlp-0.0.1/icare_nlp/receipt_qa.py
--rw-rw-r--   0 yi        (1000) yi        (1000)     2999 2024-05-01 12:31:18.000000 icare_nlp-0.0.1/icare_nlp/utils.py
-drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-01 13:53:17.902936 icare_nlp-0.0.1/icare_nlp.egg-info/
--rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-01 13:53:17.000000 icare_nlp-0.0.1/icare_nlp.egg-info/PKG-INFO
--rw-rw-r--   0 yi        (1000) yi        (1000)      289 2024-05-01 13:53:17.000000 icare_nlp-0.0.1/icare_nlp.egg-info/SOURCES.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-01 13:53:17.000000 icare_nlp-0.0.1/icare_nlp.egg-info/dependency_links.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)       10 2024-05-01 13:53:17.000000 icare_nlp-0.0.1/icare_nlp.egg-info/top_level.txt
--rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-01 13:53:17.902936 icare_nlp-0.0.1/setup.cfg
--rw-rw-r--   0 yi        (1000) yi        (1000)      343 2024-05-01 13:52:17.000000 icare_nlp-0.0.1/setup.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 04:47:02.440816 icare_nlp-0.0.2/
+-rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-02 04:47:02.440816 icare_nlp-0.0.2/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-01 12:45:45.000000 icare_nlp-0.0.2/README.md
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 04:47:02.440816 icare_nlp-0.0.2/icare_nlp/
+-rw-rw-r--   0 yi        (1000) yi        (1000)       49 2024-05-01 13:47:31.000000 icare_nlp-0.0.2/icare_nlp/__init__.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 11:36:21.000000 icare_nlp-0.0.2/icare_nlp/object_desc.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     7319 2024-05-02 04:38:46.000000 icare_nlp-0.0.2/icare_nlp/object_qa.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 09:07:45.000000 icare_nlp-0.0.2/icare_nlp/receipt_desc.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-04-29 09:07:53.000000 icare_nlp-0.0.2/icare_nlp/receipt_qa.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 04:47:02.440816 icare_nlp-0.0.2/icare_nlp/resources/
+-rw-rw-r--   0 yi        (1000) yi        (1000)        0 2024-05-02 04:39:47.000000 icare_nlp-0.0.2/icare_nlp/resources/__init__.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)   247000 2024-04-30 13:33:50.000000 icare_nlp-0.0.2/icare_nlp/resources/category_emb_tensor.pt
+-rw-rw-r--   0 yi        (1000) yi        (1000)    15336 2024-04-30 05:51:45.000000 icare_nlp-0.0.2/icare_nlp/resources/category_tactile_description.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 12:13:21.000000 icare_nlp-0.0.2/icare_nlp/resources/inv_yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)      261 2024-04-30 12:07:36.000000 icare_nlp-0.0.2/icare_nlp/resources/invert.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)    11708 2024-04-30 13:50:11.000000 icare_nlp-0.0.2/icare_nlp/resources/object_types.py
+-rw-rw-r--   0 yi        (1000) yi        (1000)     3529 2024-04-30 13:33:44.000000 icare_nlp-0.0.2/icare_nlp/resources/rev_yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     1491 2024-04-30 13:35:28.000000 icare_nlp-0.0.2/icare_nlp/resources/yolo_obj_class_def.json
+-rw-rw-r--   0 yi        (1000) yi        (1000)     2999 2024-05-01 12:31:18.000000 icare_nlp-0.0.2/icare_nlp/utils.py
+drwxrwxr-x   0 yi        (1000) yi        (1000)        0 2024-05-02 04:47:02.440816 icare_nlp-0.0.2/icare_nlp.egg-info/
+-rw-r--r--   0 yi        (1000) yi        (1000)      166 2024-05-02 04:47:02.000000 icare_nlp-0.0.2/icare_nlp.egg-info/PKG-INFO
+-rw-rw-r--   0 yi        (1000) yi        (1000)      624 2024-05-02 04:47:02.000000 icare_nlp-0.0.2/icare_nlp.egg-info/SOURCES.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)        1 2024-05-02 04:47:02.000000 icare_nlp-0.0.2/icare_nlp.egg-info/dependency_links.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)       10 2024-05-02 04:47:02.000000 icare_nlp-0.0.2/icare_nlp.egg-info/top_level.txt
+-rw-rw-r--   0 yi        (1000) yi        (1000)       38 2024-05-02 04:47:02.440816 icare_nlp-0.0.2/setup.cfg
+-rw-rw-r--   0 yi        (1000) yi        (1000)      438 2024-05-02 04:46:52.000000 icare_nlp-0.0.2/setup.py
```

### Comparing `icare_nlp-0.0.1/icare_nlp/object_qa.py` & `icare_nlp-0.0.2/icare_nlp/object_qa.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 import json
 import torch
 from sentence_transformers import SentenceTransformer, util
-import utils
+from . import utils
+from importlib import resources
 class ObjectQA(object):
     def __init__(self):
         self.cls_model = SentenceTransformer('indiejoseph/bert-cantonese-sts')
         self.sentences1 = ["點樣可以攞到", "喺我手嘅邊個方向", "喺邊?", "tv喺邊？"]
         self.sentences2 = ["附近有冇其他物體"]
         self.embeddings1 = self.cls_model.encode(self.sentences1, convert_to_tensor=True)
         self.embeddings2 = self.cls_model.encode(self.sentences2, convert_to_tensor=True)
-        with open("resources/yolo_obj_class_def.json", "r") as f:
+        # with open("resources/yolo_obj_class_def.json", "r") as f:
+        #     self.yolo_cls = json.load(f)
+        # with open("resources/inv_yolo_obj_class_def.json", "r") as f:
+        #     self.inv_yolo_cls = json.load(f)
+        # with open("resources/rev_yolo_obj_class_def.json", "r", encoding="utf-8") as f:
+        #     self.rev_yolo_cls = json.load(f)
+        with resources.open_text("icare_nlp.resources", "yolo_obj_class_def.json") as f:
             self.yolo_cls = json.load(f)
-        with open("resources/inv_yolo_obj_class_def.json", "r") as f:
+        with resources.open_text("icare_nlp.resources", "inv_yolo_obj_class_def.json") as f:
             self.inv_yolo_cls = json.load(f)
-        with open("resources/rev_yolo_obj_class_def.json", "r", encoding="utf-8") as f:
+        with resources.open_text("icare_nlp.resources", "rev_yolo_obj_class_def.json") as f:
             self.rev_yolo_cls = json.load(f)
-        self.category_emb_tensor = torch.load('resources/category_emb_tensor.pt')
+        #self.category_emb_tensor = torch.load('resources/category_emb_tensor.pt')
         self.hand_centric=False
         self.target_obj=''
-        with open("resources/category_tactile_description.json", "r", encoding="utf-8") as f:
+        # with open("resources/category_tactile_description.json", "r", encoding="utf-8") as f:
+        #     self.cate_tac_desc = json.load(f)
+        with resources.open_text("icare_nlp.resources", "category_tactile_description.json", encoding="utf-8") as f:
             self.cate_tac_desc = json.load(f)
+        with resources.path("icare_nlp.resources", "category_emb_tensor.pt") as path:
+            self.category_emb_tensor = torch.load(str(path))
     def classify_query(self, question):
         input_embedding = self.cls_model.encode(question, convert_to_tensor=True)
         similarities1 = util.pytorch_cos_sim(input_embedding, self.embeddings1)
         similarities2 = util.pytorch_cos_sim(input_embedding, self.embeddings2)
         max_similarity1 = torch.max(similarities1)
         max_similarity2 = torch.max(similarities2)
         return 1 if max_similarity1 > max_similarity2 else 2
```

### Comparing `icare_nlp-0.0.1/icare_nlp/utils.py` & `icare_nlp-0.0.2/icare_nlp/utils.py`

 * *Files identical despite different names*

