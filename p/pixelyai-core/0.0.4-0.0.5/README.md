# Comparing `tmp/pixelyai_core-0.0.4.tar.gz` & `tmp/pixelyai_core-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixelyai_core-0.0.4.tar", last modified: Thu Jan  4 17:30:48 2024, max compression
+gzip compressed data, was "pixelyai_core-0.0.5.tar", last modified: Sat Jan  6 09:35:10 2024, max compression
```

## Comparing `pixelyai_core-0.0.4.tar` & `pixelyai_core-0.0.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.419274 pixelyai_core-0.0.4/
--rw-rw-rw-   0        0        0     1506 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     3155 2024-01-04 17:30:48.418275 pixelyai_core-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2198 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/README.md
--rw-rw-rw-   0        0        0      616 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-01-04 17:30:48.419274 pixelyai_core-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1547 2024-01-04 17:30:07.000000 pixelyai_core-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.367541 pixelyai_core-0.0.4/src/
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.369045 pixelyai_core-0.0.4/src/python/
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.397296 pixelyai_core-0.0.4/src/python/pixelyai_core/
--rw-rw-rw-   0        0        0       46 2024-01-04 17:30:07.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.401799 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/
--rw-rw-rw-   0        0        0      536 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/__init__.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.403820 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/
--rw-rw-rw-   0        0        0       45 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/__init__.py
--rw-rw-rw-   0        0        0     6119 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/_serve_module.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.407818 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/inference/
--rw-rw-rw-   0        0        0       33 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/inference/__init__.py
--rw-rw-rw-   0        0        0     1904 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/inference/_setting.py
--rw-rw-rw-   0        0        0     8653 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/inference/inference.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.410818 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/jax_serve/
--rw-rw-rw-   0        0        0       44 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/jax_serve/__init__.py
--rw-rw-rw-   0        0        0     3030 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/jax_serve/_serve_module.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.413273 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/torch_serve/
--rw-rw-rw-   0        0        0       46 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/torch_serve/__init__.py
--rw-rw-rw-   0        0        0     1766 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/torch_serve/_serve_module.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.417275 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/user_interface/
--rw-rw-rw-   0        0        0       56 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/user_interface/__init__.py
--rw-rw-rw-   0        0        0     5419 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/user_interface/_gradio_user_interface.py
--rw-rw-rw-   0        0        0     4362 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/user_interface/_utils.py
--rw-rw-rw-   0        0        0    25323 2024-01-04 16:41:06.000000 pixelyai_core-0.0.4/src/python/pixelyai_core/serving/utils.py
-drwxrwxrwx   0        0        0        0 2024-01-04 17:30:48.395296 pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/
--rw-rw-rw-   0        0        0     3155 2024-01-04 17:30:48.000000 pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2024-01-04 17:30:48.000000 pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-04 17:30:48.000000 pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      241 2024-01-04 17:30:48.000000 pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-01-04 17:30:48.000000 pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/top_level.txt
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1506 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/LICENSE
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3081 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     2198 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/README.md
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      616 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/pyproject.toml
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       38 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/setup.cfg
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1547 2024-01-06 09:35:07.000000 pixelyai_core-0.0.5/setup.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-01-06 09:35:07.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      536 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/__init__.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       45 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     6245 2024-01-06 09:34:43.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/_serve_module.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       33 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1904 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/_setting.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     8653 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/inference.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       44 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3030 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/_serve_module.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       46 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1766 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/_serve_module.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.399007 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       56 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/__init__.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     5419 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/_gradio_user_interface.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     4362 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/_utils.py
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)    25323 2024-01-02 12:03:21.000000 pixelyai_core-0.0.5/src/python/pixelyai_core/serving/utils.py
+drwxrwxr-x   0 erfan     (1000) erfan     (1000)        0 2024-01-06 09:35:10.395007 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     3081 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/PKG-INFO
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)     1146 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/SOURCES.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)        1 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/dependency_links.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)      241 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/requires.txt
+-rw-rw-r--   0 erfan     (1000) erfan     (1000)       14 2024-01-06 09:35:10.000000 pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/top_level.txt
```

### Comparing `pixelyai_core-0.0.4/LICENSE` & `pixelyai_core-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/PKG-INFO` & `pixelyai_core-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: pixelyai_core
-Version: 0.0.4
-Summary: Serve Utilises of PixelyAI
-Home-page: https://github.com/erfanzar/PixelyAI
-Author: Erfan Zare Chavoshi
-Author-email: erfanzare82@eyahoo.com
-Keywords: machine learning,deep learning,pytorch,jax,flax,ggml,c++
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## PixelyAI CoreðŸ§¬
-
-### Introduction
-
-PixelyAI Core is the core component of PixelyAI, an AI assistant that helps businesses manage their customers and their
-team more effectively. It provides a suite of tools for hosting and interacting with large language models (LLMs),
-making it easy to integrate these powerful AI capabilities into your applications.
-
-### Key Features
-
-* **Support for Multiple Backends:** PixelyAI Core supports three popular backends for hosting LLMs: `GGMLServe`,
-  `TorchServe`, and `JaxServe`. This flexibility allows you to choose the backend that best suits your needs and
-  infrastructure.
-
-* **Simplified API:** PixelyAI Core provides an easy-to-use API for interacting with LLMs. This API makes it simple to
-  send queries to LLMs, receive responses, and handle errors.
-
-* **Gradio Integration:** PixelyAI Core integrates seamlessly with `Gradio`, a web framework for building interactive AI
-  applications. This integration allows you to create intuitive interfaces for interacting with `LLMs`, making it easier
-  for users to access their capabilities.
-
-### Benefits
-
-* **Improved Customer Support:** Empower your customer support team with conversational AI capabilities, enabling them
-  to provide more personalized and efficient support.
-
-* **Enhanced Team Collaboration:** Facilitate knowledge sharing and collaboration among team members through natural
-  language interactions.
-
-* **Automated Task Delegation:** Automate routine tasks, such as report generation and data analysis, freeing up team
-  members to focus on more strategic initiatives.
-
-### Getting Started
-
-To install PixelyAI Core, simply use the following command:
-
-```bash
-pip install pixelyai-core
-```
-
-Once installed, you can start using the PixelyAI Core API to interact with LLMs. For more information, please refer to
-the official documentation.
-
-### Conclusion
-
-PixelyAI Core is a powerful tool for businesses seeking to leverage the capabilities of LLMs to improve their customer
-service, collaboration, and productivity. With its support for multiple backends, simplified API, PixelyAI Core provides
-a versatile and user-friendly platform for integrating LLMs into your applications.
+Metadata-Version: 2.1
+Name: pixelyai_core
+Version: 0.0.5
+Summary: Serve Utilises of PixelyAI
+Home-page: https://github.com/erfanzar/PixelyAI
+Author: Erfan Zare Chavoshi
+Author-email: erfanzare82@eyahoo.com
+Keywords: machine learning,deep learning,pytorch,jax,flax,ggml,c++
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## PixelyAI Core🧬
+
+### Introduction
+
+PixelyAI Core is the core component of PixelyAI, an AI assistant that helps businesses manage their customers and their
+team more effectively. It provides a suite of tools for hosting and interacting with large language models (LLMs),
+making it easy to integrate these powerful AI capabilities into your applications.
+
+### Key Features
+
+* **Support for Multiple Backends:** PixelyAI Core supports three popular backends for hosting LLMs: `GGMLServe`,
+  `TorchServe`, and `JaxServe`. This flexibility allows you to choose the backend that best suits your needs and
+  infrastructure.
+
+* **Simplified API:** PixelyAI Core provides an easy-to-use API for interacting with LLMs. This API makes it simple to
+  send queries to LLMs, receive responses, and handle errors.
+
+* **Gradio Integration:** PixelyAI Core integrates seamlessly with `Gradio`, a web framework for building interactive AI
+  applications. This integration allows you to create intuitive interfaces for interacting with `LLMs`, making it easier
+  for users to access their capabilities.
+
+### Benefits
+
+* **Improved Customer Support:** Empower your customer support team with conversational AI capabilities, enabling them
+  to provide more personalized and efficient support.
+
+* **Enhanced Team Collaboration:** Facilitate knowledge sharing and collaboration among team members through natural
+  language interactions.
+
+* **Automated Task Delegation:** Automate routine tasks, such as report generation and data analysis, freeing up team
+  members to focus on more strategic initiatives.
+
+### Getting Started
+
+To install PixelyAI Core, simply use the following command:
+
+```bash
+pip install pixelyai-core
+```
+
+Once installed, you can start using the PixelyAI Core API to interact with LLMs. For more information, please refer to
+the official documentation.
+
+### Conclusion
+
+PixelyAI Core is a powerful tool for businesses seeking to leverage the capabilities of LLMs to improve their customer
+service, collaboration, and productivity. With its support for multiple backends, simplified API, PixelyAI Core provides
+a versatile and user-friendly platform for integrating LLMs into your applications.
```

### Comparing `pixelyai_core-0.0.4/README.md` & `pixelyai_core-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/pyproject.toml` & `pixelyai_core-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/setup.py` & `pixelyai_core-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pixelyai_core",
-    version="0.0.4",
+    version="0.0.5",
     author="Erfan Zare Chavoshi",
     author_email="erfanzare82@eyahoo.com",
     description="Serve Utilises of PixelyAI",
     url="https://github.com/erfanzar/PixelyAI",
     packages=find_packages("src/python"),
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
```

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/__init__.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/__init__.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/_serve_module.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/_serve_module.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,31 +144,34 @@
 
     def launch(
             self,
             launch_custom: bool = True,
             launch_chat: bool = True,
             share: bool = True,
             extra_options: dict | None = None,
+            server_name: str | None = None,
             *args,
             **kwargs
     ):
         extra_options = extra_options if extra_options is not None else {}
         urls = {}
         if launch_custom:
             self.gradio_app_custom.launch(
                 share=share,
+                server_name=server_name,
                 **extra_options
             )
             urls["custom"] = self.gradio_app_custom.share_url
         if launch_chat:
             grad_chat = self.build_inference(
                 self.process_gradio, 2048, 2048, 1
             )
             grad_chat.launch(
                 share=share,
+                server_name=server_name,
                 **extra_options
             )
             urls["chat"] = grad_chat.share_url
         return urls
 
     @staticmethod
     def format_chat(history: List[List[str]], prompt: str, system: str = None) -> str:
```

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/inference/_setting.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/_setting.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/ggml_serve/inference/inference.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/ggml_serve/inference/inference.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/jax_serve/_serve_module.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/jax_serve/_serve_module.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/torch_serve/_serve_module.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/torch_serve/_serve_module.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/user_interface/_gradio_user_interface.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/_gradio_user_interface.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/user_interface/_utils.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/user_interface/_utils.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core/serving/utils.py` & `pixelyai_core-0.0.5/src/python/pixelyai_core/serving/utils.py`

 * *Files identical despite different names*

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/PKG-INFO` & `pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-Metadata-Version: 2.1
-Name: pixelyai-core
-Version: 0.0.4
-Summary: Serve Utilises of PixelyAI
-Home-page: https://github.com/erfanzar/PixelyAI
-Author: Erfan Zare Chavoshi
-Author-email: erfanzare82@eyahoo.com
-Keywords: machine learning,deep learning,pytorch,jax,flax,ggml,c++
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## PixelyAI CoreðŸ§¬
-
-### Introduction
-
-PixelyAI Core is the core component of PixelyAI, an AI assistant that helps businesses manage their customers and their
-team more effectively. It provides a suite of tools for hosting and interacting with large language models (LLMs),
-making it easy to integrate these powerful AI capabilities into your applications.
-
-### Key Features
-
-* **Support for Multiple Backends:** PixelyAI Core supports three popular backends for hosting LLMs: `GGMLServe`,
-  `TorchServe`, and `JaxServe`. This flexibility allows you to choose the backend that best suits your needs and
-  infrastructure.
-
-* **Simplified API:** PixelyAI Core provides an easy-to-use API for interacting with LLMs. This API makes it simple to
-  send queries to LLMs, receive responses, and handle errors.
-
-* **Gradio Integration:** PixelyAI Core integrates seamlessly with `Gradio`, a web framework for building interactive AI
-  applications. This integration allows you to create intuitive interfaces for interacting with `LLMs`, making it easier
-  for users to access their capabilities.
-
-### Benefits
-
-* **Improved Customer Support:** Empower your customer support team with conversational AI capabilities, enabling them
-  to provide more personalized and efficient support.
-
-* **Enhanced Team Collaboration:** Facilitate knowledge sharing and collaboration among team members through natural
-  language interactions.
-
-* **Automated Task Delegation:** Automate routine tasks, such as report generation and data analysis, freeing up team
-  members to focus on more strategic initiatives.
-
-### Getting Started
-
-To install PixelyAI Core, simply use the following command:
-
-```bash
-pip install pixelyai-core
-```
-
-Once installed, you can start using the PixelyAI Core API to interact with LLMs. For more information, please refer to
-the official documentation.
-
-### Conclusion
-
-PixelyAI Core is a powerful tool for businesses seeking to leverage the capabilities of LLMs to improve their customer
-service, collaboration, and productivity. With its support for multiple backends, simplified API, PixelyAI Core provides
-a versatile and user-friendly platform for integrating LLMs into your applications.
+Metadata-Version: 2.1
+Name: pixelyai-core
+Version: 0.0.5
+Summary: Serve Utilises of PixelyAI
+Home-page: https://github.com/erfanzar/PixelyAI
+Author: Erfan Zare Chavoshi
+Author-email: erfanzare82@eyahoo.com
+Keywords: machine learning,deep learning,pytorch,jax,flax,ggml,c++
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## PixelyAI Core🧬
+
+### Introduction
+
+PixelyAI Core is the core component of PixelyAI, an AI assistant that helps businesses manage their customers and their
+team more effectively. It provides a suite of tools for hosting and interacting with large language models (LLMs),
+making it easy to integrate these powerful AI capabilities into your applications.
+
+### Key Features
+
+* **Support for Multiple Backends:** PixelyAI Core supports three popular backends for hosting LLMs: `GGMLServe`,
+  `TorchServe`, and `JaxServe`. This flexibility allows you to choose the backend that best suits your needs and
+  infrastructure.
+
+* **Simplified API:** PixelyAI Core provides an easy-to-use API for interacting with LLMs. This API makes it simple to
+  send queries to LLMs, receive responses, and handle errors.
+
+* **Gradio Integration:** PixelyAI Core integrates seamlessly with `Gradio`, a web framework for building interactive AI
+  applications. This integration allows you to create intuitive interfaces for interacting with `LLMs`, making it easier
+  for users to access their capabilities.
+
+### Benefits
+
+* **Improved Customer Support:** Empower your customer support team with conversational AI capabilities, enabling them
+  to provide more personalized and efficient support.
+
+* **Enhanced Team Collaboration:** Facilitate knowledge sharing and collaboration among team members through natural
+  language interactions.
+
+* **Automated Task Delegation:** Automate routine tasks, such as report generation and data analysis, freeing up team
+  members to focus on more strategic initiatives.
+
+### Getting Started
+
+To install PixelyAI Core, simply use the following command:
+
+```bash
+pip install pixelyai-core
+```
+
+Once installed, you can start using the PixelyAI Core API to interact with LLMs. For more information, please refer to
+the official documentation.
+
+### Conclusion
+
+PixelyAI Core is a powerful tool for businesses seeking to leverage the capabilities of LLMs to improve their customer
+service, collaboration, and productivity. With its support for multiple backends, simplified API, PixelyAI Core provides
+a versatile and user-friendly platform for integrating LLMs into your applications.
```

### Comparing `pixelyai_core-0.0.4/src/python/pixelyai_core.egg-info/SOURCES.txt` & `pixelyai_core-0.0.5/src/python/pixelyai_core.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-src/python/pixelyai_core.egg-info/PKG-INFO
-src/python/pixelyai_core.egg-info/SOURCES.txt
-src/python/pixelyai_core.egg-info/dependency_links.txt
-src/python/pixelyai_core.egg-info/requires.txt
-src/python/pixelyai_core.egg-info/top_level.txt
 src/python/pixelyai_core/__init__.py
 src/python/pixelyai_core.egg-info/PKG-INFO
 src/python/pixelyai_core.egg-info/SOURCES.txt
 src/python/pixelyai_core.egg-info/dependency_links.txt
 src/python/pixelyai_core.egg-info/requires.txt
 src/python/pixelyai_core.egg-info/top_level.txt
 src/python/pixelyai_core/serving/__init__.py
```

