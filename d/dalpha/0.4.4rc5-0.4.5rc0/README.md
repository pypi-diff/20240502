# Comparing `tmp/dalpha-0.4.4rc5.tar.gz` & `tmp/dalpha-0.4.5rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.4.4rc5.tar", max compression
+gzip compressed data, was "dalpha-0.4.5rc0.tar", max compression
```

## Comparing `dalpha-0.4.4rc5.tar` & `dalpha-0.4.5rc0.tar`

### file list

```diff
@@ -1,15 +1,20 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.4rc5/README.md
--rw-r--r--   0        0        0    30518 2024-04-22 12:19:21.276903 dalpha-0.4.4rc5/dalpha/__init__.py
--rw-r--r--   0        0        0      548 2024-04-19 16:22:01.493908 dalpha-0.4.4rc5/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/context.py
--rw-r--r--   0        0        0     1716 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/dalpha_openai.py
--rw-r--r--   0        0        0      178 2024-04-22 06:41:31.414519 dalpha-0.4.4rc5/dalpha/error_code.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.4rc5/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.4rc5/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/logging/utils.py
--rw-r--r--   0        0        0     5846 2024-03-06 10:11:38.540030 dalpha-0.4.4rc5/dalpha/redis.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.4rc5/dalpha/signal_handler.py
--rw-r--r--   0        0        0      881 2024-04-22 12:19:21.276903 dalpha-0.4.4rc5/pyproject.toml
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.4rc5/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.4.5rc0/README.md
+-rw-r--r--   0        0        0     1862 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0    29060 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/agent.py
+-rw-r--r--   0        0        0      548 2024-04-19 16:22:01.493908 dalpha-0.4.5rc0/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/dto.py
+-rw-r--r--   0        0        0      521 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/exception.py
+-rw-r--r--   0        0        0     6098 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.4.5rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.4.5rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     1702 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.4.5rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0      881 2024-05-02 07:23:00.795089 dalpha-0.4.5rc0/pyproject.toml
+-rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 dalpha-0.4.5rc0/PKG-INFO
```

### Comparing `dalpha-0.4.4rc5/README.md` & `dalpha-0.4.5rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc5/dalpha/__init__.py` & `dalpha-0.4.5rc0/dalpha/agent.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,121 +1,20 @@
-import requests, json, boto3, io, logging, sys, os, pkg_resources
+import requests, json, boto3, io, sys, os
 import time
 import sentry_sdk
 from requests.adapters import HTTPAdapter, Retry
 from dataclasses import asdict
 
-from dalpha.cobra_cls import Cobra
-
 from dalpha.signal_handler import get_shutdown_requested
 from dalpha.context import clear_context_evaluate, set_context, set_context_evaluate, get_context, Context
 from dalpha.logging import logger
 from dalpha.logging.events import Event
 
-from dalpha.error_code import BaseStatusCode
-
-def __load_config(file_path):
-    if not os.path.isfile(file_path):
-        logger.warning(f"{file_path} 파일을 찾을 수 없습니다.")
-        return
-    
-    with open(file_path, 'r') as file:
-        lines = file.readlines()
-    
-    for line in lines:
-        line = line.strip()
-        if line and not line.startswith("#"):
-            key, value = line.split("=")
-            if os.environ.get(key) is None:
-                os.environ[key] = value
-
-def get_env_var_or_raise(var_name):
-    """
-    환경변수를 가져오거나 없으면 에러를 발생시킴
-    """
-    value = os.environ.get(var_name)
-    if value is None:
-        raise ValueError(f"Environment variable {var_name} is not set")
-    return value
-
-def check_package_version(package_name):
-    installed_version = pkg_resources.get_distribution(package_name).version
-    try:
-        url = f"https://pypi.org/pypi/{package_name}/json"
-        response = requests.get(url)
-        data = response.json()
-        latest_version = data["info"]["version"]
-        if latest_version != installed_version:
-            logger.warning(" dalpha sdk 버전 -> " + installed_version + " / 최신 버전 -> " + latest_version)
-        else:
-            logger.info(" dalpha sdk 버전 -> " + installed_version + " (latest)")
-    except Exception as e:
-        logger.warning(f"dalpha sdk 버전 확인 중 오류가 발생했습니다:{e}")
-cfg_path = os.path.join(sys.path[0],'.dalphacfg')
-__load_config(cfg_path)
-check_package_version("dalpha")
-
-class DalphaRedis:
-    def __init__(self, client: str, db_num: int):
-        self.rd = self.setup(db_num)
-        self.client = client
-
-    def setup(self, db_num):
-        try:
-            import redis
-            from redis.backoff import ExponentialBackoff
-            from redis.retry import Retry
-            from redis.exceptions import (
-            BusyLoadingError,
-            ConnectionError,
-            TimeoutError
-            )
-            retry = Retry(ExponentialBackoff(), 3)
+from dalpha.exception import BaseStatusCode
 
