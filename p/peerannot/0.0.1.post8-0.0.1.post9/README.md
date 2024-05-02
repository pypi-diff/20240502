# Comparing `tmp/PeerAnnot-0.0.1.post8.tar.gz` & `tmp/PeerAnnot-0.0.1.post9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PeerAnnot-0.0.1.post8.tar", last modified: Tue Dec 20 14:01:54 2022, max compression
+gzip compressed data, was "PeerAnnot-0.0.1.post9.tar", last modified: Tue Dec 20 16:38:00 2022, max compression
```

## Comparing `PeerAnnot-0.0.1.post8.tar` & `PeerAnnot-0.0.1.post9.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-20 14:01:54.000000 PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      746 2022-12-20 14:01:54.000000 PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 14:01:54.000000 PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-20 14:01:54.000000 PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-20 14:01:54.000000 PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/peerannot/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/peerannot/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/helpers/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/helpers/networks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/peerannot/models/
--rw-r--r--   0 runner    (1001) docker     (123)     3680 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/DS.py
--rw-r--r--   0 runner    (1001) docker     (123)     8017 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/DS_clust.py
--rw-r--r--   0 runner    (1001) docker     (123)     9584 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/GLAD.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/MV.py
--rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/Soft.py
--rw-r--r--   0 runner    (1001) docker     (123)    15964 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/WAUM.py
--rw-r--r--   0 runner    (1001) docker     (123)    14189 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/WAUM_stacked.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/models/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/peerannot/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/runners/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     9889 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/runners/identify.py
--rw-r--r--   0 runner    (1001) docker     (123)     4883 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/runners/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    13674 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/runners/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/peerannot/training/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/training/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/peerannot/training/load_data.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 14:01:54.185533 PeerAnnot-0.0.1.post8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-20 14:01:44.000000 PeerAnnot-0.0.1.post8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2022-12-20 16:38:00.000000 PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2022-12-20 16:38:00.000000 PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 16:38:00.000000 PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2022-12-20 16:38:00.000000 PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2022-12-20 16:38:00.000000 PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/peerannot/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/peerannot/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/helpers/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/helpers/networks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/peerannot/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/DS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8017 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/DS_clust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9584 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/GLAD.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/MV.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/Soft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15964 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/WAUM.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14189 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/WAUM_stacked.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      421 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/models/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/peerannot/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/runners/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10210 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/runners/identify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4883 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/runners/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13674 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/runners/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/peerannot/training/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/training/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/peerannot/training/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 16:38:00.270258 PeerAnnot-0.0.1.post9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2022-12-20 16:37:47.000000 PeerAnnot-0.0.1.post9/setup.py
```

### Comparing `PeerAnnot-0.0.1.post8/PeerAnnot.egg-info/SOURCES.txt` & `PeerAnnot-0.0.1.post9/PeerAnnot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/helpers/converters.py` & `PeerAnnot-0.0.1.post9/peerannot/helpers/converters.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/helpers/networks.py` & `PeerAnnot-0.0.1.post9/peerannot/helpers/networks.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/DS.py` & `PeerAnnot-0.0.1.post9/peerannot/models/DS.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/DS_clust.py` & `PeerAnnot-0.0.1.post9/peerannot/models/DS_clust.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/GLAD.py` & `PeerAnnot-0.0.1.post9/peerannot/models/GLAD.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/MV.py` & `PeerAnnot-0.0.1.post9/peerannot/models/MV.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/Soft.py` & `PeerAnnot-0.0.1.post9/peerannot/models/Soft.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/WAUM.py` & `PeerAnnot-0.0.1.post9/peerannot/models/WAUM.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/models/WAUM_stacked.py` & `PeerAnnot-0.0.1.post9/peerannot/models/WAUM_stacked.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/runners/__init__.py` & `PeerAnnot-0.0.1.post9/peerannot/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/runners/datasets.py` & `PeerAnnot-0.0.1.post9/peerannot/runners/datasets.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/runners/identify.py` & `PeerAnnot-0.0.1.post9/peerannot/runners/identify.py`

 * *Files 4% similar despite different names*

```diff
@@ -258,14 +258,16 @@
             f"Saved score per worker values at {path_waum / 'score_per_worker.json'}"
         )
         with open(path_waum / "aum_per_worker.json", "w") as f:
             dump(waum.aum_per_worker, f, level=2)
         print(
             f"Saved AUM per worker values at {path_waum / 'aum_per_worker.json'}"
         )
