# Comparing `tmp/liulianmao-1.3.0.tar.gz` & `tmp/liulianmao-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liulianmao-1.3.0.tar", max compression
+gzip compressed data, was "liulianmao-1.4.0.tar", max compression
```

## Comparing `liulianmao-1.3.0.tar` & `liulianmao-1.4.0.tar`

### file list

```diff
@@ -1,25 +1,23 @@
--rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.3.0/LICENSE
--rw-r--r--   0        0        0      781 2024-05-01 15:26:09.878471 liulianmao-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     7095 2024-05-01 14:58:58.387675 liulianmao-1.3.0/README.md
--rw-r--r--   0        0        0       84 2024-04-03 13:08:57.859474 liulianmao-1.3.0/src/liulianmao/__init__.py
--rw-r--r--   0        0        0     5020 2024-05-01 15:13:48.542866 liulianmao-1.3.0/src/liulianmao/__main__.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:28.446436 liulianmao-1.3.0/src/liulianmao/client/__init__.py
--rw-r--r--   0        0        0      171 2024-04-05 06:18:07.214401 liulianmao-1.3.0/src/liulianmao/client/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    20033 2024-05-01 15:22:42.210544 liulianmao-1.3.0/src/liulianmao/client/__pycache__/core.cpython-311.pyc
--rw-r--r--   0        0        0    13563 2024-05-01 15:22:08.167782 liulianmao-1.3.0/src/liulianmao/client/core.py
--rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.3.0/src/liulianmao/client/langchain.py
--rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-1.3.0/src/liulianmao/module/__init__.py
--rw-r--r--   0        0        0      318 2024-04-14 08:28:05.811497 liulianmao-1.3.0/src/liulianmao/module/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4697 2024-04-14 08:28:05.814494 liulianmao-1.3.0/src/liulianmao/module/__pycache__/authentication.cpython-311.pyc
--rw-r--r--   0        0        0      931 2024-04-05 06:18:07.722094 liulianmao-1.3.0/src/liulianmao/module/__pycache__/const.cpython-311.pyc
--rw-r--r--   0        0        0     1056 2024-04-05 06:18:07.342514 liulianmao-1.3.0/src/liulianmao/module/__pycache__/log.cpython-311.pyc
--rw-r--r--   0        0        0     2497 2024-04-14 10:19:38.564221 liulianmao-1.3.0/src/liulianmao/module/__pycache__/model.cpython-311.pyc
--rw-r--r--   0        0        0     2481 2024-05-01 14:56:53.609585 liulianmao-1.3.0/src/liulianmao/module/__pycache__/storage.cpython-311.pyc
--rw-r--r--   0        0        0     2864 2024-04-14 08:22:48.515590 liulianmao-1.3.0/src/liulianmao/module/authentication.py
--rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.3.0/src/liulianmao/module/const.py
--rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.3.0/src/liulianmao/module/log.py
--rw-r--r--   0        0        0     2347 2024-04-14 09:58:34.104170 liulianmao-1.3.0/src/liulianmao/module/model.py
--rw-r--r--   0        0        0     1647 2024-05-01 14:53:06.868641 liulianmao-1.3.0/src/liulianmao/module/storage.py
--rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.3.0/src/liulianmao/tool/__init__.py
--rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.3.0/src/liulianmao/tool/ls.py
--rw-r--r--   0        0        0     7995 1970-01-01 00:00:00.000000 liulianmao-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-20 13:24:32.980497 liulianmao-1.4.0/LICENSE
+-rw-r--r--   0        0        0      781 2024-05-02 16:41:01.767151 liulianmao-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6686 2024-05-02 16:18:09.075783 liulianmao-1.4.0/README.md
+-rw-r--r--   0        0        0       46 2024-05-02 16:46:19.722762 liulianmao-1.4.0/src/liulianmao/__init__.py
+-rw-r--r--   0        0        0     5361 2024-05-02 16:37:51.958253 liulianmao-1.4.0/src/liulianmao/__main__.py
+-rw-r--r--   0        0        0       20 2024-05-02 10:57:42.700258 liulianmao-1.4.0/src/liulianmao/client/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-01 15:35:10.006780 liulianmao-1.4.0/src/liulianmao/client/api/__init__.py
+-rw-r--r--   0        0        0      737 2024-05-02 15:54:50.285280 liulianmao-1.4.0/src/liulianmao/client/api/llama.py
+-rw-r--r--   0        0        0    12236 2024-05-02 16:45:45.299436 liulianmao-1.4.0/src/liulianmao/client/api/openai.py
+-rw-r--r--   0        0        0     1219 2024-05-02 16:07:58.953960 liulianmao-1.4.0/src/liulianmao/client/api/README.md
+-rw-r--r--   0        0        0     9737 2024-05-02 16:34:36.458629 liulianmao-1.4.0/src/liulianmao/client/core.py
+-rw-r--r--   0        0        0      608 2024-04-05 06:17:08.745870 liulianmao-1.4.0/src/liulianmao/client/langchain.py
+-rw-r--r--   0        0        0      543 2024-05-02 15:48:15.958476 liulianmao-1.4.0/src/liulianmao/client/utils/config.py
+-rw-r--r--   0        0        0       29 2024-05-02 16:41:00.037192 liulianmao-1.4.0/src/liulianmao/const.py
+-rw-r--r--   0        0        0      119 2024-04-14 08:22:48.496972 liulianmao-1.4.0/src/liulianmao/module/__init__.py
+-rw-r--r--   0        0        0     2864 2024-04-14 08:22:48.515590 liulianmao-1.4.0/src/liulianmao/module/authentication.py
+-rw-r--r--   0        0        0      399 2024-04-01 15:16:20.555012 liulianmao-1.4.0/src/liulianmao/module/const.py
+-rw-r--r--   0        0        0      605 2024-04-01 17:40:59.131588 liulianmao-1.4.0/src/liulianmao/module/log.py
+-rw-r--r--   0        0        0     2347 2024-04-14 09:58:34.104170 liulianmao-1.4.0/src/liulianmao/module/model.py
+-rw-r--r--   0        0        0     1647 2024-05-01 14:53:06.868641 liulianmao-1.4.0/src/liulianmao/module/storage.py
+-rw-r--r--   0        0        0        0 2024-04-03 12:56:52.620830 liulianmao-1.4.0/src/liulianmao/tool/__init__.py
+-rw-r--r--   0        0        0     3728 2024-04-01 11:33:08.073130 liulianmao-1.4.0/src/liulianmao/tool/ls.py
+-rw-r--r--   0        0        0     7593 1970-01-01 00:00:00.000000 liulianmao-1.4.0/PKG-INFO
```

### Comparing `liulianmao-1.3.0/LICENSE` & `liulianmao-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/pyproject.toml` & `liulianmao-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "liulianmao"
-version = "1.3.0"
+version = "1.4.0"
 description = "A LLM client for use from the command line or IDE."
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 repository = "https://github.com/LaoshuBaby/liulianmao"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `liulianmao-1.3.0/README.md` & `liulianmao-1.4.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -37,31 +37,24 @@
 ## 示例
 
 - `python your_script.py` 将使用默认的recipe（即["init", "chat"]）。
 - `python your_script.py --recipe init other_operation` 将使用自定义的recipe（即["init", "other_operation"]）。
 - `python your_script.py --question` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
 - `python your_script.py --question --recipe init other_operation` 将打开并打印`question.txt`文件的内容，并使用自定义的recipe。
 
-## 参考文档
-
-虽然我觉得正常用户用不到这东西，给自己看方便debug的
-
-* https://platform.openai.com/docs/api-reference/audio/createSpeech
-* https://platform.openai.com/docs/guides/text-to-speech
-* https://platform.openai.com/docs/guides/images/language-specific-tips
-
 ## TODO
 
 目前有如下亟待解决的主要问题
 
 * 打包为各平台（Windows/MacOS，Linux用户请自求多福）上可独立执行的单文件程序，[“一键运行”](https://github.com/sherlock-project/sherlock/issues/2011)。
 * 允许将会话内容直接投射到txt中，并读取其更改自动作为回复。
 * 提供一个网页或GUI，直接映射两个文件的状态（可能没有必要，我们不是要重新发明一个图形化的客户端，已经有很多了）。
 * 提供除OpenAI模型以外其他模型的支持，如llama（可能需要考虑一下国内通义千问和文心一言两大模型的API兼容情况。而零一万物已知于OpenAI兼容）。在此基础上，目前的“core”可能要跟进调整，以及适应langchain的`langchain`+`langchain-core`+`langchain-openai`的模块名结构，考虑用`basic`等名称来命名通用部分。毕竟liulianmao是分为restful、sdk、langchain三条路径并驾齐驱，皆可用于展开对话的（核心也是用于CLI对话）。
-  这可能需要同时兼容远端和本地的API实例。并且目前能基于llama模型部署的包括[meta-llama](https://github.com/meta-llama)官方[示例代码](https://github.com/meta-llama/llama3/blob/main/example_chat_completion.py)、[Ollama](https://github.com/ollama/ollama)、[Jan](https://github.com/janhq/jan)等，或许可以考虑尽可能多的适配其API。（好在Ollama提供了[兼容OpenAI](https://github.com/ollama/ollama/blob/main/docs/openai.md)的文档和[原生](https://github.com/ollama/ollama/blob/main/docs/api.md#generate-a-completion)文档）
+  这可能需要同时兼容远端和本地的API实例。并且目前能基于llama模型部署的包括[meta-llama](https://github.com/meta-llama)官方[示例代码](https://github.com/meta-llama/llama3/blob/main/example_chat_completion.py)、[Ollama](https://github.com/ollama/ollama)、[Jan](https://github.com/janhq/jan)等，或许可以考虑尽可能多的适配其API。
+* 注释、日志输出、docstring，多语言化在路上了！方便非汉语开发者！
 
 ## Prompt仓库
 
 提供了一些便捷的Prompt用于在config里面指定角色的时候代替“You are a helpful assistant.” （默认的prompt成本为6个token）
 
 此外，即使所有字段全为空，什么都不做，也会有11个token的消耗。
```

