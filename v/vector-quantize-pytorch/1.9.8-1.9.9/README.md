# Comparing `tmp/vector_quantize_pytorch-1.9.8.tar.gz` & `tmp/vector_quantize_pytorch-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vector_quantize_pytorch-1.9.8.tar", last modified: Mon Oct 16 15:27:26 2023, max compression
+gzip compressed data, was "vector_quantize_pytorch-1.9.9.tar", last modified: Mon Oct 16 15:34:34 2023, max compression
```

## Comparing `vector_quantize_pytorch-1.9.8.tar` & `vector_quantize_pytorch-1.9.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:27:26.499554 vector_quantize_pytorch-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-16 15:27:26.495554 vector_quantize_pytorch-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    19583 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 15:27:26.499554 vector_quantize_pytorch-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:27:26.495554 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/finite_scalar_quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)     6690 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/lookup_free_quantization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/random_projection_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9567 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/residual_vq.py
--rw-r--r--   0 runner    (1001) docker     (127)    36722 2023-10-16 15:27:15.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/vector_quantize_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:27:26.495554 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-16 15:27:26.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-16 15:27:26.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 15:27:26.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-16 15:27:26.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-16 15:27:26.000000 vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:34:34.288930 vector_quantize_pytorch-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-16 15:34:34.288930 vector_quantize_pytorch-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    19583 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 15:34:34.288930 vector_quantize_pytorch-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:34:34.288930 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/finite_scalar_quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/lookup_free_quantization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/random_projection_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9567 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/residual_vq.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36722 2023-10-16 15:34:22.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/vector_quantize_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 15:34:34.288930 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2023-10-16 15:34:34.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2023-10-16 15:34:34.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 15:34:34.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2023-10-16 15:34:34.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-16 15:34:34.000000 vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/top_level.txt
```

### Comparing `vector_quantize_pytorch-1.9.8/LICENSE` & `vector_quantize_pytorch-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.9.8/PKG-INFO` & `vector_quantize_pytorch-1.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector_quantize_pytorch
-Version: 1.9.8
+Version: 1.9.9
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.9.8/README.md` & `vector_quantize_pytorch-1.9.9/README.md`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.9.8/setup.py` & `vector_quantize_pytorch-1.9.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'vector_quantize_pytorch',
   packages = find_packages(),
-  version = '1.9.8',
+  version = '1.9.9',
   license='MIT',
   description = 'Vector Quantization - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/vector-quantizer-pytorch',
   keywords = [
```

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/finite_scalar_quantization.py` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/finite_scalar_quantization.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/lookup_free_quantization.py` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/lookup_free_quantization.py`

 * *Files 2% similar despite different names*

```diff
@@ -197,15 +197,15 @@
         else:
             # if not training, just return dummy 0
             entropy_aux_loss = self.zero
 
         # commit loss
 
         if self.training:
-            commit_loss = F.mse_loss(original_input, quantized)
+            commit_loss = F.mse_loss(original_input, quantized.detach())
         else:
             commit_loss = self.zero
 
         # merge back codebook dim
 
         x = rearrange(x, 'b n c d -> b n (c d)')
```

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/random_projection_quantizer.py` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/random_projection_quantizer.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/residual_vq.py` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/residual_vq.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch/vector_quantize_pytorch.py` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch/vector_quantize_pytorch.py`

 * *Files identical despite different names*

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/PKG-INFO` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vector-quantize-pytorch
-Version: 1.9.8
+Version: 1.9.9
 Summary: Vector Quantization - Pytorch
 Home-page: https://github.com/lucidrains/vector-quantizer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,pytorch,quantization
 Classifier: Development Status :: 4 - Beta
```

### Comparing `vector_quantize_pytorch-1.9.8/vector_quantize_pytorch.egg-info/SOURCES.txt` & `vector_quantize_pytorch-1.9.9/vector_quantize_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

