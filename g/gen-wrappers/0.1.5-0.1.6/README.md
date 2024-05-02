# Comparing `tmp/gen_wrappers-0.1.5.tar.gz` & `tmp/gen_wrappers-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen_wrappers-0.1.5.tar", last modified: Thu May  2 20:42:52 2024, max compression
+gzip compressed data, was "gen_wrappers-0.1.6.tar", last modified: Thu May  2 20:53:40 2024, max compression
```

## Comparing `gen_wrappers-0.1.5.tar` & `gen_wrappers-0.1.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.740583 gen_wrappers-0.1.5/
--rw-rw-rw-   0        0        0      823 2024-05-02 20:42:52.738580 gen_wrappers-0.1.5/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.700343 gen_wrappers-0.1.5/creator/
--rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.5/creator/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.705537 gen_wrappers-0.1.5/creator/auto/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.5/creator/auto/__init__.py
--rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.1.5/creator/auto/creator_auto.py
--rw-rw-rw-   0        0        0     4238 2024-05-02 20:41:19.000000 gen_wrappers-0.1.5/creator/auto/request_auto.py
--rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/auto/response_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.712355 gen_wrappers-0.1.5/creator/base/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.5/creator/base/__init__.py
--rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/base/base_app.py
--rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.5/creator/base/base_request.py
--rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.5/creator/base/base_response.py
--rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.5/creator/base/job_status.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.716870 gen_wrappers-0.1.5/creator/cmfy/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.5/creator/cmfy/__init__.py
--rw-rw-rw-   0        0        0     9969 2024-05-02 16:04:46.000000 gen_wrappers-0.1.5/creator/cmfy/creator_cmfy.py
--rw-rw-rw-   0        0        0     2773 2024-05-02 20:32:31.000000 gen_wrappers-0.1.5/creator/cmfy/request_cmfy.py
--rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/cmfy/response_cmfy.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.720870 gen_wrappers-0.1.5/creator/fcus_api/
--rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.5/creator/fcus_api/__init__.py
--rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.5/creator/fcus_api/creator_fcus_api.py
--rw-rw-rw-   0        0        0     3911 2024-05-02 20:32:31.000000 gen_wrappers-0.1.5/creator/fcus_api/request_fcus_api.py
--rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.5/creator/fcus_api/response_fcus_api.py
-drwxrwxrwx   0        0        0        0 2024-05-02 20:42:52.737582 gen_wrappers-0.1.5/gen_wrappers.egg-info/
--rw-rw-rw-   0        0        0      823 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      710 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-02 20:42:52.000000 gen_wrappers-0.1.5/gen_wrappers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-02 20:42:52.740583 gen_wrappers-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1015 2024-05-02 20:42:49.000000 gen_wrappers-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.356430 gen_wrappers-0.1.6/
+-rw-rw-rw-   0        0        0      823 2024-05-02 20:53:40.353605 gen_wrappers-0.1.6/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.278603 gen_wrappers-0.1.6/creator/
+-rw-rw-rw-   0        0        0        0 2024-04-09 16:36:19.000000 gen_wrappers-0.1.6/creator/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.286041 gen_wrappers-0.1.6/creator/auto/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:51.000000 gen_wrappers-0.1.6/creator/auto/__init__.py
+-rw-rw-rw-   0        0        0     5883 2024-05-02 20:42:34.000000 gen_wrappers-0.1.6/creator/auto/creator_auto.py
+-rw-rw-rw-   0        0        0     4184 2024-05-02 20:52:05.000000 gen_wrappers-0.1.6/creator/auto/request_auto.py
+-rw-rw-rw-   0        0        0      609 2024-05-02 15:57:38.000000 gen_wrappers-0.1.6/creator/auto/response_auto.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.297026 gen_wrappers-0.1.6/creator/base/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:25:44.000000 gen_wrappers-0.1.6/creator/base/__init__.py
+-rw-rw-rw-   0        0        0     1253 2024-05-02 15:57:38.000000 gen_wrappers-0.1.6/creator/base/base_app.py
+-rw-rw-rw-   0        0        0      554 2024-05-02 19:51:12.000000 gen_wrappers-0.1.6/creator/base/base_request.py
+-rw-rw-rw-   0        0        0     1569 2024-05-02 16:04:46.000000 gen_wrappers-0.1.6/creator/base/base_response.py
+-rw-rw-rw-   0        0        0      228 2024-04-26 19:27:33.000000 gen_wrappers-0.1.6/creator/base/job_status.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.306680 gen_wrappers-0.1.6/creator/cmfy/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:43.000000 gen_wrappers-0.1.6/creator/cmfy/__init__.py
+-rw-rw-rw-   0        0        0     9974 2024-05-02 20:53:05.000000 gen_wrappers-0.1.6/creator/cmfy/creator_cmfy.py
+-rw-rw-rw-   0        0        0     2793 2024-05-02 20:53:05.000000 gen_wrappers-0.1.6/creator/cmfy/request_cmfy.py
+-rw-rw-rw-   0        0        0      503 2024-05-02 15:57:38.000000 gen_wrappers-0.1.6/creator/cmfy/response_cmfy.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.315765 gen_wrappers-0.1.6/creator/fcus_api/
+-rw-rw-rw-   0        0        0        0 2024-04-09 20:26:36.000000 gen_wrappers-0.1.6/creator/fcus_api/__init__.py
+-rw-rw-rw-   0        0        0     6340 2024-05-02 16:04:46.000000 gen_wrappers-0.1.6/creator/fcus_api/creator_fcus_api.py
+-rw-rw-rw-   0        0        0     3911 2024-05-02 20:32:31.000000 gen_wrappers-0.1.6/creator/fcus_api/request_fcus_api.py
+-rw-rw-rw-   0        0        0     1131 2024-05-02 15:57:38.000000 gen_wrappers-0.1.6/creator/fcus_api/response_fcus_api.py
+drwxrwxrwx   0        0        0        0 2024-05-02 20:53:40.350598 gen_wrappers-0.1.6/gen_wrappers.egg-info/
+-rw-rw-rw-   0        0        0      823 2024-05-02 20:53:40.000000 gen_wrappers-0.1.6/gen_wrappers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      710 2024-05-02 20:53:40.000000 gen_wrappers-0.1.6/gen_wrappers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-02 20:53:40.000000 gen_wrappers-0.1.6/gen_wrappers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-02 20:53:40.000000 gen_wrappers-0.1.6/gen_wrappers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-02 20:53:40.000000 gen_wrappers-0.1.6/gen_wrappers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-02 20:53:40.356430 gen_wrappers-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1015 2024-05-02 20:53:37.000000 gen_wrappers-0.1.6/setup.py
```

### Comparing `gen_wrappers-0.1.5/PKG-INFO` & `gen_wrappers-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen_wrappers
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.5/creator/auto/creator_auto.py` & `gen_wrappers-0.1.6/creator/auto/creator_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/auto/request_auto.py` & `gen_wrappers-0.1.6/creator/auto/request_auto.py`

 * *Files 14% similar despite different names*

```diff
@@ -66,16 +66,16 @@
     negative_prompt: str = ""
     styles: List[str] = Field(default_factory=list, examples=[[]])
     seed: int = -1
     subseed: int = -1
     subseed_strength: float = 0.0
     seed_resize_from_h: int = -1
     seed_resize_from_w: int = -1
