# Comparing `tmp/pepperpepper-0.0.6.1.tar.gz` & `tmp/pepperpepper-0.0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pepperpepper-0.0.6.1.tar", last modified: Thu May  2 07:01:48 2024, max compression
+gzip compressed data, was "pepperpepper-0.0.6.2.tar", last modified: Thu May  2 15:26:07 2024, max compression
```

## Comparing `pepperpepper-0.0.6.1.tar` & `pepperpepper-0.0.6.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.058391 pepperpepper-0.0.6.1/
--rw-rw-rw-   0        0        0      433 2024-05-02 07:01:48.057388 pepperpepper-0.0.6.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.006565 pepperpepper-0.0.6.1/PepperPepper/
--rw-rw-rw-   0        0        0     5179 2024-04-29 03:25:30.000000 pepperpepper-0.0.6.1/PepperPepper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.038715 pepperpepper-0.0.6.1/PepperPepper/callbacks/
--rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.1/PepperPepper/callbacks/__init__.py
--rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.1/PepperPepper/callbacks/custom_callback.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.1/PepperPepper/callbacks/learning_rate_scheduler.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.040985 pepperpepper-0.0.6.1/PepperPepper/core/
--rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.1/PepperPepper/core/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.1/PepperPepper/core/base_model.py
--rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.1/PepperPepper/core/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.045846 pepperpepper-0.0.6.1/PepperPepper/datasets/
--rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/__init__.py
--rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/custom_dataset.py
--rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/image_datasets.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.1/PepperPepper/datasets/text_datasets.py
--rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.1/PepperPepper/environment.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.048052 pepperpepper-0.0.6.1/PepperPepper/examples/
--rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.1/PepperPepper/examples/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.1/PepperPepper/examples/custom_task.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.1/PepperPepper/examples/image_classification.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.1/PepperPepper/examples/text_generation.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.050478 pepperpepper-0.0.6.1/PepperPepper/layers/
--rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.1/PepperPepper/layers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.1/PepperPepper/layers/attention.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.1/PepperPepper/layers/custom_layer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.052053 pepperpepper-0.0.6.1/PepperPepper/losses/
--rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.1/PepperPepper/losses/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.1/PepperPepper/losses/custom_loss.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.055619 pepperpepper-0.0.6.1/PepperPepper/models/
--rw-rw-rw-   0        0        0      990 2024-05-02 06:39:32.000000 pepperpepper-0.0.6.1/PepperPepper/models/__init__.py
--rw-rw-rw-   0        0        0    13242 2024-05-02 07:01:21.000000 pepperpepper-0.0.6.1/PepperPepper/models/cnn.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.1/PepperPepper/models/custom_model.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.1/PepperPepper/models/rnn.py
--rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.1/PepperPepper/models/transformer.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.056386 pepperpepper-0.0.6.1/PepperPepper/optimizers/
--rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.1/PepperPepper/optimizers/__init__.py
--rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.1/PepperPepper/optimizers/custom_optimizer.py
--rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.1/PepperPepper/tools.py
-drwxrwxrwx   0        0        0        0 2024-05-02 07:01:48.057388 pepperpepper-0.0.6.1/PepperPepper.egg-info/
--rw-rw-rw-   0        0        0      433 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1225 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-02 07:01:47.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.1/PepperPepper.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-02 07:01:48.058391 pepperpepper-0.0.6.1/setup.cfg
--rw-rw-rw-   0        0        0      569 2024-05-02 07:01:42.000000 pepperpepper-0.0.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.940295 pepperpepper-0.0.6.2/
+-rw-rw-rw-   0        0        0      433 2024-05-02 15:26:07.936291 pepperpepper-0.0.6.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.846907 pepperpepper-0.0.6.2/PepperPepper/
+-rw-rw-rw-   0        0        0     5142 2024-05-02 15:25:47.000000 pepperpepper-0.0.6.2/PepperPepper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.895025 pepperpepper-0.0.6.2/PepperPepper/callbacks/
+-rw-rw-rw-   0        0        0     1055 2024-04-30 03:51:49.000000 pepperpepper-0.0.6.2/PepperPepper/callbacks/__init__.py
+-rw-rw-rw-   0        0        0     1751 2024-04-30 03:51:20.000000 pepperpepper-0.0.6.2/PepperPepper/callbacks/custom_callback.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:20.000000 pepperpepper-0.0.6.2/PepperPepper/callbacks/learning_rate_scheduler.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.899562 pepperpepper-0.0.6.2/PepperPepper/core/
+-rw-rw-rw-   0        0        0     1028 2024-04-30 03:56:08.000000 pepperpepper-0.0.6.2/PepperPepper/core/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:07.000000 pepperpepper-0.0.6.2/PepperPepper/core/base_model.py
+-rw-rw-rw-   0        0        0     7029 2024-04-30 03:54:40.000000 pepperpepper-0.0.6.2/PepperPepper/core/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.910310 pepperpepper-0.0.6.2/PepperPepper/datasets/
+-rw-rw-rw-   0        0        0     1008 2024-04-29 04:09:47.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/__init__.py
+-rw-rw-rw-   0        0        0        4 2024-04-29 18:10:09.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/custom_dataset.py
+-rw-rw-rw-   0        0        0     2821 2024-04-29 04:06:14.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/image_datasets.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:31.000000 pepperpepper-0.0.6.2/PepperPepper/datasets/text_datasets.py
+-rw-rw-rw-   0        0        0      106 2024-04-30 02:10:15.000000 pepperpepper-0.0.6.2/PepperPepper/environment.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.917204 pepperpepper-0.0.6.2/PepperPepper/examples/
+-rw-rw-rw-   0        0        0     1363 2024-04-26 05:49:55.000000 pepperpepper-0.0.6.2/PepperPepper/examples/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:57.000000 pepperpepper-0.0.6.2/PepperPepper/examples/custom_task.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:42.000000 pepperpepper-0.0.6.2/PepperPepper/examples/image_classification.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:49.000000 pepperpepper-0.0.6.2/PepperPepper/examples/text_generation.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.921018 pepperpepper-0.0.6.2/PepperPepper/layers/
+-rw-rw-rw-   0        0        0     1107 2024-04-26 05:48:42.000000 pepperpepper-0.0.6.2/PepperPepper/layers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:52.000000 pepperpepper-0.0.6.2/PepperPepper/layers/attention.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:59.000000 pepperpepper-0.0.6.2/PepperPepper/layers/custom_layer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.925122 pepperpepper-0.0.6.2/PepperPepper/losses/
+-rw-rw-rw-   0        0        0      966 2024-04-26 05:49:25.000000 pepperpepper-0.0.6.2/PepperPepper/losses/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:30:08.000000 pepperpepper-0.0.6.2/PepperPepper/losses/custom_loss.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.931121 pepperpepper-0.0.6.2/PepperPepper/models/
+-rw-rw-rw-   0        0        0     1100 2024-05-02 09:25:35.000000 pepperpepper-0.0.6.2/PepperPepper/models/__init__.py
+-rw-rw-rw-   0        0        0    21299 2024-05-02 15:24:02.000000 pepperpepper-0.0.6.2/PepperPepper/models/cnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:28:04.000000 pepperpepper-0.0.6.2/PepperPepper/models/custom_model.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:27:47.000000 pepperpepper-0.0.6.2/PepperPepper/models/rnn.py
+-rw-rw-rw-   0        0        0        0 2024-04-30 01:39:29.000000 pepperpepper-0.0.6.2/PepperPepper/models/transformer.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.934338 pepperpepper-0.0.6.2/PepperPepper/optimizers/
+-rw-rw-rw-   0        0        0      878 2024-04-26 05:49:11.000000 pepperpepper-0.0.6.2/PepperPepper/optimizers/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-04-26 05:29:53.000000 pepperpepper-0.0.6.2/PepperPepper/optimizers/custom_optimizer.py
+-rw-rw-rw-   0        0        0      303 2024-04-25 15:51:07.000000 pepperpepper-0.0.6.2/PepperPepper/tools.py
+drwxrwxrwx   0        0        0        0 2024-05-02 15:26:07.935291 pepperpepper-0.0.6.2/PepperPepper.egg-info/
+-rw-rw-rw-   0        0        0      433 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1225 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-02 15:26:07.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-25 18:32:34.000000 pepperpepper-0.0.6.2/PepperPepper.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-02 15:26:07.940295 pepperpepper-0.0.6.2/setup.cfg
+-rw-rw-rw-   0        0        0      569 2024-05-02 15:26:04.000000 pepperpepper-0.0.6.2/setup.py
```

### Comparing `pepperpepper-0.0.6.1/PepperPepper/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 from . import examples
 from . import tools
 
 
 
 __all__ = ['core', 'layers', 'datasets', 'optimizers', 'losses', 'callbacks', 'examples', 'tools']
 
