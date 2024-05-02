# Comparing `tmp/torch_model_manager-0.2.0.tar.gz` & `tmp/torch_model_manager-0.2.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.2.0.tar", last modified: Thu May  2 07:22:47 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.dev1.tar", last modified: Thu May  2 07:24:56 2024, max compression
```

## Comparing `torch_model_manager-0.2.0.tar` & `torch_model_manager-0.2.0.dev1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.179138 torch_model_manager-0.2.0/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 07:22:47.179138 torch_model_manager-0.2.0/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1445 2024-05-02 07:22:42.000000 torch_model_manager-0.2.0/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.167137 torch_model_manager-0.2.0/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.171137 torch_model_manager-0.2.0/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.171137 torch_model_manager-0.2.0/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22422 2024-05-02 07:21:40.000000 torch_model_manager-0.2.0/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.085000 torch_model_manager-0.2.0.dev1/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 07:24:56.085000 torch_model_manager-0.2.0.dev1/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-02 07:24:50.000000 torch_model_manager-0.2.0.dev1/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.077000 torch_model_manager-0.2.0.dev1/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22434 2024-05-02 07:24:44.000000 torch_model_manager-0.2.0.dev1/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0.dev1/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 07:24:56.000000 torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:24:56.081000 torch_model_manager-0.2.0.dev1/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0.dev1/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0.dev1/utils/helpers.py
```

### Comparing `torch_model_manager-0.2.0/PKG-INFO` & `torch_model_manager-0.2.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0
+Version: 0.2.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0/README.md` & `torch_model_manager-0.2.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0/setup.py` & `torch_model_manager-0.2.0.dev1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.2.0'
+version = '0.2.0.dev1'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.2.0/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0.dev1/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0.dev1/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0.dev1/torch_model_manager/neptune_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -497,40 +497,40 @@
                 struct = struct[elem]
             
             return list(struct.keys())
         
         def fetch_data(self, namespace):
             return self.run[namespace].fetch_values()
         
-nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-                    run_ids_path="run_ids.json")
+# nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
+#                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
+#                     run_ids_path="run_ids.json")
 
 # from torchvision import models
 # parameters = {
 #     "lr": 1e-2,
 #     "bs": 128,
 #     "input_sz": 32 * 32 * 3,
 #     "n_classes": 10,
 #     "model_filename": "basemodel",
 #     "device": torch.device("cuda" if torch.cuda.is_available() else "cpu"),
 #     "epochs": 2,
 # }
 
 
-run = nm.Run(name="Image GAT Message Passing")
+# run = nm.Run(name="Image GAT Message Passing")
 # data = run.fetch_pkl_data("embeddings")
 # print(data)
 
 # model = models.resnet18(pretrained=True)
 # optimizer = torch.optim.Adam(model.parameters(), lr=1e-3)
 # loss = "MSE"
 # run.log_checkpoint(namespace="checkpoints", model=model, optimizer=optimizer, loss=loss, epoch=1)
 
 # chkpt = run.fetch_data("training/checkpoints")
 # print(chkpt)
 
-data = run.fetch_data("training/losses/MSE")
-print(data)
+# data = run.fetch_data("training/losses/MSE")
+# print(data)
 # import time
 # for epoch in range(100):
 #     run.track_metric(epoch, "training/losses/MSE", step=epoch, timestamp=time.time(), wait=True)
```

### Comparing `torch_model_manager-0.2.0/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0.dev1/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.2.0
+Version: 0.2.0.dev1
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.2.0/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0.dev1/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.2.0/utils/helpers.py` & `torch_model_manager-0.2.0.dev1/utils/helpers.py`

 * *Files identical despite different names*