### Comparing `liulianmao-1.3.0/src/liulianmao/__main__.py` & `liulianmao-1.4.0/src/liulianmao/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,33 +83,41 @@
 
     FEATURE = {"core": True, "langchain": False}
 
     spec = importlib.util.find_spec(".core", package="client")
     core = importlib.util.module_from_spec(spec)
     spec.loader.exec_module(core)
 
+    spec_openai = importlib.util.find_spec(".api.openai", package="client")
+    api_openai = importlib.util.module_from_spec(spec_openai)
+    spec_openai.loader.exec_module(api_openai)
+
     if FEATURE["langchain"]:
         # spec = importlib.util.find_spec('.langchain', package='client')
         # langchain = importlib.util.module_from_spec(spec)
         # spec.loader.exec_module(langchain)
         from client.langchain import main as langchain
 
     operations = {
         "default": core.chat,
-        "models": core.models,
+        "models": api_openai.openai_models,
+        "ask": core.ask,
         "chat": core.chat,
         "talk": core.talk,
         "draw": core.draw,
     }
 
     logger.debug(f"[Recipe]: {recipe}")
     for operation_name in recipe:
         operation = operations.get(operation_name)
         if operation:
-            operation()
+            if operation_name == "ask":
+                operation(actions["question"])
+            else:
+                operation()
         else:
             print(f"Operation {operation_name} is not defined.")
 
 
 if __name__ == "__main__":
     init_env()
     default_recipe = ["default"]