+
+
+
+
 # 你可以在这里添加一些文档字符串，描述这个包的功能和使用方式
 """  
 自定义深度学习包，用于完成深度学习相关的操作和复现代码。  
 
 子模块：  
     core: 包含包的核心功能和基础类。  
     models: 包含各种深度学习模型的实现。  
@@ -32,17 +36,18 @@
 """
 
 
 
 
 
 """
-当规划一个自定义的深度学习包时，合理的包结构对于提高代码的可读性、可维护性和复用性至关重要。以下是一个建议的包结构及其模块命名和功能描述：
+当规划一个自定义的深度学习包时，合理的包结构对于提高代码的可读性、可维护性和复用性至关重要。
+以下是一个建议的包结构及其模块命名和功能描述：
 
-包名: custom_deep_learning
+包名: PepperPepper
 
 模块:
 
 core 模块
 功能：包含包的核心功能和基础类。
 子模块/文件：
 base_model.py：定义基础模型类，提供模型初始化、保存、加载等基础功能。
@@ -93,15 +98,15 @@
 custom_task.py：用户自定义任务的示例。
 这样的包结构使得每个模块都有其明确的功能和职责，方便用户根据需要进行查找和使用。同时，用户还可以根据具体需求在已有模块的基础上进行扩展或添加新的模块。
 """
 
 
 
 """
-在设计您的自定义包结构时，__init__.py 文件起到了非常关键的作用，它用于初始化包，并可以定义一些公共的导入或设置。以下是如何设计您的自定义包结构以及编写 __init__.py 文件的一些建议。
+__init__.py 文件起到了非常关键的作用，它用于初始化包，并可以定义一些公共的导入或设置。以下是如何设计您的自定义包结构以及编写 __init__.py 文件的一些建议。
 
 包结构设计
 首先，根据您之前提供的模块列表，我们可以组织包结构如下：
 
 custom_deep_learning/  
 ├── __init__.py  
 ├── core/
```

### Comparing `pepperpepper-0.0.6.1/PepperPepper/callbacks/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/callbacks/custom_callback.py` & `pepperpepper-0.0.6.2/PepperPepper/callbacks/custom_callback.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/core/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/core/utils.py` & `pepperpepper-0.0.6.2/PepperPepper/core/utils.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/datasets/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/datasets/image_datasets.py` & `pepperpepper-0.0.6.2/PepperPepper/datasets/image_datasets.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/examples/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/layers/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/losses/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper/models/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/models/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,23 +11,30 @@
 from .cnn import LeNet5
 from .cnn import AlexNet
 from .cnn import VGGBlock
 from .cnn import VGG16
 from .cnn import MLPConv
 from .cnn import NiNBlock
 from .cnn import NiN
+from .cnn import InceptionBlockV1
+from .cnn import GoogLeNet
+
+
+
 #from .rnn import RNNModel
 #from .transformer import TransformerModel
 #from .custom_model import CustomModel
 
 
 # __all__ 变量定义了当使用 from models import * 时导入哪些对象
 # 注意：通常不推荐使用 from package import *
 __all__ = [
    'LeNet5',
    'AlexNet',
    'VGGBlock',
    'VGG16',
    'MLPConv',
    'NiNBlock',
-   'NiN'
+   'NiN',
+   'InceptionBlockV1',
+   'GoogLeNet'
 ]
```

### Comparing `pepperpepper-0.0.6.1/PepperPepper/optimizers/__init__.py` & `pepperpepper-0.0.6.2/PepperPepper/optimizers/__init__.py`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/PepperPepper.egg-info/SOURCES.txt` & `pepperpepper-0.0.6.2/PepperPepper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pepperpepper-0.0.6.1/setup.py` & `pepperpepper-0.0.6.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     'torchvision'
 ]
 
 
 
 setuptools.setup(
     name="PepperPepper",
-    version="0.0.6.1",
+    version="0.0.6.2",
     python_requires='>=3.11',
     author="Aohua Li",
     author_email="pepper2024jlu@163.com",
     description="It is a DeepLearning package to foster developed by Aohua Li",
     url="",
     packages=setuptools.find_packages(),
     zip_safe=True,
```

