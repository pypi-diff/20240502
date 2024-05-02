# Comparing `tmp/nvidia_dali_nightly_cuda120-1.38.0.dev20240430.tar.gz` & `tmp/nvidia_dali_nightly_cuda120-1.38.0.dev20240501.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvidia_dali_nightly_cuda120-1.38.0.dev20240430.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
+gzip compressed data, was "nvidia_dali_nightly_cuda120-1.38.0.dev20240501.tar", last modified: Mon Apr  5 07:00:00 1993, max compression
```

## Comparing `nvidia_dali_nightly_cuda120-1.38.0.dev20240430.tar` & `nvidia_dali_nightly_cuda120-1.38.0.dev20240501.tar`

### PKG-INFO

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: nvidia-dali-nightly-cuda120
-Version: 1.38.0.dev20240430
-Summary: NVIDIA DALI nightly  for CUDA 12.0. Git SHA: 82983535cd65dc1ba11018b4b35dbae6e2c305d5
+Version: 1.38.0.dev20240501
+Summary: NVIDIA DALI nightly  for CUDA 12.0. Git SHA: 80b67f93fcbd57985b35db94e9788602334ea37f
 Home-page: https://github.com/NVIDIA/dali
 Author: NVIDIA Corporation
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