-        except ImportError:
-            raise ImportError("Please install redis-py package -> pip install redis")
-        
-        return redis.StrictRedis(
-            host="k8s-redis-redis-8a93856597-98eab959ed2cbb3e.elb.ap-northeast-2.amazonaws.com",
-            port=6379,
-            decode_responses=True,
-            password=os.environ.get("REDIS_PASSWORD"),
-            retry = retry,
-            retry_on_error = [BusyLoadingError, ConnectionError, TimeoutError],
-            db = db_num
-        )
-
-    def get(self, key: str):
-        key = f"{self.client}-{key}"
-        json_dict = self.rd.get(key)
-        if json_dict:
-
-            return_lst = json.loads(json_dict)
-            return return_lst
-        else:
-            return None
-
-    def set(self, key: str, value, expire: int = None):
-        key = f"{self.client}-{key}"
-        try:
-            json_dict = json.dumps(value, ensure_ascii=False).encode("utf-8")
-            self.rd.set(key, json_dict, ex=expire)
-            return True
-        except Exception as e:
-            logger.error(f"Error : {e}")
-            return False
-
-    def delete(self, key: str):
-        key = f"{self.client}-{key}"
-        try:
-            self.rd.delete(key)
-            return True
-        except Exception as e:
-            logger.error(f"Error : {e}")
-            return False
 
 class Agent:
     def __get_internal_slack(self, header, api_id):
         try:
             response = requests.request("GET", os.path.join(self.base_url, f'inferences/{api_id}/owner'), headers=header)
             account = response.json()
             if account == -1:
@@ -405,42 +304,43 @@
                     message = f"return sqs item: {ret}",
                     event = Event.POLL,
                     data = ret
                 )
                 self.poll_time = time.time()
                 return ret
 
-        time.sleep(0.2)
-        url = f"{self.evaluate_url}/poll"
+        else:
+            time.sleep(0.2)
+            url = f"{self.evaluate_url}/poll"
 
