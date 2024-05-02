# Comparing `tmp/ditty-0.4.1.tar.gz` & `tmp/ditty-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ditty-0.4.1.tar", last modified: Sun Apr 28 04:17:56 2024, max compression
+gzip compressed data, was "ditty-0.5.0.tar", last modified: Thu May  2 15:41:44 2024, max compression
```

## Comparing `ditty-0.4.1.tar` & `ditty-0.5.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.312009 ditty-0.4.1/
--rw-r--r--   0 crow       (501) staff       (20)    11357 2023-12-10 02:25:24.000000 ditty-0.4.1/LICENSE
--rw-r--r--   0 crow       (501) staff       (20)     3616 2024-04-28 04:17:56.311943 ditty-0.4.1/PKG-INFO
--rw-r--r--   0 crow       (501) staff       (20)     3173 2023-12-10 08:48:25.000000 ditty-0.4.1/README.md
-drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.307612 ditty-0.4.1/lib/
-drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.310674 ditty-0.4.1/lib/ditty/
--rw-r--r--   0 crow       (501) staff       (20)        0 2023-12-10 02:25:24.000000 ditty-0.4.1/lib/ditty/__init__.py
--rw-r--r--   0 crow       (501) staff       (20)     5366 2023-12-10 09:23:34.000000 ditty-0.4.1/lib/ditty/data.py
--rw-r--r--   0 crow       (501) staff       (20)     7440 2023-12-10 08:46:51.000000 ditty-0.4.1/lib/ditty/pipeline.py
--rw-r--r--   0 crow       (501) staff       (20)     9272 2023-12-10 21:22:42.000000 ditty-0.4.1/lib/ditty/trainer.py
--rw-r--r--   0 crow       (501) staff       (20)      311 2023-12-10 02:25:24.000000 ditty-0.4.1/lib/ditty/utils.py
-drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-04-28 04:17:56.311682 ditty-0.4.1/lib/ditty.egg-info/
--rw-r--r--   0 crow       (501) staff       (20)     3616 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/PKG-INFO
--rw-r--r--   0 crow       (501) staff       (20)      302 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/SOURCES.txt
--rw-r--r--   0 crow       (501) staff       (20)        1 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/dependency_links.txt
--rw-r--r--   0 crow       (501) staff       (20)       56 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/requires.txt
--rw-r--r--   0 crow       (501) staff       (20)        6 2024-04-28 04:17:56.000000 ditty-0.4.1/lib/ditty.egg-info/top_level.txt
--rw-r--r--   0 crow       (501) staff       (20)      103 2024-04-28 04:17:56.312256 ditty-0.4.1/setup.cfg
--rw-r--r--   0 crow       (501) staff       (20)      639 2024-04-28 04:14:49.000000 ditty-0.4.1/setup.py
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-05-02 15:41:44.069743 ditty-0.5.0/
+-rw-r--r--   0 crow       (501) staff       (20)    11357 2023-12-10 02:25:24.000000 ditty-0.5.0/LICENSE
+-rw-r--r--   0 crow       (501) staff       (20)     3616 2024-05-02 15:41:44.069678 ditty-0.5.0/PKG-INFO
+-rw-r--r--   0 crow       (501) staff       (20)     3173 2023-12-10 08:48:25.000000 ditty-0.5.0/README.md
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-05-02 15:41:44.066886 ditty-0.5.0/lib/
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-05-02 15:41:44.068261 ditty-0.5.0/lib/ditty/
+-rw-r--r--   0 crow       (501) staff       (20)        0 2023-12-10 02:25:24.000000 ditty-0.5.0/lib/ditty/__init__.py
+-rw-r--r--   0 crow       (501) staff       (20)     5366 2023-12-10 09:23:34.000000 ditty-0.5.0/lib/ditty/data.py
+-rw-r--r--   0 crow       (501) staff       (20)     7420 2024-05-02 15:39:51.000000 ditty-0.5.0/lib/ditty/pipeline.py
+-rw-r--r--   0 crow       (501) staff       (20)     9272 2023-12-10 21:22:42.000000 ditty-0.5.0/lib/ditty/trainer.py
+-rw-r--r--   0 crow       (501) staff       (20)      311 2023-12-10 02:25:24.000000 ditty-0.5.0/lib/ditty/utils.py
+drwxr-xr-x   0 crow       (501) staff       (20)        0 2024-05-02 15:41:44.069442 ditty-0.5.0/lib/ditty.egg-info/
+-rw-r--r--   0 crow       (501) staff       (20)     3616 2024-05-02 15:41:44.000000 ditty-0.5.0/lib/ditty.egg-info/PKG-INFO
+-rw-r--r--   0 crow       (501) staff       (20)      302 2024-05-02 15:41:44.000000 ditty-0.5.0/lib/ditty.egg-info/SOURCES.txt
+-rw-r--r--   0 crow       (501) staff       (20)        1 2024-05-02 15:41:44.000000 ditty-0.5.0/lib/ditty.egg-info/dependency_links.txt
+-rw-r--r--   0 crow       (501) staff       (20)       56 2024-05-02 15:41:44.000000 ditty-0.5.0/lib/ditty.egg-info/requires.txt
+-rw-r--r--   0 crow       (501) staff       (20)        6 2024-05-02 15:41:44.000000 ditty-0.5.0/lib/ditty.egg-info/top_level.txt
+-rw-r--r--   0 crow       (501) staff       (20)      103 2024-05-02 15:41:44.069959 ditty-0.5.0/setup.cfg
+-rw-r--r--   0 crow       (501) staff       (20)      639 2024-05-02 15:41:14.000000 ditty-0.5.0/setup.py
```

### Comparing `ditty-0.4.1/LICENSE` & `ditty-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ditty-0.4.1/PKG-INFO` & `ditty-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.4.1
+Version: 0.5.0
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.4.1/README.md` & `ditty-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ditty-0.4.1/lib/ditty/data.py` & `ditty-0.5.0/lib/ditty/data.py`

 * *Files identical despite different names*

### Comparing `ditty-0.4.1/lib/ditty/pipeline.py` & `ditty-0.5.0/lib/ditty/pipeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 logging.basicConfig(level=logging.INFO)
 
 
 class Pipeline:
     def __init__(
         self,
         output_dir="./output",
-        dataset_name="code_search_net",
-        dataset_language="python",
+        dataset_namespace="code_search_net",
+        dataset_path="python",
         model_name_or_path="theblackcat102/pythia-3b-deduped-sft-r1",
         hf_hub_token=None,
         hf_hub_model_id=None,
         fp16=True,
         l8bit=True,
         l4bit=False,
         seed=None,
@@ -41,16 +41,16 @@
         gradient_checkpointing=True,
         experimental=False,
         block_size=2048,
         use_bfloat16=False,
         model_load_kwargs={"device_map": "auto"},
     ):
         self.output_dir = output_dir