+        np.savetxt(path_waum / f"too_hard_{alpha}.txt", waum.too_hard)
+        print(f"Saved too hard index at {path_waum / f'too_hard_{alpha}.txt'}")
     elif method.lower() == "WAUMstacked".lower():
         from peerannot.models.WAUM_stacked import WAUM_stacked
 
         waum = WAUM_stacked(
             DataLoader(
                 trainset, batch_size=64, pin_memory=True, num_workers=1
             ),
@@ -294,17 +296,19 @@
             f"Saved score per worker values at {path_waum / 'score_per_worker.json'}"
         )
         with open(path_waum / "aum_per_worker", "w") as f:
             dump(waum.aum_per_worker, f, level=2)
         print(
             f"Saved AUM per worker values at {path_waum / 'aum_per_worker.json'}"
         )
+        np.savetxt(path_waum / f"too_hard_{alpha}.txt", waum.too_hard)
+        print(f"Saved too hard index at {path_waum / f'too_hard_{alpha}.txt'}")
 
     if method.startswith("WAUM"):
         path_results = path_folders / "labels"
         path_results.mkdir(parents=True, exist_ok=True)
-        path_file = path_results / (method.lower() + ".npy")
+        path_file = path_results / (method.lower() + f"_{str(alpha)}" + ".npy")
         yhat = waum.get_probas()
         np.save(path_file, yhat)
         print(
             f"Aggregated labels stored at {path_file} with shape {yhat.shape}"
         )
```

### Comparing `PeerAnnot-0.0.1.post8/peerannot/runners/run.py` & `PeerAnnot-0.0.1.post9/peerannot/runners/run.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/runners/train.py` & `PeerAnnot-0.0.1.post9/peerannot/runners/train.py`

 * *Files identical despite different names*

### Comparing `PeerAnnot-0.0.1.post8/peerannot/training/load_data.py` & `PeerAnnot-0.0.1.post9/peerannot/training/load_data.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,64 +35,56 @@
         #     "coast": 5,
         #     "mountain": 6,
         #     "opencountry": 7,
         # }
         dataset.real_class_to_idx = dataset.class_to_idx
 
     dataset.inv_class_to_idx = {v: k for k, v in dataset.class_to_idx.items()}
+    if path_remove:
+        rm_idx = np.loadtxt(path_remove, dtype=int)
+    else:
+        rm_idx = []
     if path_labels:
         labs = np.load(path_labels)
         ll = []
         targets = []
         imgs = []
         true_labels = []
-        for samp in dataset.samples:
-            img, true_label = samp
-            true_label = dataset.real_class_to_idx[
-                dataset.inv_class_to_idx[true_label]
-            ]
-            true_labels.append(true_label)
-            num = int(img.split("-")[1].split(".")[0])
-            ll.append((img, labs[num]))
-            imgs.append(img)
-            targets.append(labs[num])
+        for i, samp in enumerate(dataset.samples):
+            if i not in rm_idx:
+                img, true_label = samp
+                true_label = dataset.real_class_to_idx[
+                    dataset.inv_class_to_idx[true_label]
+                ]
+                true_labels.append(true_label)
+                num = int(img.split("-")[-1].split(".")[0])
+                ll.append((img, labs[num]))
+                imgs.append(img)
+                targets.append(labs[num])
     else:
         labs = dataset.targets
         ll = []
         targets = []
         imgs = []
         true_labels = []
-        for samp in dataset.samples:
-            img, true_label = samp
-            true_label = dataset.real_class_to_idx[
-                dataset.inv_class_to_idx[true_label]
-            ]
-            true_labels.append(true_label)
-            ll.append((img, true_label))
-            imgs.append(img)
-            targets.append(true_label)
+        for i, samp in enumerate(dataset.samples):
+            if i not in rm_idx:
+                img, true_label = samp
+                true_label = dataset.real_class_to_idx[
+                    dataset.inv_class_to_idx[true_label]
+                ]
+                true_labels.append(true_label)
+                ll.append((img, true_label))
+                imgs.append(img)
+                targets.append(true_label)
     dataset.samples = ll
     dataset.imgs = imgs
     dataset.targets = targets
     dataset.true_labels = true_labels
     dataset.class_to_idx = dataset.real_class_to_idx
-    if path_remove:
-        rm_idx = np.load(path_remove)
-        dataset.samples = [
-            samp for i, samp in enumerate(dataset.samples) if i not in rm_idx
-        ]
-        dataset.targets = [
-            tar for i, tar in enumerate(dataset.targets) if i not in rm_idx
-        ]
-        dataset.imgs = [
-            im for i, im in enumerate(dataset.imgs) if i not in rm_idx
-        ]
-        dataset.true_labels = [
-            im for i, im in enumerate(dataset.true_labels) if i not in rm_idx
-        ]
     if path_labels:
         acc = (
             np.mean(np.array(dataset.targets) == np.array(dataset.true_labels))
             if np.array(dataset.targets).ndim == 1
             else np.mean(
                 np.argmax(np.array(dataset.targets), axis=1)
                 == np.array(dataset.true_labels)
```

