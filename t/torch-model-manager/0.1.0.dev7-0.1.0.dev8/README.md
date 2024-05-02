# Comparing `tmp/torch_model_manager-0.1.0.dev7.tar.gz` & `tmp/torch_model_manager-0.1.0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev7.tar", last modified: Wed May  1 13:05:13 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev8.tar", last modified: Wed May  1 13:20:28 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev7.tar` & `torch_model_manager-0.1.0.dev8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:13.007163 torch_model_manager-0.1.0.dev7/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 13:05:13.007163 torch_model_manager-0.1.0.dev7/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 13:05:13.007163 torch_model_manager-0.1.0.dev7/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 13:05:02.000000 torch_model_manager-0.1.0.dev7/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:12.987162 torch_model_manager-0.1.0.dev7/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:12.987162 torch_model_manager-0.1.0.dev7/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:12.987162 torch_model_manager-0.1.0.dev7/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:12.991163 torch_model_manager-0.1.0.dev7/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22927 2024-05-01 13:04:56.000000 torch_model_manager-0.1.0.dev7/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev7/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:13.007163 torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 13:05:12.000000 torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 13:05:12.000000 torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 13:05:12.000000 torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 13:05:12.000000 torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 13:05:12.000000 torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:05:13.007163 torch_model_manager-0.1.0.dev7/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev7/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev7/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 13:20:06.000000 torch_model_manager-0.1.0.dev8/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:27.999900 torch_model_manager-0.1.0.dev8/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.003900 torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.007900 torch_model_manager-0.1.0.dev8/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.011900 torch_model_manager-0.1.0.dev8/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23168 2024-05-01 13:19:57.000000 torch_model_manager-0.1.0.dev8/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev8/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev8/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev7/PKG-INFO` & `torch_model_manager-0.1.0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev7/README.md` & `torch_model_manager-0.1.0.dev8/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev7/setup.py` & `torch_model_manager-0.1.0.dev8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev7'
+version = '0.1.0.dev8'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev7/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev7/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev8/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev7/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev8/torch_model_manager/neptune_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -313,16 +313,17 @@
                 "model_state_dict": model.state_dict(),
                 "optimizer_state_dict": optimizer.state_dict(),
                 "loss": loss,
                 "epoch": epoch,
                 **kwargs
             }
             
-            with tempfile.NamedTemporaryFile(delete=True) as tmp_file:
-                torch.save(state_dict, tmp_file.name)
+            tmp_file = tempfile.NamedTemporaryFile(suffix = '.pth', delete=False)
+            torch.save(state_dict, tmp_file.name)
+                
                 
             self.log_files(namespace=namespace, data= None, from_path=tmp_file.name, extension='pth')
             
             print(Fore.GREEN+"The checkpoint is successfully logged to Neptune.", Fore.WHITE)
 
         def log_hyperparameters(self, 
                                hyperparams: dict, 
@@ -512,26 +513,32 @@
                 return data
                 
             except:
                 print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
 
 
-# nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-#                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-#                     run_ids_path="run_ids.json")
+nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
+                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
+                    run_ids_path="run_ids.json")
 
-# from torchvision import models
+from torchvision import models
 # parameters = {
 #     "lr": 1e-2,
 #     "bs": 128,
 #     "input_sz": 32 * 32 * 3,
 #     "n_classes": 10,
 #     "model_filename": "basemodel",
 #     "device": torch.device("cuda" if torch.cuda.is_available() else "cpu"),
 #     "epochs": 2,
 # }
 
 
 # run = nm.Run(name="Image GAT Message Passing")
-# data = run.fetch_pkl_data("embeddings")
-# print(data)
+# # data = run.fetch_pkl_data("embeddings")
+# # print(data)
+
+# model = models.resnet18(pretrained=True)
+# optimizer = torch.optim.Adam(model.parameters(), lr=1e-3)
+# loss = "MSE"
+# run.log_checkpoint(namespace="checkpoints", model=model, optimizer=optimizer, loss=loss, epoch=1)
+
```

### Comparing `torch_model_manager-0.1.0.dev7/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev8/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev7
+Version: 0.1.0.dev8
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev7/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev7/utils/helpers.py` & `torch_model_manager-0.1.0.dev8/utils/helpers.py`

 * *Files identical despite different names*

