# Comparing `tmp/gen_wrappers-0.1.0.tar.gz` & `tmp/gen_wrappers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.0.tar", last modified: Thu May  2 16:11:46 2024, max compression
+gzip compressed data, was "gen_wrappers-0.1.1.tar", last modified: Thu May  2 18:20:00 2024, max compression
```

## Comparing `gen_wrappers-0.1.0.tar` & `gen_wrappers-0.1.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.728048 gen_wrappers-0.1.0/
--rw-rw-rw-   0        0        0      823 2024-05-02 16:11:46.725263 gen_wrappers-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.665121 gen_wrappers-0.1.0/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.0/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.676878 gen_wrappers-0.1.0/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.0/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.0/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     2115 2024-05-02 16:04:46.000000 gen_wrappers-0.1.0/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.0/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.688287 gen_wrappers-0.1.0/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.0/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.0/creator/base/base_app.py
--rw-rw-rw-   0        0        0      111 2024-04-16 15:04:48.000000 gen_wrappers-0.1.0/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.0/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.0/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.698241 gen_wrappers-0.1.0/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.0/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.0/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2230 2024-05-02 15:57:38.000000 gen_wrappers-0.1.0/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.0/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.706399 gen_wrappers-0.1.0/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.0/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.0/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3496 2024-05-02 15:57:38.000000 gen_wrappers-0.1.0/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.0/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 16:11:46.722797 gen_wrappers-0.1.0/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-02 16:11:46.000000 gen_wrappers-0.1.0/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-02 16:11:46.000000 gen_wrappers-0.1.0/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 16:11:46.000000 gen_wrappers-0.1.0/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 16:11:46.000000 gen_wrappers-0.1.0/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 16:11:46.000000 gen_wrappers-0.1.0/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 16:11:46.728048 gen_wrappers-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1063 2024-05-02 16:11:16.000000 gen_wrappers-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.355773 gen_wrappers-0.1.1/
+-rw-rw-rw-   0        0        0      823 2024-05-02 18:20:00.352771 gen_wrappers-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.226155 gen_wrappers-0.1.1/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.1/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.244409 gen_wrappers-0.1.1/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.1/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     2193 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.265525 gen_wrappers-0.1.1/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.1/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      107 2024-05-02 17:56:22.000000 gen_wrappers-0.1.1/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.1/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.286063 gen_wrappers-0.1.1/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.1/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2796 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.307841 gen_wrappers-0.1.1/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.1/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.1/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3968 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.1/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 18:20:00.348135 gen_wrappers-0.1.1/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 18:20:00.000000 gen_wrappers-0.1.1/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 18:20:00.355773 gen_wrappers-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-02 18:19:46.000000 gen_wrappers-0.1.1/setup.py
```

### Comparing `gen_wrappers-0.1.0/PKG-INFO` & `gen_wrappers-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.0/creator/auto/creator_auto.py` & `gen_wrappers-0.1.1/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/creator/auto/request_auto.py` & `gen_wrappers-0.1.1/creator/auto/request_auto.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,49 @@
-from dataclasses import field, dataclass
 from typing import List, Dict, Any
 
+from pydantic import Field
+
 from creator.base.base_request import BaseRequest
 
 
-@dataclass
 class AutoTxt2Img(BaseRequest):
-    app = "AUTO"
-    prompt: str = ""
+    app: str = "AUTO"
+    prompt: str = Field("", examples=["A beautiful sunset over a mountain lake."])
     negative_prompt: str = ""
-    styles: List[str] = field(default_factory=list)
+    styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
-    subseed_strength: float = 0
+    subseed_strength: float = 0.0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
     sampler_name: str = "Euler a"
     batch_size: int = 1
     n_iter: int = 1
     steps: int = 20
-    cfg_scale: float = 7
+    cfg_scale: float = 7.0
     width: int = 1024
     height: int = 768
     restore_faces: bool = False
     tiling: bool = False
     do_not_save_samples: bool = True
     do_not_save_grid: bool = True
     eta: float = 0.0
     denoising_strength: float = 0.7
     s_min_uncond: float = 0.0
     s_churn: float = 0.0
     s_tmax: float = 0.0
     s_tmin: float = 0.0
     s_noise: float = 1.0
-    override_settings: Dict[str, Any] = field(default_factory=dict)
+    override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     override_settings_restore_afterwards: bool = True
-    refiner_checkpoint: str = ""  # Changed from None to ""
+    refiner_checkpoint: str = ""
     refiner_switch_at: int = 0
     disable_extra_networks: bool = False
-    firstpass_image: str = ""  # Changed from None to ""
-    comments: Dict[str, Any] = field(default_factory=dict)
+    firstpass_image: str = ""
+    comments: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     enable_hr: bool = False
     firstphase_width: int = 0
     firstphase_height: int = 0
     hr_scale: int = 2
     hr_upscaler: str = "Latent"
     hr_second_pass_steps: int = 0
     hr_resize_x: int = 0
@@ -51,17 +51,16 @@
     hr_checkpoint_name: str = ""
     hr_sampler_name: str = ""
     hr_prompt: str = ""
     hr_negative_prompt: str = ""
     force_task_id: str = ""
     sampler_index: str = "0"
     script_name: str = ""
-    script_args: List[Any] = field(default_factory=list)
+    script_args: List[Any] = Field(default_factory=list, examples=[[]])
     send_images: bool = True
     save_images: bool = False
-    alwayson_scripts: Dict[str, Any] = field(default_factory=dict)
+    alwayson_scripts: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     infotext: str = ""
 
 
-@dataclass
 class AutoModelLoad(BaseRequest):
