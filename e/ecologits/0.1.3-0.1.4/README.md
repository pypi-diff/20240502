# Comparing `tmp/ecologits-0.1.3.tar.gz` & `tmp/ecologits-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecologits-0.1.3.tar", max compression
+gzip compressed data, was "ecologits-0.1.4.tar", max compression
```

## Comparing `ecologits-0.1.3.tar` & `ecologits-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    16725 2024-04-30 16:58:29.732136 ecologits-0.1.3/LICENSE
--rw-r--r--   0        0        0     2243 2024-04-30 16:58:29.732136 ecologits-0.1.3/README.md
--rw-r--r--   0        0        0       80 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/__init__.py
--rw-r--r--   0        0        0    11901 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/data/models.csv
--rw-r--r--   0        0        0     2798 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/ecologits.py
--rw-r--r--   0        0        0      140 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/exceptions.py
--rw-r--r--   0        0        0      121 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/__init__.py
--rw-r--r--   0        0        0     1468 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/dag.py
--rw-r--r--   0        0        0    14956 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/llm.py
--rw-r--r--   0        0        0     4066 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/impacts/models.py
--rw-r--r--   0        0        0     2992 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/model_repository.py
--rw-r--r--   0        0        0        0 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/__init__.py
--rw-r--r--   0        0        0     7848 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/anthropic_tracer.py
--rw-r--r--   0        0        0     5094 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/cohere_tracer.py
--rw-r--r--   0        0        0     5554 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/huggingface_tracer.py
--rw-r--r--   0        0        0     5065 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/mistralai_tracer.py
--rw-r--r--   0        0        0     5313 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/openai_tracer.py
--rw-r--r--   0        0        0     1496 2024-04-30 16:58:29.736136 ecologits-0.1.3/ecologits/tracers/utils.py
--rw-r--r--   0        0        0     3591 2024-04-30 16:58:29.736136 ecologits-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     4428 1970-01-01 00:00:00.000000 ecologits-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    16725 2024-05-02 11:48:09.112273 ecologits-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2367 2024-05-02 11:48:09.112273 ecologits-0.1.4/README.md
+-rw-r--r--   0        0        0       80 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/__init__.py
+-rw-r--r--   0        0        0    11901 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/data/models.csv
+-rw-r--r--   0        0        0     2798 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/ecologits.py
+-rw-r--r--   0        0        0      140 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/exceptions.py
+-rw-r--r--   0        0        0      121 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/impacts/__init__.py
+-rw-r--r--   0        0        0     1468 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/impacts/dag.py
+-rw-r--r--   0        0        0    15276 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/impacts/llm.py
+-rw-r--r--   0        0        0     4066 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/impacts/models.py
+-rw-r--r--   0        0        0     2992 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/model_repository.py
+-rw-r--r--   0        0        0        0 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/__init__.py
+-rw-r--r--   0        0        0     7848 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/anthropic_tracer.py
+-rw-r--r--   0        0        0     5094 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/cohere_tracer.py
+-rw-r--r--   0        0        0     5554 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/huggingface_tracer.py
+-rw-r--r--   0        0        0     5065 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/mistralai_tracer.py
+-rw-r--r--   0        0        0     5313 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/openai_tracer.py
+-rw-r--r--   0        0        0     1496 2024-05-02 11:48:09.116273 ecologits-0.1.4/ecologits/tracers/utils.py
+-rw-r--r--   0        0        0     3664 2024-05-02 11:48:09.116273 ecologits-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     4580 1970-01-01 00:00:00.000000 ecologits-0.1.4/PKG-INFO
```

### Comparing `ecologits-0.1.3/LICENSE` & `ecologits-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/README.md` & `ecologits-0.1.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 <p align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="./docs/assets/logo_dark.png">
-    <img alt="EcoLogits" src="./docs/assets/logo_light.png">
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/genai-impact/ecologits/main/docs/assets/logo_dark.png">
+    <img alt="EcoLogits" src="https://raw.githubusercontent.com/genai-impact/ecologits/main/docs/assets/logo_light.png">
   </picture>
 </p>
 
 🌱 **EcoLogits** tracks the energy consumption and environmental impacts of using generative AI models through APIs.
 
 [![PyPI version](https://img.shields.io/pypi/v/ecologits?color=00bf63)](https://pypi.org/project/ecologits/)
 [![Python version](https://img.shields.io/pypi/pyversions/ecologits)](https://pypi.org/project/ecologits/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VxrpJ5xuWZKQLsSN12kdqUqkppHRct3G?usp=sharing)
 
-Documentation: [ecologits.ai](https://ecologits.ai/)
+**Documentation: [ecologits.ai](https://ecologits.ai/)**
 
 
 ## ⚙️ Installation
 
 ```shell
 pip install ecologits
 ```
```

### Comparing `ecologits-0.1.3/ecologits/data/models.csv` & `ecologits-0.1.4/ecologits/data/models.csv`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/ecologits.py` & `ecologits-0.1.4/ecologits/ecologits.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/impacts/dag.py` & `ecologits-0.1.4/ecologits/impacts/dag.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/impacts/llm.py` & `ecologits-0.1.4/ecologits/impacts/llm.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 from math import ceil
 from typing import Optional
 
 from ecologits.impacts.dag import DAG
 from ecologits.impacts.models import GWP, PE, ADPe, Embodied, Energy, Impacts, Usage
 
 MODEL_QUANTIZATION_BITS = 4
@@ -132,15 +133,15 @@
         server_power: Power consumption of the server.
         server_gpu_count: Number of available GPUs in the server.
         gpu_required_count: Number of required GPUs to load the model.
 
     Returns:
         The energy consumption of the server (GPUs are not included).
     """
-    return generation_latency * server_power * (gpu_required_count / server_gpu_count)
+    return (generation_latency / 3600) * server_power * (gpu_required_count / server_gpu_count)
 
 
 @dag.asset
 def request_energy(
     datacenter_pue: float,
     server_energy: float,
     gpu_required_count: int,
@@ -418,14 +419,15 @@
         server_embodied_pe=server_embodied_pe,
         server_lifetime=server_lifetime,
         datacenter_pue=datacenter_pue,
         if_electricity_mix_gwp=if_electricity_mix_gwp,
         if_electricity_mix_adpe=if_electricity_mix_adpe,
         if_electricity_mix_pe=if_electricity_mix_pe
     )
+    print(json.dumps(results, indent=4))
     energy = Energy(value=results["request_energy"])
     gwp_usage = GWP(value=results["request_usage_gwp"])
     adpe_usage = ADPe(value=results["request_usage_adpe"])
     pe_usage = PE(value=results["request_usage_pe"])
     gwp_embodied = GWP(value=results["request_embodied_gwp"])
     adpe_embodied = ADPe(value=results["request_embodied_adpe"])
     pe_embodied = PE(value=results["request_embodied_pe"])
@@ -442,7 +444,18 @@
         ),
         embodied=Embodied(
             gwp=gwp_embodied,
             adpe=adpe_embodied,
             pe=pe_embodied
         )
     )
+
+
+if __name__ == '__main__':
+    impacts = compute_llm_impacts(
+        model_active_parameter_count=45,
+        model_total_parameter_count=45,
+        output_token_count=250,
+        request_latency=10000,
+    )
+    print('Energy:', impacts.energy.value)
+
```

### Comparing `ecologits-0.1.3/ecologits/impacts/models.py` & `ecologits-0.1.4/ecologits/impacts/models.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/model_repository.py` & `ecologits-0.1.4/ecologits/model_repository.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/tracers/anthropic_tracer.py` & `ecologits-0.1.4/ecologits/tracers/anthropic_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/tracers/cohere_tracer.py` & `ecologits-0.1.4/ecologits/tracers/cohere_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/tracers/huggingface_tracer.py` & `ecologits-0.1.4/ecologits/tracers/huggingface_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/tracers/mistralai_tracer.py` & `ecologits-0.1.4/ecologits/tracers/mistralai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/tracers/openai_tracer.py` & `ecologits-0.1.4/ecologits/tracers/openai_tracer.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/ecologits/tracers/utils.py` & `ecologits-0.1.4/ecologits/tracers/utils.py`

 * *Files identical despite different names*

### Comparing `ecologits-0.1.3/pyproject.toml` & `ecologits-0.1.4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "ecologits"
-version = "0.1.3"
+version = "0.1.4"
 description = "EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs."
 authors = [
     "GenAI Impact",
     "Data For Good"
 ]
 maintainers = [
     "GenAI Impact"
 ]
 license = "MPL-2.0"
 readme = "README.md"
+homepage = "https://ecologits.ai"
 repository = "https://github.com/genai-impact/ecologits"
+documentation = "https://ecologits.ai"
 classifiers = [
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Topic :: Internet",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Intended Audience :: Developers",
     "Intended Audience :: Information Technology",
```

### Comparing `ecologits-0.1.3/PKG-INFO` & `ecologits-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ecologits
-Version: 0.1.3
+Version: 0.1.4
 Summary: EcoLogits tracks and estimates the energy consumption and environmental impacts of using generative AI models through APIs.
-Home-page: https://github.com/genai-impact/ecologits
+Home-page: https://ecologits.ai
 License: MPL-2.0
 Author: GenAI Impact
 Maintainer: GenAI Impact
 Requires-Python: >=3.9,<4
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
@@ -38,31 +38,32 @@
 Requires-Dist: minijinja (>=1.0.16,<2.0.0) ; extra == "huggingface-hub"
 Requires-Dist: mistralai (>=0.1.3,<0.2.0) ; extra == "mistralai"
 Requires-Dist: openai (>=1.12.0,<2.0.0) ; extra == "openai"
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: tiktoken (>=0.6.0,<0.7.0) ; extra == "huggingface-hub"
 Requires-Dist: wrapt (>=1.14.1,<2.0.0)
+Project-URL: Documentation, https://ecologits.ai
 Project-URL: Repository, https://github.com/genai-impact/ecologits
 Description-Content-Type: text/markdown
 
 <p align="center">
   <picture>
-    <source media="(prefers-color-scheme: dark)" srcset="./docs/assets/logo_dark.png">
-    <img alt="EcoLogits" src="./docs/assets/logo_light.png">
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/genai-impact/ecologits/main/docs/assets/logo_dark.png">
+    <img alt="EcoLogits" src="https://raw.githubusercontent.com/genai-impact/ecologits/main/docs/assets/logo_light.png">
   </picture>
 </p>
 
 🌱 **EcoLogits** tracks the energy consumption and environmental impacts of using generative AI models through APIs.
 
 [![PyPI version](https://img.shields.io/pypi/v/ecologits?color=00bf63)](https://pypi.org/project/ecologits/)
 [![Python version](https://img.shields.io/pypi/pyversions/ecologits)](https://pypi.org/project/ecologits/)
 [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1VxrpJ5xuWZKQLsSN12kdqUqkppHRct3G?usp=sharing)
 
-Documentation: [ecologits.ai](https://ecologits.ai/)
+**Documentation: [ecologits.ai](https://ecologits.ai/)**
 
 
 ## ⚙️ Installation
 
 ```shell
 pip install ecologits
 ```
```

