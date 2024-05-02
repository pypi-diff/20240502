# Comparing `tmp/fedjust-0.1.1.tar.gz` & `tmp/fedjust-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedjust-0.1.1.tar", max compression
+gzip compressed data, was "fedjust-0.1.2.tar", max compression
```

## Comparing `fedjust-0.1.1.tar` & `fedjust-0.1.2.tar`

### file list

```diff
@@ -1,13 +1,28 @@
--rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.1/FedJust/__init__.py
--rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.1/FedJust/aggregators/aggregator.py
--rw-r--r--   0        0        0     1515 2024-04-29 21:08:19.328339 fedjust-0.1.1/FedJust/files/archive.py
--rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.1/FedJust/files/handlers.py
--rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.1/FedJust/files/loggers.py
--rw-r--r--   0        0        0    15838 2024-04-30 15:06:32.398396 fedjust-0.1.1/FedJust/model/federated_model.py
--rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.1/FedJust/node/federated_node.py
--rw-r--r--   0        0        0     3335 2024-04-29 21:08:19.332339 fedjust-0.1.1/FedJust/operations/evaluations.py
--rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.1/FedJust/operations/orchestrations.py
--rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.1/FedJust/simulation/simulation.py
--rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.1/README.md
--rw-r--r--   0        0        0      426 2024-04-30 15:07:19.149581 fedjust-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3664 1970-01-01 00:00:00.000000 fedjust-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/__init__.py
+-rw-r--r--   0        0        0     1328 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/aggregators/__pycache__/aggregator.cpython-310.pyc
+-rw-r--r--   0        0        0     2048 2024-05-02 14:26:14.580289 fedjust-0.1.2/FedJust/aggregators/__pycache__/fedopt_aggregator.cpython-310.pyc
+-rw-r--r--   0        0        0     1052 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/aggregators/aggregator.py
+-rw-r--r--   0        0        0     1443 2024-05-02 14:26:01.448570 fedjust-0.1.2/FedJust/aggregators/fedopt_aggregator.py
+-rw-r--r--   0        0        0     1594 2024-05-01 11:48:27.774254 fedjust-0.1.2/FedJust/files/__pycache__/archive.cpython-310.pyc
+-rw-r--r--   0        0        0     1670 2024-05-01 11:48:27.774254 fedjust-0.1.2/FedJust/files/__pycache__/handlers.cpython-310.pyc
+-rw-r--r--   0        0        0      958 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/files/__pycache__/loggers.cpython-310.pyc
+-rw-r--r--   0        0        0     1515 2024-05-02 14:35:56.655748 fedjust-0.1.2/FedJust/files/archive.py
+-rw-r--r--   0        0        0     1721 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/files/handlers.py
+-rw-r--r--   0        0        0     2187 2024-04-29 21:08:19.328339 fedjust-0.1.2/FedJust/files/loggers.py
+-rw-r--r--   0        0        0    11104 2024-05-01 12:59:51.537271 fedjust-0.1.2/FedJust/model/__pycache__/federated_model.cpython-310.pyc
+-rw-r--r--   0        0        0    15871 2024-05-01 12:59:48.121354 fedjust-0.1.2/FedJust/model/federated_model.py
+-rw-r--r--   0        0        0     5227 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/node/__pycache__/federated_node.cpython-310.pyc
+-rw-r--r--   0        0        0     5910 2024-04-29 21:13:37.832090 fedjust-0.1.2/FedJust/node/federated_node.py
+-rw-r--r--   0        0        0     2844 2024-05-01 12:26:55.777282 fedjust-0.1.2/FedJust/operations/__pycache__/evaluations.cpython-310.pyc
+-rw-r--r--   0        0        0     3648 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/operations/__pycache__/orchestrations.cpython-310.pyc
+-rw-r--r--   0        0        0     3335 2024-05-01 12:25:08.143947 fedjust-0.1.2/FedJust/operations/evaluations.py
+-rw-r--r--   0        0        0     3430 2024-04-29 21:08:19.332339 fedjust-0.1.2/FedJust/operations/orchestrations.py
+-rw-r--r--   0        0        0     4737 2024-05-01 12:56:25.406255 fedjust-0.1.2/FedJust/simulation/__pycache__/adaptive_optimizer_simulation.cpython-310.pyc
+-rw-r--r--   0        0        0     8511 2024-05-01 11:48:27.770254 fedjust-0.1.2/FedJust/simulation/__pycache__/simulation.cpython-310.pyc
+-rw-r--r--   0        0        0     6205 2024-05-01 12:56:19.110407 fedjust-0.1.2/FedJust/simulation/adaptive_optimizer_simulation.py
+-rw-r--r--   0        0        0    10659 2024-04-29 21:08:19.332339 fedjust-0.1.2/FedJust/simulation/simulation.py
+-rw-r--r--   0        0        0      906 2024-05-01 12:08:02.750896 fedjust-0.1.2/FedJust/utils/__pycache__/computations.cpython-310.pyc
+-rw-r--r--   0        0        0      824 2024-05-01 12:07:32.211788 fedjust-0.1.2/FedJust/utils/computations.py
+-rw-r--r--   0        0        0     3091 2024-04-29 21:08:19.332339 fedjust-0.1.2/README.md
+-rw-r--r--   0        0        0      426 2024-05-02 14:37:08.390196 fedjust-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3664 1970-01-01 00:00:00.000000 fedjust-0.1.2/PKG-INFO
```

### Comparing `fedjust-0.1.1/FedJust/aggregators/aggregator.py` & `fedjust-0.1.2/FedJust/aggregators/aggregator.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/FedJust/files/archive.py` & `fedjust-0.1.2/FedJust/files/archive.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,14 +31,14 @@
     -------
     tuple[str, str str]
     """
     root = os.path.join(path, archive_name)
     assert not os.path.exists(root), f"Directory {root} already exists" 
     
     metrics_savepath = os.path.join(root, 'results')
-    nodes_models_savepath = os.path.join(root, 'models', 'orchestrator')
-    orchestrator_model_savepath = os.path.join(root, 'models', 'nodes')
+    orchestrator_model_savepath = os.path.join(root, 'models', 'orchestrator')
+    nodes_models_savepath = os.path.join(root, 'models', 'nodes')
     os.makedirs(metrics_savepath)
     os.makedirs(nodes_models_savepath)
     os.makedirs(orchestrator_model_savepath)
     
     return(metrics_savepath, nodes_models_savepath, orchestrator_model_savepath)
```

### Comparing `fedjust-0.1.1/FedJust/files/handlers.py` & `fedjust-0.1.2/FedJust/files/handlers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/FedJust/files/loggers.py` & `fedjust-0.1.2/FedJust/files/loggers.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/FedJust/model/federated_model.py` & `fedjust-0.1.2/FedJust/model/federated_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,20 +192,20 @@
         Returns
         -------------
             Oredered_Dict: Gradients of the network.
         """
         assert self.initial_model != None, "Computing gradients require saving initial model first!"
         self.net.to(self.cpu) # Dupming weights on cpu.
         self.initial_model.to(self.cpu)