-        self.dataset_name = dataset_name
-        self.dataset_language = dataset_language
+        self.dataset_namespace = dataset_namespace
+        self.dataset_path = dataset_path
         self.model_name_or_path = model_name_or_path
         self.hf_hub_token = hf_hub_token
         self.hf_hub_model_id = hf_hub_model_id
         self.fp16 = fp16
         self.seed = seed
         self.epochs = 1
         self.max_steps = None
@@ -89,16 +89,15 @@
 
     def dataset(self) -> DataLoader:
         """
         Subclass Pipeline and customize for your own dataset.
         """
 
         data = Data(
-            load_kwargs={"path": self.dataset_name, "name":
-                         self.dataset_language},
+            load_kwargs={"path": self.dataset_namespace, "name": self.dataset_path},
             tokenizer=self.tokenizer,
             seed=self.seed,
             batch_size=self.batch_size,
             grad_accum=self.grad_accum,
         )
 
         columns = data.dataset.features
@@ -156,20 +155,20 @@
         peft_config = LoraConfig(
             task_type=TaskType.CAUSAL_LM,
             target_modules=target_modules,
             inference_mode=False,
             r=8,
             lora_alpha=16,
             lora_dropout=0.05,
-            bias="none"
+            bias="none",
         )
 
-
         if self.l4bit:
             from peft import prepare_model_for_kbit_training
+
             self.model = prepare_model_for_kbit_training(
                 self.model, use_gradient_checkpointing=self.gradient_checkpointing
             )
         elif self.l8bit:
             self.model = prepare_model_for_int8_training(
                 self.model, use_gradient_checkpointing=self.gradient_checkpointing
             )
```

### Comparing `ditty-0.4.1/lib/ditty/trainer.py` & `ditty-0.5.0/lib/ditty/trainer.py`

 * *Files identical despite different names*

### Comparing `ditty-0.4.1/lib/ditty.egg-info/PKG-INFO` & `ditty-0.5.0/lib/ditty.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ditty
-Version: 0.4.1
+Version: 0.5.0
 Home-page: https://github.com/iantbutler01/ditty
 Author: Ian T Butler (KinglyCrow)
 Author-email: iantbutler01@gmail.com
 License: Apache V2
 Keywords: finetuning,llm,nlp,machine learning
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `ditty-0.4.1/setup.py` & `ditty-0.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from setuptools import setup, find_packages
 
 setup(
     name='ditty',
-    version='0.4.1',
+    version='0.5.0',
     license='Apache V2',
     author="Ian T Butler (KinglyCrow)",
     author_email='iantbutler01@gmail.com',
     packages=find_packages('lib'),
     package_dir={'': 'lib'},
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