-    sampler_name: str = "string"
-    scheduler: str = "string"
+    sampler_name: str = ""
+    scheduler: str = ""
     batch_size: int = 1
     n_iter: int = 1
     steps: int = 50
     cfg_scale: float = 7.0
     width: int = 512
     height: int = 512
     restore_faces: bool = True
@@ -87,39 +87,39 @@
     s_min_uncond: float = 0.0
     s_churn: float = 0.0
     s_tmax: float = 0.0
     s_tmin: float = 0.0
     s_noise: float = 0.0
     override_settings: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     override_settings_restore_afterwards: bool = True
-    refiner_checkpoint: str = "string"
+    refiner_checkpoint: str = ""
     refiner_switch_at: int = 0
     disable_extra_networks: bool = False
-    firstpass_image: str = "string"
+    firstpass_image: str = ""
     comments: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
     init_images: List[str] = Field(default_factory=list, examples=[[]])
     resize_mode: int = 0
     image_cfg_scale: float = 0.0
-    mask: str = "string"
+    mask: str = ""
     mask_blur_x: int = 4
     mask_blur_y: int = 4
     mask_blur: int = 0
     mask_round: bool = True
     inpainting_fill: int = 0
     inpaint_full_res: bool = True
     inpaint_full_res_padding: int = 0
     inpainting_mask_invert: int = 0
     initial_noise_multiplier: float = 0.0
-    latent_mask: str = "string"
-    force_task_id: str = "string"
+    latent_mask: str = ""
+    force_task_id: str = ""
     sampler_index: str = "Euler"
     include_init_images: bool = False
-    script_name: str = "string"
+    script_name: str = ""
     script_args: List[Any] = Field(default_factory=list, examples=[[]])
     send_images: bool = True
     save_images: bool = False
     alwayson_scripts: Dict[str, Any] = Field(default_factory=dict, examples=[{}])
-    infotext: str = "string"
+    infotext: str = ""
 
 
 class AutoModelLoad(BaseRequest):
     sd_model_checkpoint: str = Field("", examples=["sdxl/juggernautXL_v9Rundiffusionphoto2.safetensors"])
```

### Comparing `gen_wrappers-0.1.5/creator/auto/response_auto.py` & `gen_wrappers-0.1.6/creator/auto/response_auto.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/base/base_app.py` & `gen_wrappers-0.1.6/creator/base/base_app.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/base/base_request.py` & `gen_wrappers-0.1.6/creator/base/base_request.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/base/base_response.py` & `gen_wrappers-0.1.6/creator/base/base_response.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/cmfy/creator_cmfy.py` & `gen_wrappers-0.1.6/creator/cmfy/creator_cmfy.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import httpx
 import requests
 
 from creator.base.base_app import BaseApp
 from creator.base.base_request import BaseRequest
 from creator.base.base_response import ResponseDataType, ResponseData, BaseResponse
 from creator.base.job_status import JobStatus