-        headers = {
-        'token': self.token
-        }
-        try:
-            response = requests.request("GET", url, headers=headers, timeout=10)
-        except requests.exceptions.Timeout:
-            logger.warning(f'error from poll / time-out \n poll function will return None.')
-            return None
-        if response.status_code == 422:
-            return None
-        elif response.status_code != 200:
-            logger.warning(f'error from poll / response status_code {response.status_code}: {response.text} \n poll function will return None.')
-            return None
-        logger.info(
-            message = "return poll item",
-            event = Event.POLL,
-            data = response.json()
-        )
-        set_context_evaluate(
-            evaluate_id=response.json()['id'],
-            account_id=response.json()['accountId']
-        )
-        sentry_sdk.set_context("context",asdict(get_context()))
-        self.poll_time = time.time()
-        return response.json()
+            headers = {
+            'token': self.token
+            }
+            try:
+                response = requests.request("GET", url, headers=headers, timeout=10)
+            except requests.exceptions.Timeout:
+                logger.warning(f'error from poll / time-out \n poll function will return None.')
+                return None
+            if response.status_code == 422:
+                return None
+            elif response.status_code != 200:
+                logger.warning(f'error from poll / response status_code {response.status_code}: {response.text} \n poll function will return None.')
+                return None
+            logger.info(
+                message = "return poll item",
+                event = Event.POLL,
+                data = response.json()
+            )
+            set_context_evaluate(
+                evaluate_id=response.json()['id'],
+                account_id=response.json()['accountId']
+            )
+            sentry_sdk.set_context("context",asdict(get_context()))
+            self.poll_time = time.time()
+            return response.json()
 
     def update_poll(self):
         '''
         data update의 경우 kafka로부터 data update event가 담긴 메세지를 받아온다.
         '''
         record = self.kafka_consumer.poll(
             timeout_ms=5000,
@@ -643,43 +543,97 @@
                     return
                 else:
                     message = f'error from validate_error / response status_code {response.status_code}: {response.text}'
                     sentry_sdk.capture_message(message)
                     raise Exception(message)
         finally:
             clear_context_evaluate()
-        
+
+    def internal_call(self, service_code:str, key:str, metadata:dict, polling_interval=0.5, time_out=60):
+        '''
+        service_code : 서비스 코드
+        key : key
+        metadata : 요청할 메타데이터
+        polling_interval : 폴링 간격
+        max_polling_time : 최대 폴링 횟수
+        '''
+        header = {
+            'X-Api-Key': os.environ.get('INTERNAL_X_API_KEY'),
+            'Content-Type': 'application/json'
+        }
+        url = os.path.join(self.base_url, f'partner/polling/{service_code}/{key}')
+        with requests.Session() as s:
+            retries = Retry(total=self.max_retry, backoff_factor=0.05, status_forcelist=[ 500, 502, 503, 504 ])
+            adapter = HTTPAdapter(max_retries=retries)
+            s.mount('http://', adapter)
+            s.mount('https://', adapter)
+            response = s.post(url, headers=header, data=json.dumps(metadata))
+            if response.status_code == 200:
+                eval_id = response.json()['id']
+            else:
+                message = f'error from internal_call(post) / response status_code {response.status_code}: {response.text}'
+                sentry_sdk.capture_message(message)
+                raise Exception(message)
+        while time_out > 0:
+            time.sleep(polling_interval)
+            time_out -= polling_interval
+            with requests.Session() as s:
+                retries = Retry(total=self.max_retry, backoff_factor=0.05, status_forcelist=[ 500, 502, 503, 504 ])
+                adapter = HTTPAdapter(max_retries=retries)
+                s.mount('http://', adapter)
+                s.mount('https://', adapter)
+                response = s.get(os.path.join(self.base_url, f'partner/{service_code}/{key}/{eval_id}'), headers=header)
+                if response.status_code == 202:
+                    continue
+                elif response.status_code == 200:
+                    if response.json()['success'] == True:
+                        return response.json()['payload']
+                    else:
+                        message = f'error response from internal_call(get) / response status_code {response.status_code}: {response.text}'
+                        sentry_sdk.capture_message(message)
+                        raise Exception(message)
+                else:
+                    message = f'error from internal_call(get) / response status_code {response.status_code}: {response.text}'
+                    sentry_sdk.capture_message(message)
+                    raise Exception(message)
+        message = f'internal_call timeout'
+        sentry_sdk.capture_message(message)
+        raise Exception(message)
+
     def download_from_url(self, url):
         r = requests.get(url, stream=True)
         if r.status_code != 200:
             raise Exception(f"can't download from url {r.status_code} : {r.text}")
         else:
             return io.BytesIO(r.content)
             # return Image.open(io.BytesIO(r.content)).convert('RGB')
 
+
     def download_from_s3(self, bucket, key, download_path):
         try:
             self.s3.download_file(bucket, key, download_path)
         except Exception as e:
             raise Exception(f"failed to download from s3\n{e}")
 
+
     def upload_s3(self, upload_path, bucket, key = None, account_id = None):
         if key is None and account_id is not None:
             if not isinstance(account_id, int): raise TypeError('account_id is not a int')
             key = f"channel_id={account_id}/{time.strftime('y=%Y/m=%m/d=%d', time.localtime(time.time()))}/{os.path.basename(upload_path)}"
         try:
             self.s3.upload_file(upload_path, bucket, key)
             logger.info(
                 message = f"uploaded to s3://{bucket}/{key}",
                 event = Event.UPLOAD_S3,
             )
             return os.path.join(f"https://{bucket}.s3.ap-northeast-2.amazonaws.com", key)
         except Exception as e:
             raise Exception(f"failed to upload s3\n{e}")
 
+
     def upload_s3_image(self, pil_image, bucket, img_save_name = None, key = None, account_id = None):
         '''
         pil_image : PIL.Image
         bucket : S3에 업로드할 버킷 이름
         img_save_name : S3에 저장될 이미지 파일 이름
         key : S3에 저장될 이미지 파일 경로
         account_id : S3에 저장될 이미지 파일 경로에 포함될 account_id
@@ -703,35 +657,15 @@
                 message = f"uploaded to s3://{bucket}/{key}",
                 event = Event.UPLOAD_S3,
             )
             return os.path.join(f"https://{bucket}.s3.ap-northeast-2.amazonaws.com", key)
         except Exception as e:
             raise Exception(f"failed to upload s3\n{e}")
 
-    def stop_instance(self):
-        try:
-            res = requests.request("GET", 'http://169.254.169.254/latest/meta-data/instance-id')
-            if res.status_code != 200:
-                raise Exception("get instance-id failed!")
-            instance_id = res.text[2:]
-            
-            url = f"https://api.dalpha.so/instances/{instance_id}/stop/@sdk"
-
-            headers = {
-                'token': self.token,
-                'Content-Type': 'application/json'
-            }
-
-            response = requests.request("PUT", url, headers=headers)
-            if response.status_code != 200:
-                raise Exception(f'error from stop_instance / response status_code {response.status_code}')
 
-        except Exception as e:
-            raise Exception(f"error from stop_instance\n{e}")
-        
     def slack_alert(self, channel_name, text):
         '''
         channel_name : slack 채널 id 또는 #채널명
         text : 보낼 메세지
         원하는 slack channel에 메세지를 보내는 함수
         '''
         headers = {
```

### Comparing `dalpha-0.4.4rc5/dalpha/cobra_cls.py` & `dalpha-0.4.5rc0/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc5/dalpha/context.py` & `dalpha-0.4.5rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc5/dalpha/dalpha_openai.py` & `dalpha-0.4.5rc0/dalpha/openai_cls.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 from dalpha.logging.events import Event
-from dalpha.logging.log_formatter import logger
+from dalpha.logging import logger
 
 class DalphaOpenAI:
     def __init__(self, api_key):
         from openai import OpenAI
         self.api_key = api_key
         self.client = OpenAI(api_key=self.api_key)
```

### Comparing `dalpha-0.4.4rc5/dalpha/logging/__init__.py` & `dalpha-0.4.5rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc5/dalpha/logging/log_formatter.py` & `dalpha-0.4.5rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc5/dalpha/logging/utils.py` & `dalpha-0.4.5rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.4.4rc5/dalpha/redis.py` & `dalpha-0.4.5rc0/dalpha/redis_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,22 @@
 import json
 import os
-from dalpha import get_env_var_or_raise
 from dalpha.logging import logger
 
+
+def get_env_var_or_raise(var_name):
+    """
+    환경변수를 가져오거나 없으면 에러를 발생시킴
+    """
+    value = os.environ.get(var_name)
+    if value is None:
+        raise ValueError(f"Environment variable {var_name} is not set")
+    return value
+
+
 class DalphaRedisClient:
     def __init__(self, service_code: str, db_num: int = 0):
         self.rd = self.setup(db_num)
         self.namespace = service_code
         
     def __to_redis_key(self, key: str):
         return f"{self.namespace}:{key}"
@@ -146,8 +156,8 @@
             full_key = self.__to_redis_key(key)
             while cursor != 0:
                 cursor, part_data = await self.rd.hscan(full_key, cursor, match=pattern, count=batch_count)
                 hash_contents.update(part_data.items())
             return hash_contents
         except Exception as e:
             logger.error(f"Dalpha Redis Error: {e}")
-            return None
+            return None
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dalpha-0.4.4rc5/pyproject.toml` & `dalpha-0.4.5rc0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.4.4rc5"
+version = "0.4.5rc0"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -16,17 +16,17 @@
 kafka-python = "^2.0.2"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.4.4rc5"
+version = "0.4.5rc0"
 authors = [
-  { name="Beomseok", email="beomseok.lee@dalpha.so" },
+  { name="Beomseok", email="beomseok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `dalpha-0.4.4rc5/PKG-INFO` & `dalpha-0.4.5rc0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.4.4rc5
+Version: 0.4.5rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

