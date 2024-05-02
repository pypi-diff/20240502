# Comparing `tmp/pepperpepper-0.0.5.9.tar.gz` & `tmp/pepperpepper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.5.9.tar", last modified: Tue Apr 30 16:37:09 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.tar", last modified: Thu May  2 06:41:35 2024, max compression
```

## Comparing `pepperpepper-0.0.5.9.tar` & `pepperpepper-0.0.6.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.958895 pepperpepper-0.0.5.9/
--rw-rw-rw-   0        0        0      433 2024-04-30 16:37:09.958895 pepperpepper-0.0.5.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.863825 pepperpepper-0.0.5.9/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.5.9/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.912263 pepperpepper-0.0.5.9/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.5.9/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.5.9/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.5.9/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.925963 pepperpepper-0.0.5.9/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.5.9/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.5.9/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.5.9/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.935594 pepperpepper-0.0.5.9/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.5.9/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.5.9/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.5.9/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.5.9/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.5.9/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.938458 pepperpepper-0.0.5.9/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.5.9/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.5.9/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.5.9/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.5.9/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.944763 pepperpepper-0.0.5.9/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.5.9/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.5.9/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.5.9/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.944763 pepperpepper-0.0.5.9/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.5.9/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.5.9/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.944763 pepperpepper-0.0.5.9/PepperPepper/models/
--rw-rw-rw-   0        0        0      873 2024-04-30 16:36:55.000000 pepperpepper-0.0.5.9/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    10402 2024-04-30 16:32:02.000000 pepperpepper-0.0.5.9/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.5.9/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.5.9/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.5.9/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.958048 pepperpepper-0.0.5.9/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.5.9/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.5.9/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.5.9/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-04-30 16:37:09.958895 pepperpepper-0.0.5.9/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-04-30 16:37:09.000000 pepperpepper-0.0.5.9/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-04-30 16:37:09.000000 pepperpepper-0.0.5.9/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-30 16:37:09.000000 pepperpepper-0.0.5.9/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-04-30 16:37:09.000000 pepperpepper-0.0.5.9/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-04-30 16:37:09.000000 pepperpepper-0.0.5.9/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.5.9/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-04-30 16:37:09.958895 pepperpepper-0.0.5.9/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-04-30 16:37:02.000000 pepperpepper-0.0.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/
+-rw-rw-rw-   0        0        0      431 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.581231 pepperpepper-0.0.6/PepperPepper/
+-rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.6/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.613087 pepperpepper-0.0.6/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.628717 pepperpepper-0.0.6/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.644338 pepperpepper-0.0.6/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.659961 pepperpepper-0.0.6/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.675718 pepperpepper-0.0.6/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.675718 pepperpepper-0.0.6/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PepperPepper/models/
+-rw-rw-rw-   0        0        0      990 2024-05-02 06:39:32.000000 pepperpepper-0.0.6/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    13354 2024-05-02 06:33:46.000000 pepperpepper-0.0.6/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      431 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 06:41:35.000000 pepperpepper-0.0.6/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-02 06:41:35.691347 pepperpepper-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      567 2024-05-02 06:40:01.000000 pepperpepper-0.0.6/setup.py
```

### Comparing `pepperpepper-0.0.5.9/PepperPepper/__init__.py` & `pepperpepper-0.0.6/PepperPepper/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/core/utils.py` & `pepperpepper-0.0.6/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6/PepperPepper/models/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,20 +8,26 @@
 
 # models/__init__.py
 # 如果需要，您可以直接导入这些模块中的特定类或函数
 from .cnn import LeNet5
 from .cnn import AlexNet
 from .cnn import VGGBlock
 from .cnn import VGG16
+from .cnn import MLPConv
+from .cnn import NiNBlock
+from .cnn import NiN
 #from .rnn import RNNModel
 #from .transformer import TransformerModel
 #from .custom_model import CustomModel
 
 
 # __all__ 变量定义了当使用 from models import * 时导入哪些对象
 # 注意：通常不推荐使用 from package import *
 __all__ = [
    'LeNet5',
    'AlexNet',
    'VGGBlock',
-   'VGG16'
+   'VGG16',
+   'MLPConv',
+   'NiNBlock',
+   'NiN'
 ]
