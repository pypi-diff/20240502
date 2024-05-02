# Comparing `tmp/wah-0.1.8.tar.gz` & `tmp/wah-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wah-0.1.8.tar", last modified: Mon Feb  5 10:02:53 2024, max compression
+gzip compressed data, was "wah-0.1.9.tar", last modified: Tue Feb  6 06:49:13 2024, max compression
```

## Comparing `wah-0.1.8.tar` & `wah-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-02-05 10:02:53.374261 wah-0.1.8/
--rw-rw-rw-   0        0        0     1088 2024-01-25 07:45:40.000000 wah-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     4834 2024-02-05 10:02:53.362930 wah-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     4319 2024-02-01 09:59:18.000000 wah-0.1.8/README.md
--rw-rw-rw-   0        0        0      733 2024-02-05 09:57:12.000000 wah-0.1.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-02-05 10:02:53.374261 wah-0.1.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-02-05 10:02:53.338125 wah-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2024-02-05 10:02:53.354263 wah-0.1.8/src/wah/
--rw-rw-rw-   0        0        0      132 2024-02-05 08:41:14.000000 wah-0.1.8/src/wah/__init__.py
--rw-rw-rw-   0        0        0      268 2024-01-29 07:14:29.000000 wah-0.1.8/src/wah/config.py
--rw-rw-rw-   0        0        0     1764 2024-02-05 08:53:53.000000 wah-0.1.8/src/wah/data.py
--rw-rw-rw-   0        0        0     1081 2024-01-29 07:14:29.000000 wah-0.1.8/src/wah/log.py
--rw-rw-rw-   0        0        0      721 2024-02-01 06:08:05.000000 wah-0.1.8/src/wah/metrics.py
--rw-rw-rw-   0        0        0     6332 2024-02-05 10:01:25.000000 wah-0.1.8/src/wah/train.py
--rw-rw-rw-   0        0        0      775 2024-02-05 08:16:06.000000 wah-0.1.8/src/wah/typing.py
--rw-rw-rw-   0        0        0      582 2024-02-05 08:42:07.000000 wah-0.1.8/src/wah/utils.py
-drwxrwxrwx   0        0        0        0 2024-02-05 10:02:53.361930 wah-0.1.8/src/wah.egg-info/
--rw-rw-rw-   0        0        0     4834 2024-02-05 10:02:53.000000 wah-0.1.8/src/wah.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2024-02-05 10:02:53.000000 wah-0.1.8/src/wah.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-05 10:02:53.000000 wah-0.1.8/src/wah.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-02-05 10:02:53.000000 wah-0.1.8/src/wah.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-02-06 06:49:13.079870 wah-0.1.9/
+-rw-rw-rw-   0        0        0     1088 2024-01-25 07:45:40.000000 wah-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     4834 2024-02-06 06:49:13.078873 wah-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4319 2024-02-01 09:59:18.000000 wah-0.1.9/README.md
+-rw-rw-rw-   0        0        0      733 2024-02-06 06:47:49.000000 wah-0.1.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-02-06 06:49:13.080868 wah-0.1.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-02-06 06:49:12.996777 wah-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2024-02-06 06:49:13.069910 wah-0.1.9/src/wah/
+-rw-rw-rw-   0        0        0      132 2024-02-05 08:41:14.000000 wah-0.1.9/src/wah/__init__.py
+-rw-rw-rw-   0        0        0      268 2024-01-29 07:14:29.000000 wah-0.1.9/src/wah/config.py
+-rw-rw-rw-   0        0        0     1764 2024-02-05 08:53:53.000000 wah-0.1.9/src/wah/data.py
+-rw-rw-rw-   0        0        0     1081 2024-01-29 07:14:29.000000 wah-0.1.9/src/wah/log.py
+-rw-rw-rw-   0        0        0      721 2024-02-01 06:08:05.000000 wah-0.1.9/src/wah/metrics.py
+-rw-rw-rw-   0        0        0     6336 2024-02-06 06:40:44.000000 wah-0.1.9/src/wah/train.py
+-rw-rw-rw-   0        0        0      775 2024-02-05 08:16:06.000000 wah-0.1.9/src/wah/typing.py
+-rw-rw-rw-   0        0        0      582 2024-02-05 08:42:07.000000 wah-0.1.9/src/wah/utils.py
+drwxrwxrwx   0        0        0        0 2024-02-06 06:49:13.077877 wah-0.1.9/src/wah.egg-info/
+-rw-rw-rw-   0        0        0     4834 2024-02-06 06:49:12.000000 wah-0.1.9/src/wah.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      296 2024-02-06 06:49:12.000000 wah-0.1.9/src/wah.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-06 06:49:12.000000 wah-0.1.9/src/wah.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-02-06 06:49:12.000000 wah-0.1.9/src/wah.egg-info/top_level.txt
```

### Comparing `wah-0.1.8/LICENSE` & `wah-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/PKG-INFO` & `wah-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wah
-Version: 0.1.8
+Version: 0.1.9
 Summary: a library so simple you will learn Within An Hour
 Author-email: Juyeop Kim <juyeopkim@yonsei.ac.kr>
 Project-URL: Homepage, https://github.com/yupeeee/WAH
 Project-URL: Issues, https://github.com/yupeeee/WAH/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `wah-0.1.8/README.md` & `wah-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/pyproject.toml` & `wah-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "wah"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     { name = "Juyeop Kim", email = "juyeopkim@yonsei.ac.kr" },
 ]
 description = "a library so simple you will learn Within An Hour"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `wah-0.1.8/src/wah/data.py` & `wah-0.1.9/src/wah/data.py`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/src/wah/log.py` & `wah-0.1.9/src/wah/log.py`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/src/wah/metrics.py` & `wah-0.1.9/src/wah/metrics.py`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/src/wah/train.py` & `wah-0.1.9/src/wah/train.py`

 * *Files 8% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         for name, param in self.model.named_parameters():
             layer, attr = os.path.splitext(name)
             attr = attr[1:]  # removing '.'
 
             self.log(f"grads/l2_norm/{self.logger.name}/{layer}/{attr}", torch.norm(param.grad.flatten(), p=2))
 
     def on_train_epoch_end(self) -> None:
-        # self.log("step", self.current_epoch)
+        self.log("step", self.current_epoch + 1)
 
         self.log("train/avg_loss", self.train_loss)
 
         for label, metric in self.train_metrics:
             self.log(f"train/{label}", metric, metric_attribute=f"train_{clean(label)}")
 
         tensorboard = self.logger.experiment
@@ -168,15 +168,15 @@
             features = self.feature_extractor(data)["features"].reshape(len(batch), -1)
             features_l2 = torch.norm(features, p=2, dim=-1).cpu() / math.sqrt(features.size(-1))
             self.val_features_l2.append(features_l2)
 
         return loss
 
     def on_validation_epoch_end(self) -> None:
-        # self.log("step", self.current_epoch)
+        self.log("step", self.current_epoch + 1)
 
         self.log("val/avg_loss", self.val_loss)
 
         for label, metric in self.val_metrics:
             self.log(f"val/{label}", metric, metric_attribute=f"val_{clean(label)}")
 
         tensorboard = self.logger.experiment
```

### Comparing `wah-0.1.8/src/wah/typing.py` & `wah-0.1.9/src/wah/typing.py`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/src/wah/utils.py` & `wah-0.1.9/src/wah/utils.py`

 * *Files identical despite different names*

### Comparing `wah-0.1.8/src/wah.egg-info/PKG-INFO` & `wah-0.1.9/src/wah.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wah
-Version: 0.1.8
+Version: 0.1.9
 Summary: a library so simple you will learn Within An Hour
 Author-email: Juyeop Kim <juyeopkim@yonsei.ac.kr>
 Project-URL: Homepage, https://github.com/yupeeee/WAH
 Project-URL: Issues, https://github.com/yupeeee/WAH/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

