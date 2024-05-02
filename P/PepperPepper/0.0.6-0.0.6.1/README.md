# Comparing `tmp/pepperpepper-0.0.6.tar.gz` & `tmp/pepperpepper-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.tar", last modified: Thu May  2 06:41:35 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.1.tar", last modified: Thu May  2 07:01:48 2024, max compression
```

## Comparing `pepperpepper-0.0.6.tar` & `pepperpepper-0.0.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/
--rw-rw-rw-   0        0        0      431 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.581231 pepperpepper-0.0.6/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.6/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.613087 pepperpepper-0.0.6/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.628717 pepperpepper-0.0.6/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.644338 pepperpepper-0.0.6/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.659961 pepperpepper-0.0.6/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.675718 pepperpepper-0.0.6/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.675718 pepperpepper-0.0.6/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PepperPepper/models/
--rw-rw-rw-   0        0        0      990 2024-05-02 06:39:32.000000 pepperpepper-0.0.6/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    13354 2024-05-02 06:33:46.000000 pepperpepper-0.0.6/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      431 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      567 2024-05-02 06:40:01.000000 pepperpepper-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.058391 pepperpepper-0.0.6.1/
+-rw-rw-rw-   0        0        0      433 2024-05-02 07:01:48.057388 pepperpepper-0.0.6.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.006565 pepperpepper-0.0.6.1/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.6.1/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.038715 pepperpepper-0.0.6.1/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.1/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.1/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.1/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.040985 pepperpepper-0.0.6.1/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.1/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.1/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.1/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.045846 pepperpepper-0.0.6.1/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.1/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.048052 pepperpepper-0.0.6.1/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.1/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.1/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.1/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.1/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.050478 pepperpepper-0.0.6.1/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.1/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.1/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.1/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.052053 pepperpepper-0.0.6.1/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.1/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.1/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.055619 pepperpepper-0.0.6.1/PepperPepper/models/
+-rw-rw-rw-   0        0        0      990 2024-05-02 06:39:32.000000 pepperpepper-0.0.6.1/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    13242 2024-05-02 07:01:21.000000 pepperpepper-0.0.6.1/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.1/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.1/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.1/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.056386 pepperpepper-0.0.6.1/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.1/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.1/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.1/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.057388 pepperpepper-0.0.6.1/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-02 07:01:48.058391 pepperpepper-0.0.6.1/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-05-02 07:01:42.000000 pepperpepper-0.0.6.1/setup.py
```

### Comparing `pepperpepper-0.0.6/PepperPepper/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.1/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.1/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.1/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6.1/PepperPepper/models/cnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -351,24 +351,21 @@
             NiNBlock(96, 256, kernel_size=5, stride=1, padding=2),
             torch.nn.MaxPool2d(kernel_size=3, stride=2),
             NiNBlock(256, 384, kernel_size=3, stride=1, padding=1),
             torch.nn.MaxPool2d(kernel_size=3, stride=2),
             torch.nn.Dropout(p=0.5),  # 引入Dropout层防止过拟合
             NiNBlock(384, num_classes, kernel_size=3, stride=1, padding=1),
             # 使用全局平均池化替代全连接层
-            torch.nn.AdaptiveAvgPool2d((1, 1))
+            torch.nn.AdaptiveAvgPool2d((1, 1)),
+            torch.nn.Flatten()
         )
 
     def forward(self, x):
         # 通过特征提取层
         x = self.features(x)
-        # 将四维张量展平为二维张量
-        x = x.view(x.size(0), -1)
-        # 通过分类器层
-        x = self.classifier(x)
         return x
```

### Comparing `pepperpepper-0.0.6/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.1/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.1/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6/setup.py` & `pepperpepper-0.0.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6",
+    version="0.0.6.1",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