```

### Comparing `liulianmao-1.3.0/src/liulianmao/client/core.py` & `liulianmao-1.4.0/src/liulianmao/client/api/openai.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,38 +1,27 @@
-import json
 import os
 import sys
-from typing import List
 from datetime import datetime
+from typing import List
 
 import requests
 
 current_dir = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(current_dir, ".."))
+sys.path.append(os.path.join(current_dir, "..", ".."))
 
+from client.utils.config import load_conf
 from module.authentication import API_KEY, API_URL
 from module.log import logger
 from module.model import select_model
 from module.storage import PROJECT_FOLDER, get_user_folder, init
 
 conversation = []
 
 
-def load_conf():
-    config_file_path = os.path.join(
-        get_user_folder(), PROJECT_FOLDER, "assets", "config.json"
-    )
-    with open(config_file_path, "r", encoding="utf-8") as file:
-        config = json.load(file)
-
-    logger.trace("[Config]\n" + f"{config}")
-    return config
-
-
-def models(model_series :str = ""):
+def openai_models(model_series: str = ""):
     logger.debug(f"[model_series]: {model_series}")
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
     logger.trace("[Headers]\n" + f"{headers}")
 
@@ -40,20 +29,19 @@
 
     def extract_ids(data):
         collected_ids = []
 
         for item in data:
             for key, value in item.items():
                 if key == "id":
