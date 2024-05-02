# Comparing `tmp/torch_model_manager-0.1.0.dev8.tar.gz` & `tmp/torch_model_manager-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev8.tar", last modified: Wed May  1 13:20:28 2024, max compression
+gzip compressed data, was "torch_model_manager-0.1.0.dev9.tar", last modified: Thu May  2 00:14:28 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev8.tar` & `torch_model_manager-0.1.0.dev9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-01 13:20:06.000000 torch_model_manager-0.1.0.dev8/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:27.999900 torch_model_manager-0.1.0.dev8/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.003900 torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.007900 torch_model_manager-0.1.0.dev8/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.011900 torch_model_manager-0.1.0.dev8/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23168 2024-05-01 13:19:57.000000 torch_model_manager-0.1.0.dev8/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev8/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-01 13:20:27.000000 torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-01 13:20:28.039900 torch_model_manager-0.1.0.dev8/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev8/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev8/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-02 00:14:22.000000 torch_model_manager-0.1.0.dev9/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.333655 torch_model_manager-0.1.0.dev9/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.337655 torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.337655 torch_model_manager-0.1.0.dev9/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.337655 torch_model_manager-0.1.0.dev9/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23778 2024-05-01 19:16:10.000000 torch_model_manager-0.1.0.dev9/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev9/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.341655 torch_model_manager-0.1.0.dev9/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev9/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev8/PKG-INFO` & `torch_model_manager-0.1.0.dev9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev8/README.md` & `torch_model_manager-0.1.0.dev9/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev8/setup.py` & `torch_model_manager-0.1.0.dev9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev8'
+version = '0.1.0.dev9'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev8/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev8/tests/test_utils/test_helpers.py` & `torch_model_manager-0.1.0.dev9/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev8/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.1.0.dev9/torch_model_manager/neptune_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -511,21 +511,32 @@
             
                 print(Fore.GREEN+"The data is successfully fetched from Neptune.", Fore.WHITE)
                 return data
                 
             except:
                 print(Fore.RED+"The data is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
+        def load_model_checkpoint(self, namespace):
+            tmp_file = tempfile.NamedTemporaryFile(delete=True)
+            try:
+                self.run[namespace].download(tmp_file.name)
+                state_dict = torch.load(tmp_file.name)
+                
+                return state_dict
+            except:
+                print(Fore.RED+"The checkpoint is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
+        def fetch_data(self, namespace):
+            return list(self.run.get_structure()[namespace].keys())
+        
+# nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
+#                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
+#                     run_ids_path="run_ids.json")
 
-nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-                    run_ids_path="run_ids.json")
-
-from torchvision import models
+# from torchvision import models
 # parameters = {
 #     "lr": 1e-2,
 #     "bs": 128,
 #     "input_sz": 32 * 32 * 3,
 #     "n_classes": 10,
 #     "model_filename": "basemodel",
 #     "device": torch.device("cuda" if torch.cuda.is_available() else "cpu"),
@@ -538,7 +549,9 @@
 # # print(data)
 
 # model = models.resnet18(pretrained=True)
 # optimizer = torch.optim.Adam(model.parameters(), lr=1e-3)
 # loss = "MSE"
 # run.log_checkpoint(namespace="checkpoints", model=model, optimizer=optimizer, loss=loss, epoch=1)
 
+# chkpt = run.fetch_data("images")
+# print(chkpt)
```

### Comparing `torch_model_manager-0.1.0.dev8/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.1.0.dev9/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev8/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev8/utils/helpers.py` & `torch_model_manager-0.1.0.dev9/utils/helpers.py`

 * *Files identical despite different names*

