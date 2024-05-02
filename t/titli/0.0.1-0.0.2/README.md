# Comparing `tmp/titli-0.0.1.tar.gz` & `tmp/titli-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "titli-0.0.1.tar", last modified: Wed May  1 08:11:09 2024, max compression
+gzip compressed data, was "titli-0.0.2.tar", last modified: Thu May  2 08:59:10 2024, max compression
```

## Comparing `titli-0.0.1.tar` & `titli-0.0.2.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:09.348307 titli-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-01 08:11:00.000000 titli-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-01 08:11:09.348307 titli-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-01 08:11:00.000000 titli-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 08:11:09.348307 titli-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-01 08:11:00.000000 titli-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:09.344307 titli-0.0.1/titli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:00.000000 titli-0.0.1/titli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:09.348307 titli-0.0.1/titli/fe/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-01 08:11:00.000000 titli-0.0.1/titli/fe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-01 08:11:00.000000 titli-0.0.1/titli/fe/after_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-01 08:11:00.000000 titli-0.0.1/titli/fe/base_feature_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-01 08:11:00.000000 titli-0.0.1/titli/fe/corClust.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:09.348307 titli-0.0.1/titli/ids/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-01 08:11:00.000000 titli-0.0.1/titli/ids/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-01 08:11:00.000000 titli-0.0.1/titli/ids/base_ids.py
--rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-05-01 08:11:00.000000 titli-0.0.1/titli/ids/kitsune.py
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-01 08:11:00.000000 titli-0.0.1/titli/ids/pytorch_kitsune.py
--rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-05-01 08:11:00.000000 titli-0.0.1/titli/ids/torch_kitnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:09.348307 titli-0.0.1/titli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-01 08:11:00.000000 titli-0.0.1/titli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-01 08:11:00.000000 titli-0.0.1/titli/utils/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 08:11:09.348307 titli-0.0.1/titli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-01 08:11:09.000000 titli-0.0.1/titli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-01 08:11:09.000000 titli-0.0.1/titli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:11:09.000000 titli-0.0.1/titli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 08:11:09.000000 titli-0.0.1/titli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-01 08:11:09.000000 titli-0.0.1/titli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 08:11:09.000000 titli-0.0.1/titli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.660381 titli-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-02 08:59:05.000000 titli-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 08:59:10.660381 titli-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-02 08:59:05.000000 titli-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 08:59:10.660381 titli-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-05-02 08:59:05.000000 titli-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:05.000000 titli-0.0.2/titli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/fe/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23767 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/after_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6110 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/base_feature_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-05-02 08:59:05.000000 titli-0.0.2/titli/fe/corClust.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/ids/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/base_ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17521 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/kitsune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/pytorch_kitsune.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4084 2024-05-02 08:59:05.000000 titli-0.0.2/titli/ids/torch_kitnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.656381 titli-0.0.2/titli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-02 08:59:05.000000 titli-0.0.2/titli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-02 08:59:05.000000 titli-0.0.2/titli/utils/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 08:59:10.660381 titli-0.0.2/titli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-02 08:59:10.000000 titli-0.0.2/titli.egg-info/top_level.txt
```

### Comparing `titli-0.0.1/LICENSE` & `titli-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/PKG-INFO` & `titli-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titli
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for collection of IDS and tools for evaluating them
 Home-page: https://github.com/spg-iitd/raids
 Author: Subrat Kumar Swain
 Author-email: mailofswainsubrat@gmail.com
 License: MIT
 Keywords: ids adversarial network nids
 Classifier: Programming Language :: Python :: 3
```

### Comparing `titli-0.0.1/setup.py` & `titli-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='titli',
-    version='0.0.1',
+    version='0.0.2',
     description='A library for collection of IDS and tools for evaluating them',
     long_description=open("README.md").read(),
     long_description_content_type = "text/markdown",
     url='https://github.com/spg-iitd/raids',
     packages=find_packages(),
     license='MIT',
     author="Subrat Kumar Swain",
```

### Comparing `titli-0.0.1/titli/fe/after_image.py` & `titli-0.0.2/titli/fe/after_image.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/titli/fe/base_feature_extractor.py` & `titli-0.0.2/titli/fe/base_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/titli/fe/corClust.py` & `titli-0.0.2/titli/fe/corClust.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/titli/ids/base_ids.py` & `titli-0.0.2/titli/ids/base_ids.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/titli/ids/kitsune.py` & `titli-0.0.2/titli/ids/kitsune.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/titli/ids/pytorch_kitsune.py` & `titli-0.0.2/titli/ids/pytorch_kitsune.py`

 * *Files identical despite different names*

### Comparing `titli-0.0.1/titli/ids/torch_kitnet.py` & `titli-0.0.2/titli/ids/torch_kitnet.py`

 * *Files 4% similar despite different names*

```diff
@@ -75,31 +75,29 @@
 
 
 class TorchKitNET(nn.Module):
     def __init__(self, clusters: list, norms_path: str):
         super(TorchKitNET, self).__init__()
         self.dataset = "PcapDatasetRaw"
         self.input_dim = sum([len(c) for c in clusters])
-        self.raw = True
         self.hr = 0.75
         self.clusters = clusters
         self.rmse = RMSELoss()
         self.tails = nn.ModuleList([BaseAutoencoder(len(c), int(np.ceil(len(c) * self.hr))) for c in clusters])
         self.head = BaseAutoencoder(len(clusters), int(np.ceil(len(clusters) * self.hr)))
         with open(norms_path, "rb") as f:
             self.norm_params = pickle.load(f)
 
     def forward(self, x):
-        x = torch.tensor(x)
         x = x.view(-1, self.input_dim)
 
         x_clusters = []
         for c in self.clusters:
-            norm_max = self.norm_params[f"norm_max_{c[0]}"]
-            norm_min = self.norm_params[f"norm_min_{c[0]}"]
+            norm_max = torch.tensor(self.norm_params[f"norm_max_{c[0]}"])
+            norm_min = torch.tensor(self.norm_params[f"norm_min_{c[0]}"])
 
             x_cluster = torch.index_select(x, 1, torch.tensor(c))
             x_cluster = (x_cluster - norm_min) / (norm_max - norm_min + 0.0000000000000001)
             x_cluster = x_cluster.float()
 
             x_clusters.append(x_cluster)
```

### Comparing `titli-0.0.1/titli.egg-info/PKG-INFO` & `titli-0.0.2/titli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: titli
-Version: 0.0.1
+Version: 0.0.2
 Summary: A library for collection of IDS and tools for evaluating them
 Home-page: https://github.com/spg-iitd/raids
 Author: Subrat Kumar Swain
 Author-email: mailofswainsubrat@gmail.com
 License: MIT
 Keywords: ids adversarial network nids
 Classifier: Programming Language :: Python :: 3
```