-                    if model_series!= "" and model_series in value.lower():
+                    if model_series != "" and model_series in value.lower():
                         collected_ids.append(value)
                     elif model_series == "":
                         collected_ids.append(value)
 
-
         return collected_ids
 
     if response.status_code == 200:
         logger.trace("[Debug] response.status_code == 200")
         # judge mime
         try:
             logger.trace("[Response]\n" + str(response.json()))
@@ -67,62 +55,88 @@
         logger.trace("[Debug] response.status_code != 200")
         logger.error(
             f"Error: {response.status_code} {response.content.decode('utf-8')}"
         )
         return {}
 
 
-def speech(msg):
+def openai_audio_speech(
+    msg,
+    model: str = "tts-1",
+    voice: str = "alloy",
+    response_format: str = "mp3",
+    speed: float = 1.0,
+):
+    def validate_voice(voice: str) -> str:
+        voice_list = ["alloy", "echo", "fable", "onyx", "nova", "shimmer"]
+        if voice not in voice_list:
+            logger.error("voice not supported")
+            return voice_list[0]
+        else:
+            return voice
+
+    def validate_format(response_format: str) -> str:
+        format_list = ["mp3", "opus", "aac", "flac", "wav", "pcm"]
+        if response_format not in format_list:
+            logger.error("responce_format not supported")
+            return format_list[0]
+        else:
+            return response_format
+
+    def validate_speed(speed: float) -> None:
+        min_speed = 0.25
+        max_speed = 4.0
+
+        if speed > max_speed or speed < min_speed:
+            logger.error("speed not supported")
+            return 1.0
+        else:
+            return speed
+
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
-    data = {"model": "tts-1", "input": msg, "voice": "alloy"}
+    data = {
+        "input": msg,
+        "model": model,
+        "voice": validate_voice(voice),
+        "response_format": validate_format(response_format),
+        "speed": validate_speed(speed),
+    }
+
     response = requests.post(
         API_URL + "/v1/audio/speech", json=data, headers=headers
     )
 
     if response.status_code == 200:
-        current_time = datetime.now().isoformat(timespec='milliseconds')
-        safe_filename = current_time.replace(':', '_')
+        current_time = datetime.now().isoformat(timespec="milliseconds")
+        safe_filename = current_time.replace(":", "_")
         speech_file_path = os.path.join(
-            get_user_folder(), PROJECT_FOLDER, "audios", "tts_"+safe_filename+".mp3"
+            get_user_folder(),
+            PROJECT_FOLDER,
+            "audios",
+            f"tts_{safe_filename.lower()}.{response_format.lower()}",
         )
         with open(speech_file_path, "wb") as f:
             f.write(response.content)
-        logger.success("音频文件保存成功。")
+        logger.success(f"音频文件保存成功。{speech_file_path}")
     else:
         logger.error(
             "生成语音失败。状态码：",
             response.status_code,
             "\n",
             response.content.decode("utf-8"),
         )
 
 
