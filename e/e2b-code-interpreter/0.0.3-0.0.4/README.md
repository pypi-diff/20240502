# Comparing `tmp/e2b_code_interpreter-0.0.3.tar.gz` & `tmp/e2b_code_interpreter-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2b_code_interpreter-0.0.3.tar", max compression
+gzip compressed data, was "e2b_code_interpreter-0.0.4.tar", max compression
```

## Comparing `e2b_code_interpreter-0.0.3.tar` & `e2b_code_interpreter-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     3173 2024-04-05 04:56:42.544807 e2b_code_interpreter-0.0.3/README.md
--rw-r--r--   0        0        0      114 2024-04-05 04:56:42.544807 e2b_code_interpreter-0.0.3/e2b_code_interpreter/__init__.py
--rw-r--r--   0        0        0    11060 2024-04-05 04:56:42.544807 e2b_code_interpreter-0.0.3/e2b_code_interpreter/main.py
--rw-r--r--   0        0        0     9056 2024-04-05 04:56:42.548807 e2b_code_interpreter-0.0.3/e2b_code_interpreter/messaging.py
--rw-r--r--   0        0        0     7017 2024-04-05 04:56:42.548807 e2b_code_interpreter-0.0.3/e2b_code_interpreter/models.py
--rw-r--r--   0        0        0      768 2024-04-05 04:57:09.432918 e2b_code_interpreter-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4089 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     2331 2024-05-02 04:32:07.475102 e2b_code_interpreter-0.0.4/README.md
+-rw-r--r--   0        0        0      149 2024-05-02 04:32:07.475102 e2b_code_interpreter-0.0.4/e2b_code_interpreter/__init__.py
+-rw-r--r--   0        0        0    11061 2024-05-02 04:32:07.475102 e2b_code_interpreter-0.0.4/e2b_code_interpreter/main.py
+-rw-r--r--   0        0        0     9056 2024-05-02 04:32:07.475102 e2b_code_interpreter-0.0.4/e2b_code_interpreter/messaging.py
+-rw-r--r--   0        0        0     7188 2024-05-02 04:32:07.475102 e2b_code_interpreter-0.0.4/e2b_code_interpreter/models.py
+-rw-r--r--   0        0        0      766 2024-05-02 04:32:32.051163 e2b_code_interpreter-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 e2b_code_interpreter-0.0.4/PKG-INFO
```

### Comparing `e2b_code_interpreter-0.0.3/README.md` & `e2b_code_interpreter-0.0.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,30 @@
+Metadata-Version: 2.1
+Name: e2b-code-interpreter
+Version: 0.0.4
+Summary: E2B Code Interpreter - Stateful code execution
+Home-page: https://e2b.dev/
+License: Apache-2.0
+Author: e2b
+Author-email: hello@e2b.dev
+Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: e2b (>=0.17.0)
+Requires-Dist: pydantic (>1,<3)
+Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
+Project-URL: Bug Tracker, https://github.com/e2b-dev/code-interpreter/issues
+Project-URL: Repository, https://github.com/e2b-dev/e2b-code-interpreter/tree/python
+Description-Content-Type: text/markdown
+
 # Code interpreter extension for Python
 
 The repository contains a template and modules for the code interpreter sandbox. It is based on the Jupyter server and implements the Jupyter Kernel messaging protocol. This allows for sharing context between code executions and improves support for plotting charts and other display-able data.
 
 ## Key Features
 
 - **Stateful Execution**: Unlike traditional sandboxes that treat each code execution independently, this package maintains context across executions.
@@ -85,48 +108,7 @@
 print("world")
 """
 
 with CodeInterpreter() as sandbox:
     sandbox.notebook.exec_cell(code, on_stdout=print, on_stderr=print, on_result=(lambda result: print(result.text)))
 ```
 
-### Pre-installed Python packages inside the sandbox
-
-The full and always up-to-date list can be found in the [`requirements.txt`](https://github.com/e2b-dev/E2B/blob/stateful-code-interpreter/sandboxes/code-interpreter-stateful/requirements.txt) file.
-
-```text
-# Jupyter server requirements
-jupyter-server==2.13.0
-ipykernel==6.29.3
-ipython==8.22.2
-
-# Other packages
-aiohttp==3.9.3
-beautifulsoup4==4.12.3
-bokeh==3.3.4
-gensim==4.3.2
-imageio==2.34.0
-joblib==1.3.2
-librosa==0.10.1
-matplotlib==3.8.3
-nltk==3.8.1
-numpy==1.26.4
-opencv-python==4.9.0.80
-openpyxl==3.1.2
-pandas==1.5.3
-plotly==5.19.0
-pytest==8.1.0
-python-docx==1.1.0
-pytz==2024.1
-requests==2.26.0
-scikit-image==0.22.0
-scikit-learn==1.4.1.post1
-scipy==1.12.0
-seaborn==0.13.2
-soundfile==0.12.1
-spacy==3.7.4
-textblob==0.18.0
-tornado==6.4
-urllib3==1.26.7
-xarray==2024.2.0
-xlrd==2.0.1
-```
```

### Comparing `e2b_code_interpreter-0.0.3/e2b_code_interpreter/main.py` & `e2b_code_interpreter-0.0.4/e2b_code_interpreter/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 import logging
 import threading
+import requests
+
 from concurrent.futures import Future
 from typing import Any, Callable, List, Optional, Dict
 
-import requests
 from e2b import EnvVars, ProcessMessage, Sandbox
 from e2b.constants import TIMEOUT
 
 from e2b_code_interpreter.messaging import JupyterKernelWebSocket
 from e2b_code_interpreter.models import KernelException, Execution, Result
 
 logger = logging.getLogger(__name__)
```

### Comparing `e2b_code_interpreter-0.0.3/e2b_code_interpreter/messaging.py` & `e2b_code_interpreter-0.0.4/e2b_code_interpreter/messaging.py`

 * *Files identical despite different names*

### Comparing `e2b_code_interpreter-0.0.3/e2b_code_interpreter/models.py` & `e2b_code_interpreter-0.0.4/e2b_code_interpreter/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,14 +75,20 @@
         self.jpeg = data.pop("image/jpeg", None)
         self.pdf = data.pop("application/pdf", None)
         self.latex = data.pop("text/latex", None)
         self.json = data.pop("application/json", None)
         self.javascript = data.pop("application/javascript", None)
         self.extra = data
 
+    # Allows to iterate over formats()
+    def __getitem__(self, item):
+        if item in self.raw:
+            return self.raw[item]
+        return getattr(self, item)
+
     def formats(self) -> Iterable[str]:
         """
         Returns all available formats of the result.
 
         :return: All available formats of the result in MIME types.
         """
         formats = []
```

### Comparing `e2b_code_interpreter-0.0.3/pyproject.toml` & `e2b_code_interpreter-0.0.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "e2b-code-interpreter"
-version = "0.0.3"
+version = "0.0.4"
 description = "E2B Code Interpreter - Stateful code execution"
 authors = ["e2b <hello@e2b.dev>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://e2b.dev/"
 repository = "https://github.com/e2b-dev/e2b-code-interpreter/tree/python"
 packages = [{ include = "e2b_code_interpreter" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
-e2b = ">=0.14.11"
 pydantic = ">1, <3"
 websocket-client = "^1.7.0"
+e2b = ">=0.17.0"
 
 [tool.poetry.group.dev.dependencies]
 black = "^24.3.0"
 pytest = "^7.4.0"
 python-dotenv = "^1.0.0"
 pytest-dotenv = "^0.5.2"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/e2b-dev/code-interpreter/issues"
```

