# Comparing `tmp/spaces-0.9b2.tar.gz` & `tmp/spaces-0.9b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spaces-0.9b2.tar", max compression
+gzip compressed data, was "spaces-0.9b3.tar", max compression
```

## Comparing `spaces-0.9b2.tar` & `spaces-0.9b3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.9b2/README.md
--rw-r--r--   0        0        0     1524 2023-07-19 13:54:39.025113 spaces-0.9b2/pyproject.toml
--rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.9b2/spaces/__init__.py
--rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.9b2/spaces/config.py
--rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.9b2/spaces/gpu/__init__.py
--rw-r--r--   0        0        0     2670 2023-07-19 13:53:10.399065 spaces-0.9b2/spaces/gpu/client.py
--rw-r--r--   0        0        0     1650 2023-07-19 11:04:13.597888 spaces-0.9b2/spaces/gpu/decorator.py
--rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.9b2/spaces/gpu/torch.py
--rw-r--r--   0        0        0     7768 2023-07-19 11:04:13.597888 spaces-0.9b2/spaces/gpu/wrappers.py
--rw-r--r--   0        0        0     1264 2023-07-19 11:04:13.597888 spaces-0.9b2/spaces/gradio.py
--rw-r--r--   0        0        0     1198 2023-07-19 11:04:13.597888 spaces-0.9b2/spaces/utils.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.9b2/setup.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.9b2/PKG-INFO
+-rw-r--r--   0        0        0       61 2023-02-23 09:04:36.869652 spaces-0.9b3/README.md
+-rw-r--r--   0        0        0     1524 2023-07-19 15:29:42.569453 spaces-0.9b3/pyproject.toml
+-rw-r--r--   0        0        0      212 2023-06-30 09:31:31.779698 spaces-0.9b3/spaces/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-30 09:32:40.450793 spaces-0.9b3/spaces/config.py
+-rw-r--r--   0        0        0      262 2023-06-30 15:54:25.725430 spaces-0.9b3/spaces/gpu/__init__.py
+-rw-r--r--   0        0        0     2794 2023-07-19 15:21:36.336343 spaces-0.9b3/spaces/gpu/client.py
+-rw-r--r--   0        0        0     1650 2023-07-19 11:04:13.597888 spaces-0.9b3/spaces/gpu/decorator.py
+-rw-r--r--   0        0        0     3573 2023-07-07 16:29:17.706242 spaces-0.9b3/spaces/gpu/torch.py
+-rw-r--r--   0        0        0     7768 2023-07-19 11:04:13.597888 spaces-0.9b3/spaces/gpu/wrappers.py
+-rw-r--r--   0        0        0     1264 2023-07-19 11:04:13.597888 spaces-0.9b3/spaces/gradio.py
+-rw-r--r--   0        0        0     1198 2023-07-19 11:04:13.597888 spaces-0.9b3/spaces/utils.py
+-rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 spaces-0.9b3/setup.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 spaces-0.9b3/PKG-INFO
```

### Comparing `spaces-0.9b2/pyproject.toml` & `spaces-0.9b3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "spaces"
-version = "0.9b2"
+version = "0.9b3"
 description = "Utilities for Hugging Face Spaces"
 authors = ["Charles Bensimon <charles@huggingface.co>"]
 readme = "README.md"
 homepage = "https://huggingface.co"
 repository = "https://github.com/huggingface/huggingface_hub"
 license = "Apache-2.0"
```

### Comparing `spaces-0.9b2/spaces/gpu/client.py` & `spaces-0.9b3/spaces/gpu/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,18 +51,23 @@
             raise RuntimeError("Error while initializing ZeroGPU: NotFound")
     if status != HTTPStatus.OK: # pragma: no cover
         raise RuntimeError("Error while initializing ZeroGPU: Unknown")
 
 
 def schedule(task_id: int, request: gr.Request) -> ScheduleResponse:
 
-    if not hasattr(request, 'headers') or not hasattr(request.headers, '__dict__'):
+    headers = getattr(request, 'headers', None)
+    if headers is None or not hasattr(headers, '__dict__'):
         raise gr.Error("Internal Gradio error")
 
-    if not (token := request.headers.__dict__.get(TOKEN_HEADER.lower())):
+    # Compatibility trick
+    if not hasattr(headers, 'get'):
+        headers = headers.__dict__ # pragma: no cover
+
+    if not (token := headers.get(TOKEN_HEADER.lower())):
         raise gr.Error("Internal infra error")
 
     res = post('/schedule', params=ScheduleParams(
         cgroupPath=CGROUP_PATH,
         taskId=task_id,
         token=token,
     ))
```

### Comparing `spaces-0.9b2/spaces/gpu/decorator.py` & `spaces-0.9b3/spaces/gpu/decorator.py`

 * *Files identical despite different names*

### Comparing `spaces-0.9b2/spaces/gpu/torch.py` & `spaces-0.9b3/spaces/gpu/torch.py`

 * *Files identical despite different names*

### Comparing `spaces-0.9b2/spaces/gpu/wrappers.py` & `spaces-0.9b3/spaces/gpu/wrappers.py`

 * *Files identical despite different names*

### Comparing `spaces-0.9b2/spaces/gradio.py` & `spaces-0.9b3/spaces/gradio.py`

 * *Files identical despite different names*

### Comparing `spaces-0.9b2/spaces/utils.py` & `spaces-0.9b3/spaces/utils.py`

 * *Files identical despite different names*

### Comparing `spaces-0.9b2/setup.py` & `spaces-0.9b3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
  'psutil>=5.9.5,<6.0.0',
  'pydantic>=1.10.8,<2.0.0',
  'requests>=2.29.0,<3.0.0',
  'typing-extensions>=4.5.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'spaces',
-    'version': '0.9b2',
+    'version': '0.9b3',
     'description': 'Utilities for Hugging Face Spaces',
     'long_description': '# Hugging Face Spaces\n\n## Installation\n\n`pip install spaces`\n',
     'author': 'Charles Bensimon',
     'author_email': 'charles@huggingface.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://huggingface.co',
```

### Comparing `spaces-0.9b2/PKG-INFO` & `spaces-0.9b3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spaces
-Version: 0.9b2
+Version: 0.9b3
 Summary: Utilities for Hugging Face Spaces
 Home-page: https://huggingface.co
 License: Apache-2.0
 Author: Charles Bensimon
 Author-email: charles@huggingface.co
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