-        weights_t1 = self.net.state_dict()
-        weights_t2 = self.initial_model.state_dict()
+        weights_trained = self.net.state_dict()
+        weights_initial = self.initial_model.state_dict()
         
-        self.gradients = OrderedDict.fromkeys(weights_t1.keys(), 0)
-        for key in weights_t1:
-            self.gradients[key] =  weights_t1[key] - weights_t2[key]
+        self.gradients = OrderedDict.fromkeys(weights_trained.keys(), 0)
+        for key in weights_trained:
+            self.gradients[key] =  weights_trained[key] - weights_initial[key]
 
         return self.gradients # Try: to provide original weights, no copies
 
 
     def update_weights(
         self, 
         avg_tensors
@@ -357,15 +357,15 @@
                 test_loss = criterion(output, targets).item()
                 losses.append(test_loss)
                 pred = output.argmax(dim=1, keepdim=True)
                 correct += pred.eq(targets.view_as(pred)).sum().item()
                 y_pred.append(pred)
                 y_true.append(targets)
 
-        test_loss = np.mean(losses)
+        test_loss = np.mean(test_loss)
         accuracy = correct / total
 
         y_true = [item.item() for sublist in y_true for item in sublist]
         y_pred = [item.item() for sublist in y_pred for item in sublist]
 
         f1score = f1_score(y_true, y_pred, average="macro")
         precision = precision_score(y_true, y_pred, average="macro")
```

### Comparing `fedjust-0.1.1/FedJust/node/federated_node.py` & `fedjust-0.1.2/FedJust/node/federated_node.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/FedJust/operations/evaluations.py` & `fedjust-0.1.2/FedJust/operations/evaluations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/FedJust/operations/orchestrations.py` & `fedjust-0.1.2/FedJust/operations/orchestrations.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/FedJust/simulation/simulation.py` & `fedjust-0.1.2/FedJust/simulation/simulation.py`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/README.md` & `fedjust-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fedjust-0.1.1/PKG-INFO` & `fedjust-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FedJust
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: Scolpe
 Author-email: 63779111+Scolpe@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

