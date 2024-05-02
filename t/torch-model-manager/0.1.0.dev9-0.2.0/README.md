# Comparing `tmp/torch_model_manager-0.1.0.dev9.tar.gz` & `tmp/torch_model_manager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_model_manager-0.1.0.dev9.tar", last modified: Thu May  2 00:14:28 2024, max compression
+gzip compressed data, was "torch_model_manager-0.2.0.tar", last modified: Thu May  2 07:22:47 2024, max compression
```

## Comparing `torch_model_manager-0.1.0.dev9.tar` & `torch_model_manager-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/PKG-INFO
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/README.md
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/setup.cfg
--rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1450 2024-05-02 00:14:22.000000 torch_model_manager-0.1.0.dev9/setup.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.333655 torch_model_manager-0.1.0.dev9/tests/
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.337655 torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.337655 torch_model_manager-0.1.0.dev9/tests/test_utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/tests/test_utils/test_helpers.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.337655 torch_model_manager-0.1.0.dev9/torch_model_manager/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/torch_model_manager/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    23778 2024-05-01 19:16:10.000000 torch_model_manager-0.1.0.dev9/torch_model_manager/neptune_manager.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.1.0.dev9/torch_model_manager/torch_model_manager.py
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.345655 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/
--rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8746 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/PKG-INFO
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/SOURCES.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/dependency_links.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/requires.txt
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 00:14:28.000000 torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/top_level.txt
-drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 00:14:28.341655 torch_model_manager-0.1.0.dev9/utils/
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.1.0.dev9/utils/__init__.py
--rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.1.0.dev9/utils/helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.179138 torch_model_manager-0.2.0/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/PKG-INFO
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     8105 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/README.md
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       38 2024-05-02 07:22:47.179138 torch_model_manager-0.2.0/setup.cfg
+-rwxrwxrwx   0 billalmokhtari  (1000) billalmokhtari  (1000)     1445 2024-05-02 07:22:42.000000 torch_model_manager-0.2.0/setup.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.167137 torch_model_manager-0.2.0/tests/
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.171137 torch_model_manager-0.2.0/tests/test_torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     2462 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_torch_model_manager/test_torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.171137 torch_model_manager-0.2.0/tests/test_utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     3018 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/tests/test_utils/test_helpers.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/torch_model_manager/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       95 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/torch_model_manager/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    22422 2024-05-02 07:21:40.000000 torch_model_manager-0.2.0/torch_model_manager/neptune_manager.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)    16971 2024-04-27 14:30:36.000000 torch_model_manager-0.2.0/torch_model_manager/torch_model_manager.py
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/torch_model_manager.egg-info/
+-rw-r--r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     8741 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/PKG-INFO
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)      545 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/SOURCES.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        1 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/dependency_links.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       47 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/requires.txt
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)       32 2024-05-02 07:22:47.000000 torch_model_manager-0.2.0/torch_model_manager.egg-info/top_level.txt
+drwxrwxr-x   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-05-02 07:22:47.175138 torch_model_manager-0.2.0/utils/
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)        0 2024-04-24 08:45:48.000000 torch_model_manager-0.2.0/utils/__init__.py
+-rw-rw-r--   0 billalmokhtari  (1000) billalmokhtari  (1000)     6525 2024-04-28 09:54:06.000000 torch_model_manager-0.2.0/utils/helpers.py
```

### Comparing `torch_model_manager-0.1.0.dev9/PKG-INFO` & `torch_model_manager-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev9
+Version: 0.2.0
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev9/README.md` & `torch_model_manager-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev9/setup.py` & `torch_model_manager-0.2.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
-version = '0.1.0.dev9'
+version = '0.2.0'
 setup(
     name='torch-model-manager',
     version=version,
     description='A package for managing PyTorch models',
     author='Billal MOKHTARI',
     author_email='mokhtaribillal1@gmail.com',
     packages=find_packages(exclude=['tests',
```

### Comparing `torch_model_manager-0.1.0.dev9/tests/test_torch_model_manager/test_torch_model_manager.py` & `torch_model_manager-0.2.0/tests/test_torch_model_manager/test_torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev9/tests/test_utils/test_helpers.py` & `torch_model_manager-0.2.0/tests/test_utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev9/torch_model_manager/neptune_manager.py` & `torch_model_manager-0.2.0/torch_model_manager/neptune_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -252,65 +252,29 @@
                 profile = ProfileReport(dataframe, title=profile_report_title, **profile_report_kwargs)
                 
                 self.run[namespace][profile_report_name].upload(
                     File.from_content(profile.to_html(), extension="html")
                 )
             
         
-        # def init_npt_logger(self, 
-        #                     model: nn.Module,
-        #                     base_namespace: str='training', 
-        #                     log_model_diagram: bool=True, 
-        #                     log_freq: int=1,
-        #                     **kwargs):
-        #     """
-        #     Initialize the Neptune logger.
-
-        #     Args:
-        #         model (nn.Module): The model to log.
-        #         base_namespace (str, optional): The base namespace for logging. Defaults to 'training'.
-        #         log_model_diagram (bool, optional): Whether to log the model diagram. Defaults to True.
-        #         log_gradients (bool, optional): Whether to log the gradients. Defaults to True.
-        #         log_parameters (bool, optional): Whether to log the parameters. Defaults to True.
-        #         log_freq (int, optional): The logging frequency. Defaults to 1.
-        #     """
-        #     self.npt_logger = NeptuneLogger(
-        #         run=self.run,
-        #         base_namespace=base_namespace,
-        #         model=model,
-        #         log_model_diagram=log_model_diagram,
-        #         log_freq=log_freq,
-
-        #     )
-            
-        #     output = kwargs.get("output", None)
-        #     show_attrs = kwargs.get("show_attrs", True)
-        #     show_saved = kwargs.get("show_saved", True)
-        #     render_args = kwargs.get("render_args", {"filename": "model", "format": "png"})
-            
-        #     if output is not None:
-        #         make_dot(output, 
-        #             params=dict(model.named_parameters()), 
-        #             show_attrs=show_attrs, show_saved=show_saved).render(**render_args)
-        #         self.run[self.npt_logger.base_namespace]["model"][render_args["filename"]].upload(File.from_path(render_args["filename"]+"."+render_args["format"]), wait=True)
-                
-        
         def track_metric(self, 
-                         model: nn.Module, 
                          metric: Union[float, int],
-                         namespace: str):
+                         namespace: str,
+                         step = None,
+                         timestamp = None, 
+                         wait = False):
             """
             Track a metric.
 
             Args:
                 model (nn.Module): The model to track the metric for.
                 metric (Union[float, int]): The metric value.
                 namespace (str): The namespace to log the metric.
             """
-            self.run[namespace].append(metric)
+            self.run[namespace].append(metric, step=step, timestamp=timestamp, wait=wait)
 
         def log_checkpoint(self, namespace, model, optimizer, loss, epoch, **kwargs):
             state_dict = {
                 "model_state_dict": model.state_dict(),
                 "optimizer_state_dict": optimizer.state_dict(),
                 "loss": loss,
                 "epoch": epoch,
@@ -521,37 +485,52 @@
                 self.run[namespace].download(tmp_file.name)
                 state_dict = torch.load(tmp_file.name)
                 
                 return state_dict
             except:
                 print(Fore.RED+"The checkpoint is not fetched from Neptune. Please check the namespace."+Fore.WHITE)
 
+        def fetch_files(self, namespace):
+            ns = namespace.split("/")
+            
+            struct = self.run.get_structure()
+            for elem in ns :
+                struct = struct[elem]
+            
+            return list(struct.keys())
+        
         def fetch_data(self, namespace):
-            return list(self.run.get_structure()[namespace].keys())
+            return self.run[namespace].fetch_values()
         
-# nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
-#                     api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
-#                     run_ids_path="run_ids.json")
+nm = NeptuneManager(project_name="Billal-MOKHTARI/Image-Clustering-based-on-Dual-Message-Passing",
+                    api_token="eyJhcGlfYWRkcmVzcyI6Imh0dHBzOi8vYXBwLm5lcHR1bmUuYWkiLCJhcGlfdXJsIjoiaHR0cHM6Ly9hcHAubmVwdHVuZS5haSIsImFwaV9rZXkiOiI0NGRlOTNiZC0zNGZlLTRjNWUtYWEyMC00NzEwOWJkOTRhODgifQ==",
+                    run_ids_path="run_ids.json")
 
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
 
 
-# run = nm.Run(name="Image GAT Message Passing")
-# # data = run.fetch_pkl_data("embeddings")
-# # print(data)
+run = nm.Run(name="Image GAT Message Passing")
+# data = run.fetch_pkl_data("embeddings")
+# print(data)
 
 # model = models.resnet18(pretrained=True)
 # optimizer = torch.optim.Adam(model.parameters(), lr=1e-3)
 # loss = "MSE"
 # run.log_checkpoint(namespace="checkpoints", model=model, optimizer=optimizer, loss=loss, epoch=1)
 
-# chkpt = run.fetch_data("images")
-# print(chkpt)
+# chkpt = run.fetch_data("training/checkpoints")
+# print(chkpt)
+
+data = run.fetch_data("training/losses/MSE")
+print(data)
+# import time
+# for epoch in range(100):
+#     run.track_metric(epoch, "training/losses/MSE", step=epoch, timestamp=time.time(), wait=True)
```

### Comparing `torch_model_manager-0.1.0.dev9/torch_model_manager/torch_model_manager.py` & `torch_model_manager-0.2.0/torch_model_manager/torch_model_manager.py`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/PKG-INFO` & `torch_model_manager-0.2.0/torch_model_manager.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-model-manager
-Version: 0.1.0.dev9
+Version: 0.2.0
 Summary: A package for managing PyTorch models
 Home-page: https://github.com/Billal-MOKHTARI/torch-model-manager
 Author: Billal MOKHTARI
 Author-email: mokhtaribillal1@gmail.com
 Keywords: PyTorch,Deep Learning,Machine Learning,High Level Programming
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `torch_model_manager-0.1.0.dev9/torch_model_manager.egg-info/SOURCES.txt` & `torch_model_manager-0.2.0/torch_model_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `torch_model_manager-0.1.0.dev9/utils/helpers.py` & `torch_model_manager-0.2.0/utils/helpers.py`

 * *Files identical despite different names*