-    sd_model_checkpoint: str = "sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"
+    sd_model_checkpoint: str = Field("", examples=["sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"])
```

### Comparing `gen_wrappers-0.1.0/creator/auto/response_auto.py` & `gen_wrappers-0.1.1/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/creator/base/base_app.py` & `gen_wrappers-0.1.1/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/creator/base/base_response.py` & `gen_wrappers-0.1.1/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.1.1/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.1.1/creator/cmfy/request_cmfy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,118 +1,119 @@
 import json
 from dataclasses import dataclass
 
+from pydantic import Field
+
 from creator.base.base_request import BaseRequest
 
 default_workflow_json = {
-  "3": {
-    "inputs": {
-      "seed": 985289875893903,
-      "steps": 20,
-      "cfg": 7.5,
-      "sampler_name": "uni_pc",
-      "scheduler": "karras",
-      "denoise": 1,
-      "model": [
-        "4",
-        0
-      ],
-      "positive": [
-        "6",
-        0
-      ],
-      "negative": [
-        "7",
-        0
-      ],
-      "latent_image": [
-        "5",
-        0
-      ]
-    },
-    "class_type": "KSampler",
-    "_meta": {
-      "title": "KSampler"
-    }
-  },
-  "4": {
-    "inputs": {
-      "ckpt_name": "sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"
-    },
-    "class_type": "CheckpointLoaderSimple",
-    "_meta": {
-      "title": "Load Checkpoint"
-    }
-  },
-  "5": {
-    "inputs": {
-      "width": 1024,
-      "height": 768,
-      "batch_size": 1
-    },
-    "class_type": "EmptyLatentImage",
-    "_meta": {
-      "title": "Empty Latent Image"
-    }
-  },
-  "6": {
-    "inputs": {
-      "text": "a photograph of a smiling green alien holding a sign which says \"Run Diffusion\", ultra realistic, street, city, sci-fi, ultra realistic, cute, friendly",
-      "clip": [
-        "4",
-        1
-      ]
-    },
-    "class_type": "CLIPTextEncode",
-    "_meta": {
-      "title": "CLIP Text Encode (Prompt)"
-    }
-  },
-  "7": {
-    "inputs": {
-      "text": "blurry, low quality",
-      "clip": [
-        "4",
-        1
-      ]
-    },
-    "class_type": "CLIPTextEncode",
-    "_meta": {
-      "title": "CLIP Text Encode (Prompt)"
-    }
-  },
-  "8": {
-    "inputs": {
-      "samples": [
-        "3",
-        0
-      ],
-      "vae": [
-        "4",
-        2
-      ]
-    },
-    "class_type": "VAEDecode",
-    "_meta": {
-      "title": "VAE Decode"
-    }
-  },
-  "9": {
-    "inputs": {
-      "filename_prefix": "ComfyUI",
-      "images": [
-        "8",
-        0
-      ]
-    },
-    "class_type": "SaveImage",
-    "_meta": {
-      "title": "Save Image"
+    "3": {
+        "inputs": {
+            "seed": 985289875893903,
+            "steps": 20,
+            "cfg": 7.5,
+            "sampler_name": "uni_pc",
+            "scheduler": "karras",
+            "denoise": 1,
+            "model": [
+                "4",
+                0
+            ],
+            "positive": [
+                "6",
+                0
+            ],
+            "negative": [
+                "7",
+                0
+            ],
+            "latent_image": [
+                "5",
+                0
+            ]
+        },
+        "class_type": "KSampler",
+        "_meta": {
+            "title": "KSampler"
+        }
+    },
+    "4": {
+        "inputs": {
+            "ckpt_name": "sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"
+        },
+        "class_type": "CheckpointLoaderSimple",
+        "_meta": {
+            "title": "Load Checkpoint"
+        }
+    },
+    "5": {
+        "inputs": {
+            "width": 1024,
+            "height": 768,
+            "batch_size": 1
+        },
+        "class_type": "EmptyLatentImage",
+        "_meta": {
+            "title": "Empty Latent Image"
+        }
+    },
+    "6": {
+        "inputs": {
+            "text": "a photograph of a smiling green alien holding a sign which says \"Run Diffusion\", ultra realistic, street, city, sci-fi, ultra realistic, cute, friendly",
+            "clip": [
+                "4",
+                1
+            ]
+        },
+        "class_type": "CLIPTextEncode",
+        "_meta": {
+            "title": "CLIP Text Encode (Prompt)"
+        }
+    },
+    "7": {
+        "inputs": {
+            "text": "blurry, low quality",
+            "clip": [
+                "4",
+                1
+            ]
+        },
+        "class_type": "CLIPTextEncode",
+        "_meta": {
+            "title": "CLIP Text Encode (Prompt)"
+        }
+    },
+    "8": {
+        "inputs": {
+            "samples": [
+                "3",
+                0
+            ],
+            "vae": [
+                "4",
+                2
+            ]
+        },
+        "class_type": "VAEDecode",
+        "_meta": {
+            "title": "VAE Decode"
+        }
+    },
+    "9": {
+        "inputs": {
+            "filename_prefix": "ComfyUI",
+            "images": [
+                "8",
+                0
+            ]
+        },
+        "class_type": "SaveImage",
+        "_meta": {
+            "title": "Save Image"
+        }
     }
-  }
 }
 
 
-@dataclass
 class CmfyTxt2Img(BaseRequest):
-    app = "CMFY"
-    workflow_json: str = json.dumps(default_workflow_json)
+    app: str = "CMFY"
+    workflow_json: str = Field("", examples=[json.dumps({})])
```

### Comparing `gen_wrappers-0.1.0/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.1.1/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.1.1/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.1.1/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.0
+Version: 0.1.1
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.0/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.1.1/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.0/setup.py` & `gen_wrappers-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import httpx
-import pydantic
-import requests
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.0',
+    version='0.1.1',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