-from creator.cmfy.request_cmfy import CmfyTxt2Img
+from creator.cmfy.request_cmfy import CmfyWorkflow
 from creator.cmfy.response_cmfy import ResponseCmfy
 
 logger = logging.getLogger(__name__)
 
 
 @dataclasses.dataclass
 class NodeInput:
@@ -30,38 +30,38 @@
 
 @dataclasses.dataclass
 class CmfyWorkflow:
     prompt: str
     nodes: Dict[str, NodeInput]
 
     @staticmethod
-    def from_json(params: CmfyTxt2Img) -> str:
+    def from_json(params: CmfyWorkflow) -> str:
         json_str = params.workflow_json
         return json_str
 
     def to_json(self) -> str:
         dump = {}
         for node_id, node in self.nodes.items():
             dump[node_id] = dataclasses.asdict(node)
 
         return json.dumps({"prompt": dump})
 
 
 class AppCmfy(BaseApp):
-    param_classes = [CmfyTxt2Img]
+    param_classes = [CmfyWorkflow]
     output = {}
 
     def __init__(self):
         super().__init__()
         focus_port = os.environ.get("PORT_CMFY", 8888)
         if isinstance(focus_port, str):
             focus_port = int(focus_port)
         self.api_base_url = f"http://0.0.0.0:{focus_port}"
 
-    async def create(self, params: CmfyTxt2Img) -> ResponseCmfy:
+    async def create(self, params: CmfyWorkflow) -> ResponseCmfy:
         cmfy_port = os.environ.get("PORT_CMFY", 8889)
         url = f"http://localhost:{cmfy_port}/prompt"
         workflow = json.loads(params.workflow_json)
         self._check_loaded_model(workflow)
         logger.debug(f"CMFY data: {workflow}")
         # Send a POST to cmfy_url with the workflow json
         # The response will be JSON string with the below format
@@ -97,15 +97,15 @@
                 data_type=ResponseDataType.IMAGE,
                 total_count=len(data)
             )
             logger.info(f"Success, returning response with {len(data)} images")
             return ResponseCmfy.success(response_data)
         return ResponseCmfy.error("Error creating prompt")
 
-    async def create_async(self, params: CmfyTxt2Img) -> ResponseCmfy:
+    async def create_async(self, params: CmfyWorkflow) -> ResponseCmfy:
         cmfy_port = os.environ.get("PORT_CMFY", 8889)
         url = f"http://localhost:{cmfy_port}/prompt"
         workflow = json.loads(params.workflow_json)
         self._check_loaded_model(workflow)
         logger.debug(f"CMFY data: {workflow}")
         # Send a POST to cmfy_url with the workflow json
         # The response will be JSON string with the below format
```

### Comparing `gen_wrappers-0.1.5/creator/cmfy/request_cmfy.py` & `gen_wrappers-0.1.6/creator/cmfy/request_cmfy.py`

 * *Files 6% similar despite different names*

```diff
@@ -110,9 +110,9 @@
         "_meta": {
             "title": "Save Image"
         }
     }
 }
 
 
-class CmfyTxt2Img(BaseRequest):
-    workflow_json: str = Field("", examples=[json.dumps({})])
+class CmfyWorkflow(BaseRequest):
+    workflow_json: str = Field("", examples=[json.dumps(default_workflow_json)])
```

### Comparing `gen_wrappers-0.1.5/creator/fcus_api/creator_fcus_api.py` & `gen_wrappers-0.1.6/creator/fcus_api/creator_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/fcus_api/request_fcus_api.py` & `gen_wrappers-0.1.6/creator/fcus_api/request_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/creator/fcus_api/response_fcus_api.py` & `gen_wrappers-0.1.6/creator/fcus_api/response_fcus_api.py`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/gen_wrappers.egg-info/PKG-INFO` & `gen_wrappers-0.1.6/gen_wrappers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-wrappers
-Version: 0.1.5
+Version: 0.1.6
 Summary: A set of wrapper classes for various generative API projects
 Home-page: https://github.com/d8ahazard/gen_wrappers
 Author: d8ahazard
 Author-email: d8ahazard@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `gen_wrappers-0.1.5/gen_wrappers.egg-info/SOURCES.txt` & `gen_wrappers-0.1.6/gen_wrappers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gen_wrappers-0.1.5/setup.py` & `gen_wrappers-0.1.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gen_wrappers',
-    version='0.1.5',
+    version='0.1.6',
     author='d8ahazard',
     author_email='d8ahazard@gmail.com',
     description='A set of wrapper classes for various generative API projects',
     long_description_content_type='text/markdown',
     url='https://github.com/d8ahazard/gen_wrappers',  # Change this to your repository URL
     packages=find_packages(),
     install_requires=[
```