```

### Comparing `pepperpepper-0.0.5.9/PepperPepper/models/cnn.py` & `pepperpepper-0.0.6/PepperPepper/models/cnn.py`

 * *Files 16% similar despite different names*

```diff
@@ -250,27 +250,135 @@
         返回:
             torch.Tensor: 分类的logits
         """
         # 特征提取
         x = self.features(x)
 
         # 在将特征图送入全连接层之前，需要将其展平（flatten）
-        # 假设输入图像的大小是224x224，经过5个池化层（每个池化层将尺寸减半）后，
+        # 假设输入图像的大小是3x224x224，经过5个池化层（每个池化层将尺寸减半）后，
         # 特征图的大小会变成 7x7
         x = x.view(x.size(0), -1)  # 展平操作，-1 表示让PyTorch自动计算该维度的大小
 
         # 送入分类器
         x = self.classifier(x)
 
         return x
 
 
 
 
 
 
 
+
+
+
+
+#5.MLPConv层
+class MLPConv(torch.nn.Module):
+    """
+    MLPConv层，包含一个1x1卷积层模拟MLP的行为
+    """
+    def __init__(self, in_channels, hidden_channels, out_channels):
+        super(MLPConv,self).__init__()
+        # 第一个1x1卷积层，用于减少通道数
+        self.conv1 = torch.nn.Conv2d(in_channels, hidden_channels, kernel_size=1, bias=True)
+
+        # ReLU激活函数
+        self.relu = torch.nn.ReLU(inplace=True)
+
+        # 第二个1x1卷积层，用于恢复到输出通道数
+        self.conv2 = torch.nn.Conv2d(hidden_channels, out_channels, kernel_size=1, bias=True)
+
+
+
+    def forward(self, x):
+        # 通过第一个1x1卷积层
+        x = self.conv1(x)
+        # 应用ReLU激活函数
+        x = self.relu(x)
+        # 通过第二个1x1卷积层
+        x = self.conv2(x)
+        # 应用ReLU激活函数
+        x = self.relu(x)
+        return x
+
+
+
+
+
+
+#6.NiN块
+class NiNBlock(torch.nn.Module):
+    """
+    NiN块，包含一个标准的卷积层和一个MLPConv层
+    """
+    def __init__(self, in_channels, num_channels, kernel_size=3, stride=1, padding=1):
+        super(NiNBlock, self).__init__()
+        # 标准的卷积层
+        self.conv = torch.nn.Conv2d(in_channels, num_channels, kernel_size=kernel_size, stride=stride, padding=padding, bias=True)
+        # MLPConv层
+        self.mlpconv = MLPConv(num_channels, num_channels // 2, num_channels)
+
+
+
+
+
+    def forward(self, x):
+        # 通过标准的卷积层
+        x = self.conv(x)
+        # 通过MLPConv层
+        x = self.mlpconv(x)
+        return x
+
+
+
+
+
+
+#7.Network in Network模型
+class NiN(torch.nn.Module):
+    """
+    Network in Network模型
+    输入图片大小为224x224
+    """
+
+    def __init__(self, num_classes=10):
+        super(NiN, self).__init__()
+        # 初始卷积层
+        self.features = torch.nn.Sequential(
+            NiNBlock(3, 96, kernel_size=11, stride=4, padding=0),  # 使用较大的卷积核和步长来减少空间维度
+            torch.nn.MaxPool2d(kernel_size=3, stride=2),  # 最大池化层
+            NiNBlock(96, 256, kernel_size=5, stride=1, padding=2),
+            torch.nn.MaxPool2d(kernel_size=3, stride=2),
+            NiNBlock(256, 384, kernel_size=3, stride=1, padding=1),
+            torch.nn.MaxPool2d(kernel_size=3, stride=2),
+            torch.nn.Dropout(p=0.5),  # 引入Dropout层防止过拟合
+            NiNBlock(384, num_classes, kernel_size=3, stride=1, padding=1),
+            # 使用全局平均池化替代全连接层
+            torch.nn.AdaptiveAvgPool2d((1, 1))
+        )
+
+    def forward(self, x):
+        # 通过特征提取层
+        x = self.features(x)
+        # 将四维张量展平为二维张量
+        x = x.view(x.size(0), -1)
+        # 通过分类器层
+        x = self.classifier(x)
+        return x
+
+
+
+
+
+
+
+
+
+
+
```

### Comparing `pepperpepper-0.0.5.9/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.5.9/setup.py` & `pepperpepper-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.5.9",
+    version="0.0.6",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

