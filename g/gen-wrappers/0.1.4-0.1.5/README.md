# Comparing `tmp/gen_wrappers-0.1.4.tar.gz` & `tmp/gen_wrappers-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.4.tar", last modified: Thu May  2 20:03:26 2024, max compression
+gzip compressed data, was "gen_wrappers-0.1.5.tar", last modified: Thu May  2 20:42:52 2024, max compression
```

## Comparing `gen_wrappers-0.1.4.tar` & `gen_wrappers-0.1.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.311063 gen_wrappers-0.1.4/
--rw-rw-rw-   0        0        0      823 2024-05-02 20:03:26.311063 gen_wrappers-0.1.4/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.281088 gen_wrappers-0.1.4/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.4/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.286154 gen_wrappers-0.1.4/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.4/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5719 2024-05-02 16:04:46.000000 gen_wrappers-0.1.4/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     2193 2024-05-02 18:19:46.000000 gen_wrappers-0.1.4/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.4/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.291630 gen_wrappers-0.1.4/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.4/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.4/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.4/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.4/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.4/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.296721 gen_wrappers-0.1.4/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.4/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.4/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2796 2024-05-02 18:19:46.000000 gen_wrappers-0.1.4/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.4/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.300723 gen_wrappers-0.1.4/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.4/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.4/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3980 2024-05-02 20:02:31.000000 gen_wrappers-0.1.4/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.4/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:03:26.310062 gen_wrappers-0.1.4/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-02 20:03:26.000000 gen_wrappers-0.1.4/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-02 20:03:26.000000 gen_wrappers-0.1.4/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:03:26.000000 gen_wrappers-0.1.4/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 20:03:26.000000 gen_wrappers-0.1.4/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 20:03:26.000000 gen_wrappers-0.1.4/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:03:26.312567 gen_wrappers-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-02 20:03:09.000000 gen_wrappers-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.740583 gen_wrappers-0.1.5/
+-rw-rw-rw-   0        0        0      823 2024-05-02 20:42:52.738580 gen_wrappers-0.1.5/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.700343 gen_wrappers-0.1.5/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.5/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.705537 gen_wrappers-0.1.5/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.5/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.1.5/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4238 2024-05-02 20:41:19.000000 gen_wrappers-0.1.5/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.712355 gen_wrappers-0.1.5/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.5/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.5/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.5/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.5/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.716870 gen_wrappers-0.1.5/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.5/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.5/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2773 2024-05-02 20:32:31.000000 gen_wrappers-0.1.5/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.720870 gen_wrappers-0.1.5/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.5/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.5/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3911 2024-05-02 20:32:31.000000 gen_wrappers-0.1.5/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.737582 gen_wrappers-0.1.5/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:42:52.740583 gen_wrappers-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-02 20:42:49.000000 gen_wrappers-0.1.5/setup.py
```

### Comparing `gen_wrappers-0.1.4/PKG-INFO` & `gen_wrappers-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.4/creator/auto/creator_auto.py` & `gen_wrappers-0.1.5/creator/auto/creator_auto.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import asyncio
 import logging
 import os
 import random
 import traceback
-from typing import Any, List
+from typing import Any, List, Union
 
 import httpx
 
-from creator.auto.request_auto import AutoTxt2Img, AutoModelLoad
+from creator.auto.request_auto import AutoTxt2Img, AutoModelLoad, AutoImg2Img
 from creator.auto.response_auto import ResponseAuto
 from creator.base.base_app import BaseApp
 from creator.base.base_response import BaseResponse
 
 logger = logging.getLogger(__name__)
 
 
 class AppAuto(BaseApp):
-    param_classes = [AutoTxt2Img]
+    param_classes = [AutoTxt2Img, AutoImg2Img]
     output = {}
     jobs = {}
 
     def __init__(self):
         super().__init__()
         auto_port = os.environ.get("PORT_AUTO", 8081)
         if isinstance(auto_port, str):
             auto_port = int(auto_port)
         self.jobs = {}
         self.output = {}
         self.api_base_url = f"http://0.0.0.0:{auto_port}/sdapi"
 
-    async def create(self, params: AutoTxt2Img, job_id=None) -> BaseResponse:
+    async def create(self, params: Union[AutoTxt2Img, AutoImg2Img], job_id=None) -> BaseResponse:
         print(f"Creating job with params: {params}")
-
-        url = f"{self.api_base_url}/sdapi/v1/txt2img"
+        endpoint_name = "txt2img" if isinstance(params, AutoTxt2Img) else "img2img"
+        url = f"{self.api_base_url}/sdapi/v1/{endpoint_name}"
         data = params.__dict__
         headers = {'Content-Type': 'application/json'}
         async with httpx.AsyncClient() as client:
             response = await client.post(url, data=data, headers=headers)
             response.raise_for_status()
         output = response.json()
         print(f"Response received: {output}")
         if job_id:
             self.output[job_id] = output
         return ResponseAuto.parse_response(output)
 
-    async def create_async(self, params: AutoTxt2Img) -> BaseResponse:
+    async def create_async(self, params: Union[AutoTxt2Img, AutoImg2Img]) -> BaseResponse:
         job_id = str(random.randint(0, 100000))
         print(f"Creating job with ID {job_id}")
 
         # Store the job_id immediately with a placeholder to indicate it's pending
         self.output[job_id] = {"status": "pending"}
 
         # Fire off the job without waiting for it to complete
```

### Comparing `gen_wrappers-0.1.4/creator/auto/request_auto.py` & `gen_wrappers-0.1.5/creator/auto/request_auto.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from pydantic import Field
 
 from creator.base.base_request import BaseRequest
 
 
 class AutoTxt2Img(BaseRequest):
