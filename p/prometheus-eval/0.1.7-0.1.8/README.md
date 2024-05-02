# Comparing `tmp/prometheus_eval-0.1.7.tar.gz` & `tmp/prometheus_eval-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prometheus_eval-0.1.7.tar", max compression
+gzip compressed data, was "prometheus_eval-0.1.8.tar", max compression
```

## Comparing `prometheus_eval-0.1.7.tar` & `prometheus_eval-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.7/README.md
--rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.7/prometheus_eval/__init__.py
--rw-r--r--   0        0        0     9355 2024-05-01 14:42:02.809346 prometheus_eval-0.1.7/prometheus_eval/judge.py
--rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.7/prometheus_eval/prompts.py
--rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.7/prometheus_eval/utils.py
--rw-r--r--   0        0        0     2142 2024-05-01 14:51:19.783489 prometheus_eval-0.1.7/prometheus_eval/vllm.py
--rw-r--r--   0        0        0      595 2024-05-01 14:51:28.075520 prometheus_eval-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-01 11:39:59.068594 prometheus_eval-0.1.8/README.md
+-rw-r--r--   0        0        0      230 2024-05-01 13:51:32.126311 prometheus_eval-0.1.8/prometheus_eval/__init__.py
+-rw-r--r--   0        0        0     9355 2024-05-01 14:42:02.809346 prometheus_eval-0.1.8/prometheus_eval/judge.py
+-rw-r--r--   0        0        0     5786 2024-05-01 13:42:46.303450 prometheus_eval-0.1.8/prometheus_eval/prompts.py
+-rw-r--r--   0        0        0     7448 2024-05-01 13:42:57.411514 prometheus_eval-0.1.8/prometheus_eval/utils.py
+-rw-r--r--   0        0        0     2113 2024-05-01 14:52:44.731804 prometheus_eval-0.1.8/prometheus_eval/vllm.py
+-rw-r--r--   0        0        0      595 2024-05-01 14:52:48.063817 prometheus_eval-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      540 1970-01-01 00:00:00.000000 prometheus_eval-0.1.8/PKG-INFO
```

### Comparing `prometheus_eval-0.1.7/prometheus_eval/judge.py` & `prometheus_eval-0.1.8/prometheus_eval/judge.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.7/prometheus_eval/prompts.py` & `prometheus_eval-0.1.8/prometheus_eval/prompts.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.7/prometheus_eval/utils.py` & `prometheus_eval-0.1.8/prometheus_eval/utils.py`

 * *Files identical despite different names*

### Comparing `prometheus_eval-0.1.7/prometheus_eval/vllm.py` & `prometheus_eval-0.1.8/prometheus_eval/vllm.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,16 @@
         name: str,
         num_gpus: int = 1,
         download_dir: Optional[str] = None,
         dtype: str = "auto",
         gpu_memory_utilization: int = 0.8,
         **kwargs,
     ) -> None:
-        dtype: str = "auto"
         self.name: str = name
 
-
         self.model: LLM = LLM(
             model=self.name,
             tensor_parallel_size=num_gpus,
             dtype=dtype,
             gpu_memory_utilization=gpu_memory_utilization,
             download_dir=download_dir,
             **kwargs
```

### Comparing `prometheus_eval-0.1.7/pyproject.toml` & `prometheus_eval-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prometheus-eval"
-version = "0.1.7"
+version = "0.1.8"
 description = "A package for evaluating the performance of language models with Prometheus"
 authors = ["Juyoung Suk <juyoung@kaist.ac.kr>", "Seungone Kim <seungone@cmu.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 vllm = "<0.4.0"
```

### Comparing `prometheus_eval-0.1.7/PKG-INFO` & `prometheus_eval-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prometheus-eval
-Version: 0.1.7
+Version: 0.1.8
 Summary: A package for evaluating the performance of language models with Prometheus
 Author: Juyoung Suk
 Author-email: juyoung@kaist.ac.kr
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

