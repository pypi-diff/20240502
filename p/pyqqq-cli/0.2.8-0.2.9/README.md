# Comparing `tmp/pyqqq_cli-0.2.8.tar.gz` & `tmp/pyqqq_cli-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqqq_cli-0.2.8.tar", max compression
+gzip compressed data, was "pyqqq_cli-0.2.9.tar", max compression
```

## Comparing `pyqqq_cli-0.2.8.tar` & `pyqqq_cli-0.2.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1064 2024-04-24 03:51:23.461068 pyqqq_cli-0.2.8/README.md
--rw-r--r--   0        0        0      655 2024-04-24 05:46:39.778829 pyqqq_cli-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      358 2024-04-03 03:46:05.358635 pyqqq_cli-0.2.8/qupiato/cli/config.py
--rw-r--r--   0        0        0     8645 2024-04-24 05:44:57.315544 pyqqq_cli-0.2.8/qupiato/cli/main.py
--rw-r--r--   0        0        0     5863 2024-04-24 05:34:08.906077 pyqqq_cli-0.2.8/qupiato/cli/utils.py
--rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-22 08:23:09.109923 pyqqq_cli-0.2.9/README.md
+-rw-r--r--   0        0        0      655 2024-05-02 09:48:21.706887 pyqqq_cli-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      358 2024-05-02 09:40:11.894616 pyqqq_cli-0.2.9/qupiato/cli/config.py
+-rw-r--r--   0        0        0     8773 2024-05-02 09:40:59.528982 pyqqq_cli-0.2.9/qupiato/cli/main.py
+-rw-r--r--   0        0        0     7097 2024-05-02 09:45:29.468608 pyqqq_cli-0.2.9/qupiato/cli/utils.py
+-rw-r--r--   0        0        0     1936 1970-01-01 00:00:00.000000 pyqqq_cli-0.2.9/PKG-INFO
```

### Comparing `pyqqq_cli-0.2.8/README.md` & `pyqqq_cli-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `pyqqq_cli-0.2.8/pyproject.toml` & `pyqqq_cli-0.2.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyqqq-cli"
-version = "0.2.8"
+version = "0.2.9"
 description = "CLI tool for controlling strategies deployed on the PyQQQ platform."
 authors = ["PyQQQ team <pyqqq.cs@gmail.com>"]
 readme = "README.md"
 packages = [{include = "qupiato"}]
 license = "MIT"
 documentation = "https://qupiato-sdk-18secs-cf54ebea1b14b422537daf0462fb86d68f4582d064a4.gitlab.io"
```

### Comparing `pyqqq_cli-0.2.8/qupiato/cli/main.py` & `pyqqq_cli-0.2.9/qupiato/cli/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from pyqqq.executors.hook import HookExecutor
-from qupiato.cli.utils import create_and_upload_to_gcs_bucket, get_token, ws_api_call, get_version, get_agent, encode_secret, search_strategies, get_user, pull_strategy
+from qupiato.cli.utils import create_and_upload_to_gcs_bucket, get_token, ws_api_call, get_version, get_agent, encode_secret, search_strategies, get_user, pull_strategy, publish_strategy
 import asyncio
 import click
 import datetime as dtm
 import importlib
 import os
 import qupiato.cli.config as c
 import re
@@ -68,14 +68,18 @@
         "publish": publish
     }
 
     async for line in ws_api_call(req):
         if 'text' in line:
             click.echo(line['text'])
 
+    if publish:
+        click.echo("Publishing strategy")
+        publish_strategy(entryfile, strategy_name)
+
 
 @main.command()
 def list():
     """ List deployed strategies """
 
     asyncio.run(list_strategies())
```

### Comparing `pyqqq_cli-0.2.8/qupiato/cli/utils.py` & `pyqqq_cli-0.2.9/qupiato/cli/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 import tempfile
 import uuid
 import websockets
 import zipfile
 import base64
 from dotenv import dotenv_values
 import io
+import re
 
 async def ws_api_call(req: Dict):
     async with websockets.connect(c.DEPLOYER_WS_URL) as ws:
         await ws.send(json.dumps(req))
 
         while True:
             try:
@@ -136,14 +137,49 @@
     with io.BytesIO() as buffer:
         for chunk in response.iter_content(None):
             buffer.write(chunk)
 
         with zipfile.ZipFile(buffer) as zipf:
             zipf.extractall(name)
 
+# 전략의 공개 설정
+def publish_strategy(entryfile, strategy_name):
+    entry_dir = os.path.dirname(os.path.normpath(entryfile))
+    markdown = None
+    for root, _, files in os.walk(entry_dir or '.'):
+        if markdown is not None:
+            break
+
+        for file in files:
+            file_path = os.path.join(root, file)
+            norm_path = os.path.normpath(file_path)
+            d_name = os.path.dirname(norm_path)
+
+            if entry_dir == d_name and re.match('readme.md', os.path.basename(norm_path), re.I):
+                markdown = norm_path
+                break
+
+    url = f"{c.API_SERVER_URL}/strategy/publish"
+    headers = {
+        'Authorization': f'Bearer {get_token()}'
+    }
+    payload = { 'strategy': strategy_name }
+
+    if markdown:
+        files = { 'file': (os.path.basename(markdown), open(markdown, 'rb'), 'application/octet-stream') }
+        response = requests.post(url, headers=headers, files=files, data=payload)
+    else:
+        response = requests.post(url, headers=headers, data=payload)
+
+    if response.status_code != 200 and response.status_code != 201:
+        raise Exception("Publish failed to strategies")
+
+    return response.json()
+
+# 사용자 정보 조회
 def get_user(uid):
     url = f"{c.API_SERVER_URL}/user"
     headers = {
         'Authorization': f'Bearer {get_token()}'
     }
     response = requests.get(url, headers=headers, params={'uid': uid})
```

### Comparing `pyqqq_cli-0.2.8/PKG-INFO` & `pyqqq_cli-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqqq-cli
-Version: 0.2.8
+Version: 0.2.9
 Summary: CLI tool for controlling strategies deployed on the PyQQQ platform.
 License: MIT
 Author: PyQQQ team
 Author-email: pyqqq.cs@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