-def completion_llama(question: str, model: str, amount: int = 1):
-    headers = {
-        "Content-Type": "application/json",
-    }
-    payload = {
-        "model": model,
-        "messages": question,
-        "temperature": temperature,
-        "n": amount,
-    }
-    logger.trace("[Headers]\n" + f"{headers}")
-    logger.trace("[Payload]\n" + f"{payload}")
-    response = requests.post(
-        API_URL + "/completions", headers=headers, json=payload
-    )
-    return response
-
-
-def completion(question, available_models: List[str] = [], amount: int = 1):
+def openai_chat_completion(
+    question, available_models: List[str] = [], amount: int = 1
+):
     config = load_conf()
     model_type = config["model_type"]
     system_content = config["system_message"]["content"]
     temperature = float(config["settings"]["temperature"])
 
     headers = {
         "Authorization": f"Bearer {API_KEY}",
@@ -192,52 +206,110 @@
         logger.trace("[Debug] response.status_code != 200")
         logger.error(
             f"Error: {response.status_code} {response.content.decode('utf-8')}"
         )
         return {}
 
 
-def generate_image(prompt, num_images: int = 1):
+def openai_images_generations(
+    prompt,
+    model: str = "dall-e-3",
+    size: str = "1024x1024",
+    quality: str = "standard",
+    num: int = 1,
+):
     config = load_conf()
     headers = {
         "Authorization": f"Bearer {API_KEY}",
         "Content-Type": "application/json",
     }
 
     payload = {
-        # "model": "dall-e-3",
+        "model": model,
         "prompt": prompt,
-        "size": "1024x1024",
-        "quality": "standard",
-        "n": 1,
+        "size": size,
+        "quality": quality,
+        "n": num,
     }
 
     logger.trace("[Headers]\n" + f"{headers}")
     logger.trace("[Payload]\n" + f"{payload}")
 
     response = requests.post(
         API_URL + "/v1/images/generations", headers=headers, json=payload
     )
 
     def download_image(url, save_path):
-        
         from urllib.parse import parse_qs, urlparse
 
         parsed_url = urlparse(url)
         file_name = parsed_url.path.split("/")[-1]
-        file_params = parse_qs(parsed_url.query)
 
         # 检查并根据内容类型更改文件后缀
+        file_params = parse_qs(parsed_url.query)
+        logger.trace(f"[extension_check:file_params]: {file_params}")
         response = requests.head(url)
-        if "Content-Type" in response.headers:
-            content_type = response.headers["Content-Type"]
-            file_extension = content_type.split("/")[-1]
-            file_name_no_ext = os.path.splitext(file_name)[0]
-            file_name = f"{file_name_no_ext}.{file_extension}"
+        logger.trace(f"[extension_check:response.headers]: {response.headers}")
+
+        def get_content_type():
+            if file_params.get("rsct", []) != []:
+                return str(file_params["rsct"][0])
+            elif "Content-Type" in response.headers:
+                return str(response.headers["Content-Type"])
+            else:
+                return ""
+
+        if get_content_type():
+            content_type = get_content_type()
+            file_name_ext = content_type.split("/")[-1]
+            file_name_stem = os.path.splitext(file_name)[0]
+            file_name = f"{file_name_stem}.{file_name_ext}"
+
+            def generate_unique_file_name(
+                save_path, file_name_stem, file_name_ext
+            ):
+                full_file_name = f"{file_name_stem}.{file_name_ext}"
+                full_save_path = os.path.join(save_path, full_file_name)
+                file_number = 0
+
+                # 检查文件是否存在，如果存在则在文件名中增加编号
+                if os.path.exists(full_save_path):
+                    logger.trace(
+                        f"[file_name:collision.number]: {full_save_path}"
+                    )
+                    logger.trace(
+                        f"[file_name:collision.exist]: {full_save_path}"
+                    )
+                    while os.path.exists(full_save_path):
+                        logger.trace(
+                            f"[file_name:collision.number]: {full_save_path}"
+                        )
+                        logger.trace(
+                            f"[file_name:collision.exist]: {full_save_path}"
+                        )
+                        file_number += 1
+                        full_file_name = (
+                            f"{file_name_stem}({file_number}).{file_name_ext}"
+                        )
+                        full_save_path = os.path.join(
+                            save_path, full_file_name
+                        )
 
+                    return f"{file_name_stem}({file_number}).{file_name_ext}"
+                else:
+                    return f"{file_name_stem}.{file_name_ext}"
+
+            file_name = generate_unique_file_name(
+                save_path, file_name_stem, file_name_ext
+            )
+        else:
+            logger.warning(
+                "haven't get image content_type and use default filename"
+            )
+            file_name = file_name
         logger.trace(f"[file_name]: {file_name}")
 
         # 下载文件
         response = requests.get(url)
         if response.status_code == 200:
             full_save_path = os.path.join(save_path, file_name)
             with open(full_save_path, "wb") as f:
@@ -279,141 +351,7 @@
                 f.write(response.content)
             logger.success("图片文件保存成功。")
         else:
             logger.warning("未知的内容类型。")
     else:
         logger.error(f"响应状态码错误：{response.status_code}")
         logger.error(response.content.decode("utf-8"))
-
-
-def ask(msg: str, available_models: List[str], default_amount: int = 1):
-    response = completion(msg, available_models, amount=default_amount)
-    try:
-        choices = response.get("choices", [])
-
-        # 使用.get()方法更安全地访问字典键值，以避免KeyError异常
-        response_usage_completion_tokens = response.get("usage", {}).get(
-            "completion_tokens", -1
-        )
-        response_usage_prompt_tokens = response.get("usage", {}).get(
-            "prompt_tokens", -1
-        )
-        response_usage_total_tokens = response.get("usage", {}).get(
-            "total_tokens", -1
-        )
-
-        # 假设这里有一些处理response的代码
-
-    except Exception as e:
-        # 记录关键错误信息而不是直接退出程序，提供更好的错误上下文
-        logger.exception(f"An error occurred: {e}", exc_info=True)
-        # 可以在这里处理特定的清理工作，如果有必要的话
-        # 最后，可能会根据程序的需要选择是否退出
-        # sys.exit()
-
-    # 使用展平路径的变量名进行日志记录
-    logger.debug(
-        "[Token Usage]\n"
-        + json.dumps(
-            {
-                "response_usage_completion_tokens": response_usage_completion_tokens,
-                "response_usage_prompt_tokens": response_usage_prompt_tokens,
-                "response_usage_total_tokens": response_usage_total_tokens,
-                # 计算验证
-                "verify": f"{response_usage_completion_tokens} + {response_usage_prompt_tokens} = {response_usage_completion_tokens + response_usage_prompt_tokens}",
-            },
-            indent=2,
-            ensure_ascii=False,
-            sort_keys=False,
-        )
-    )
-
-    # 根据choices的数量来输出
-    for i, choice in enumerate(choices):
-        logger.success(
-            f"[Answer] ({i + 1}/{len(choices)})\n{choice['message']['content']}"
-        )
-
-    # 为了保持函数的兼容性（返回单一或多个答案），返回整个choices列表的消息内容
-    return [choice["message"]["content"] for choice in choices]
-
-
-def chat():
-    init()
-    available_models = models("gpt")
-
-    with open(
-        os.path.join(
-            get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
-        ),
-        "r",
-        encoding="utf-8",
-    ) as file:
-        msg = file.read()
-
-    flag_continue = True
-    conversation = ask(msg, available_models)
-
-    if not flag_continue:
-        with open(
-            os.path.join(
-                get_user_folder(), PROJECT_FOLDER, "terminal", "answer.txt"
-            ),
-            "w",
-            encoding="utf-8",
-        ) as file:
-            file.write(conversation)
-    else:
-        flag_end = False
-        while not flag_end:
-            import time
-
-            # 部分控制台输入是异步的，给足够的时间以保证不会打断输出
-            time.sleep(0.05)
-            logger.info("[Interaction] 请输入追问")
-            append_question = input()
-            append_question_judge = append_question.replace("\n", "").replace(
-                " ", ""
-            )
-            if append_question_judge != "END" and append_question_judge != "":
-                conversation = ask(append_question, available_models)
-            else:
-                flag_end = True
-                break
-
-
-def talk():
-    init()
-    available_models = models("tts")
-
-    with open(
-        os.path.join(
-            get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
-        ),
-        "r",
-        encoding="utf-8",
-    ) as f:
-        msg = f.read()
-    speech(msg)
-
-
-def draw():
-    init()
-    available_models = models("dall-e")
-    with open(
-        os.path.join(
-            get_user_folder(), PROJECT_FOLDER, "terminal", "question.txt"
-        ),
-        "r",
-        encoding="utf-8",
-    ) as f:
-        msg = f.read()
-    generate_image(msg)
-
-
-def main():
-    logger.critical("THIS PROGRAM NOT INTENT TO RUN SUBMODULE".upper())
-    exit(0)
-
-
-if __name__ == "__main__":
-    main()
```

### Comparing `liulianmao-1.3.0/src/liulianmao/client/langchain.py` & `liulianmao-1.4.0/src/liulianmao/client/langchain.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/src/liulianmao/module/authentication.py` & `liulianmao-1.4.0/src/liulianmao/module/authentication.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/src/liulianmao/module/log.py` & `liulianmao-1.4.0/src/liulianmao/module/log.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/src/liulianmao/module/model.py` & `liulianmao-1.4.0/src/liulianmao/module/model.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/src/liulianmao/module/storage.py` & `liulianmao-1.4.0/src/liulianmao/module/storage.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/src/liulianmao/tool/ls.py` & `liulianmao-1.4.0/src/liulianmao/tool/ls.py`

 * *Files identical despite different names*

### Comparing `liulianmao-1.3.0/PKG-INFO` & `liulianmao-1.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liulianmao
-Version: 1.3.0
+Version: 1.4.0
 Summary: A LLM client for use from the command line or IDE.
 Home-page: https://github.com/LaoshuBaby/liulianmao
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -63,31 +63,24 @@
 ## 示例
 
 - `python your_script.py` 将使用默认的recipe（即["init", "chat"]）。
 - `python your_script.py --recipe init other_operation` 将使用自定义的recipe（即["init", "other_operation"]）。
 - `python your_script.py --question` 将打开并打印`question.txt`文件的内容，并使用默认的recipe。
 - `python your_script.py --question --recipe init other_operation` 将打开并打印`question.txt`文件的内容，并使用自定义的recipe。
 
-## 参考文档
-
-虽然我觉得正常用户用不到这东西，给自己看方便debug的
-
-* https://platform.openai.com/docs/api-reference/audio/createSpeech
-* https://platform.openai.com/docs/guides/text-to-speech
-* https://platform.openai.com/docs/guides/images/language-specific-tips
-
 ## TODO
 
 目前有如下亟待解决的主要问题
 
 * 打包为各平台（Windows/MacOS，Linux用户请自求多福）上可独立执行的单文件程序，[“一键运行”](https://github.com/sherlock-project/sherlock/issues/2011)。
 * 允许将会话内容直接投射到txt中，并读取其更改自动作为回复。
 * 提供一个网页或GUI，直接映射两个文件的状态（可能没有必要，我们不是要重新发明一个图形化的客户端，已经有很多了）。
 * 提供除OpenAI模型以外其他模型的支持，如llama（可能需要考虑一下国内通义千问和文心一言两大模型的API兼容情况。而零一万物已知于OpenAI兼容）。在此基础上，目前的“core”可能要跟进调整，以及适应langchain的`langchain`+`langchain-core`+`langchain-openai`的模块名结构，考虑用`basic`等名称来命名通用部分。毕竟liulianmao是分为restful、sdk、langchain三条路径并驾齐驱，皆可用于展开对话的（核心也是用于CLI对话）。
-  这可能需要同时兼容远端和本地的API实例。并且目前能基于llama模型部署的包括[meta-llama](https://github.com/meta-llama)官方[示例代码](https://github.com/meta-llama/llama3/blob/main/example_chat_completion.py)、[Ollama](https://github.com/ollama/ollama)、[Jan](https://github.com/janhq/jan)等，或许可以考虑尽可能多的适配其API。（好在Ollama提供了[兼容OpenAI](https://github.com/ollama/ollama/blob/main/docs/openai.md)的文档和[原生](https://github.com/ollama/ollama/blob/main/docs/api.md#generate-a-completion)文档）
+  这可能需要同时兼容远端和本地的API实例。并且目前能基于llama模型部署的包括[meta-llama](https://github.com/meta-llama)官方[示例代码](https://github.com/meta-llama/llama3/blob/main/example_chat_completion.py)、[Ollama](https://github.com/ollama/ollama)、[Jan](https://github.com/janhq/jan)等，或许可以考虑尽可能多的适配其API。
+* 注释、日志输出、docstring，多语言化在路上了！方便非汉语开发者！
 
 ## Prompt仓库
 
 提供了一些便捷的Prompt用于在config里面指定角色的时候代替“You are a helpful assistant.” （默认的prompt成本为6个token）
 
 此外，即使所有字段全为空，什么都不做，也会有11个token的消耗。
```