-    app: str = "AUTO"
     prompt: str = Field("", examples=["A beautiful sunset over a mountain lake."])
     negative_prompt: str = ""
     styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
     subseed_strength: float = 0.0
     seed_resize_from_h: int = -1
@@ -58,9 +57,69 @@
     script_args: List[Any] = Field(default_factory=list, examples=[[]])
     send_images: bool = True
     save_images: bool = False
     alwayson_scripts: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     infotext: str = ""
 
 
+class AutoImg2Img(BaseRequest):
+    prompt: str = ""
+    negative_prompt: str = ""
+    styles: List[str] = Field(default_factory=list, examples=[[]])
+    seed: int = -1
+    subseed: int = -1
+    subseed_strength: float = 0.0
+    seed_resize_from_h: int = -1
+    seed_resize_from_w: int = -1
+    sampler_name: str = "string"
+    scheduler: str = "string"
+    batch_size: int = 1
+    n_iter: int = 1
+    steps: int = 50
+    cfg_scale: float = 7.0
+    width: int = 512
+    height: int = 512
+    restore_faces: bool = True
+    tiling: bool = True
+    do_not_save_samples: bool = False
+    do_not_save_grid: bool = False
+    eta: float = 0.0
+    denoising_strength: float = 0.75
+    s_min_uncond: float = 0.0
+    s_churn: float = 0.0
+    s_tmax: float = 0.0
+    s_tmin: float = 0.0
+    s_noise: float = 0.0
+    override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
+    override_settings_restore_afterwards: bool = True
+    refiner_checkpoint: str = "string"
+    refiner_switch_at: int = 0
+    disable_extra_networks: bool = False
+    firstpass_image: str = "string"
+    comments: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
+    init_images: List[str] = Field(default_factory=list, examples=[[]])
+    resize_mode: int = 0
+    image_cfg_scale: float = 0.0
+    mask: str = "string"
+    mask_blur_x: int = 4
+    mask_blur_y: int = 4
+    mask_blur: int = 0
+    mask_round: bool = True
+    inpainting_fill: int = 0
+    inpaint_full_res: bool = True
+    inpaint_full_res_padding: int = 0
+    inpainting_mask_invert: int = 0
+    initial_noise_multiplier: float = 0.0
+    latent_mask: str = "string"
+    force_task_id: str = "string"
+    sampler_index: str = "Euler"
+    include_init_images: bool = False
+    script_name: str = "string"
+    script_args: List[Any] = Field(default_factory=list, examples=[[]])
+    send_images: bool = True
+    save_images: bool = False
+    alwayson_scripts: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
+    infotext: str = "string"
+
+
 class AutoModelLoad(BaseRequest):
     sd_model_checkpoint: str = Field("", examples=["sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"])
```

### Comparing `gen_wrappers-0.1.4/creator/auto/response_auto.py` & `gen_wrappers-0.1.5/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/creator/base/base_app.py` & `gen_wrappers-0.1.5/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/creator/base/base_request.py` & `gen_wrappers-0.1.5/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/creator/base/base_response.py` & `gen_wrappers-0.1.5/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.1.5/creator/cmfy/creator_cmfy.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.1.5/creator/cmfy/request_cmfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -111,9 +111,8 @@
             "title": "Save Image"
         }
     }
 }
 
 
 class CmfyTxt2Img(BaseRequest):
-    app: str = "CMFY"
     workflow_json: str = Field("", examples=[json.dumps({})])
```

### Comparing `gen_wrappers-0.1.4/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.1.5/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.1.5/creator/fcus_api/request_fcus_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 
 class Lora(BaseModel):
     model_name: str = Field("", examples=["sd_xl_offset_example-lora_1.0.safetensors"])
     weight: float = 1.0
 
 
 class FcusTxt2Img(BaseRequest):
-    app: str = "FCUS"
     prompt: str = ""
     negative_prompt: str = ""
     style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = "Speed"
     aspect_ratios_selection: str = "1152*896"
     image_number: int = 2
     image_seed: int = -1
@@ -57,15 +56,14 @@
     loras: List[Lora] = Field(default_factory=list, examples=[[Lora()]])
     advanced_params: Optional[FcusAdvancedParams] = Field(default=None, examples=[FcusAdvancedParams()])
     require_base64: bool = True
     async_process: bool = True
 
 
 class FcusUpscaleOrVary(BaseRequest):
-    app: str = "FCUS"
     input_image: str = ""
     uov_method: str = ""
     prompt: str = ""
     negative_prompt: str = ""
     style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
     performance_selection: str = ""
     aspect_ratios_selection: str = ""
@@ -79,15 +77,14 @@
     loras: List[Lora] = Field(default_factory=list, examples=[[Lora()]])
     advanced_params: Optional[FcusAdvancedParams] = Field(default=None, examples=[FcusAdvancedParams()])
     require_base64: bool = False
     async_process: bool = True
 
 
 class FcusInpaintOrOutpaint(BaseRequest):
-    app: str = "FCUS"
     request_params: str = ""
     input_image: str = ""
     input_mask: str = ""
     outpaint_selections: List[str] = Field(default_factory=list, examples=[])
     prompt: str = ""
     negative_prompt: str = ""
     style_selections: List[str] = Field(default_factory=list, examples=[["Fooocus V2", "Fooocus Enhance", "Fooocus Sharp"]])
```

### Comparing `gen_wrappers-0.1.4/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.1.5/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.1.5/gen_wrappers.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.4
+Version: 0.1.5
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.4/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.1.5/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.4/setup.py` & `gen_wrappers-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.4',
+    version='0.1.5',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

