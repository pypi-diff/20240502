# Comparing `tmp/justai-3.2.9.tar.gz` & `tmp/justai-3.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "justai-3.2.9.tar", last modified: Fri Apr  5 11:22:35 2024, max compression
+gzip compressed data, was "justai-3.3.1.tar", last modified: Thu May  2 08:29:32 2024, max compression
```

## Comparing `justai-3.2.9.tar` & `justai-3.3.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.561756 justai-3.2.9/
--rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.2.9/LICENSE
--rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.2.9/MANIFEST.in
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 11:22:35.561535 justai-3.2.9/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)     4082 2024-04-05 11:22:34.000000 justai-3.2.9/README.md
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.554285 justai-3.2.9/justai/
--rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.2.9/justai/__init__.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.555878 justai-3.2.9/justai/agent/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.2.9/justai/agent/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.2.9/justai/agent/agent.py
--rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.2.9/justai/agent/message.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.556505 justai-3.2.9/justai/interactive/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.2.9/justai/interactive/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.2.9/justai/interactive/commands.py
--rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.2.9/justai/interactive/repl.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.557916 justai-3.2.9/justai/models/
--rw-r--r--   0 hp         (501) staff       (20)     2833 2024-04-05 09:47:29.000000 justai-3.2.9/justai/models/anthropic_models.py
--rw-r--r--   0 hp         (501) staff       (20)     2334 2024-03-21 09:14:50.000000 justai-3.2.9/justai/models/gguf_models.py
--rw-r--r--   0 hp         (501) staff       (20)      871 2024-03-21 08:22:51.000000 justai-3.2.9/justai/models/model.py
--rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.2.9/justai/models/modelfactory.py
--rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.2.9/justai/models/openai_models.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.559411 justai-3.2.9/justai/tools/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.2.9/justai/tools/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.2.9/justai/tools/cache.py
--rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.2.9/justai/tools/display.py
--rw-r--r--   0 hp         (501) staff       (20)     3226 2024-04-02 08:38:55.000000 justai-3.2.9/justai/tools/log.py
--rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.2.9/justai/tools/prompts.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.560631 justai-3.2.9/justai/translator/
--rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.2.9/justai/translator/__init__.py
--rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.2.9/justai/translator/languages.py
--rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.2.9/justai/translator/prompts.toml
--rw-r--r--   0 hp         (501) staff       (20)    14480 2024-04-05 11:22:16.000000 justai-3.2.9/justai/translator/translator.py
--rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.2.9/justai/translator/xliff.py
-drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-04-05 11:22:35.560986 justai-3.2.9/justai.egg-info/
--rw-r--r--   0 hp         (501) staff       (20)     6408 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/PKG-INFO
--rw-r--r--   0 hp         (501) staff       (20)      785 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/SOURCES.txt
--rw-r--r--   0 hp         (501) staff       (20)        1 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/dependency_links.txt
--rw-r--r--   0 hp         (501) staff       (20)      137 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/requires.txt
--rw-r--r--   0 hp         (501) staff       (20)        7 2024-04-05 11:22:35.000000 justai-3.2.9/justai.egg-info/top_level.txt
--rw-r--r--   0 hp         (501) staff       (20)      887 2024-04-05 11:22:34.000000 justai-3.2.9/pyproject.toml
--rw-r--r--   0 hp         (501) staff       (20)       38 2024-04-05 11:22:35.561797 justai-3.2.9/setup.cfg
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.127888 justai-3.3.1/
+-rw-r--r--   0 hp         (501) staff       (20)     1211 2020-11-28 21:10:12.000000 justai-3.3.1/LICENSE
+-rw-r--r--   0 hp         (501) staff       (20)      198 2024-02-20 10:20:38.000000 justai-3.3.1/MANIFEST.in
+-rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-02 08:29:32.127579 justai-3.3.1/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)     4082 2024-05-02 08:29:29.000000 justai-3.3.1/README.md
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.117151 justai-3.3.1/justai/
+-rw-r--r--   0 hp         (501) staff       (20)      579 2024-04-01 20:26:06.000000 justai-3.3.1/justai/__init__.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.119347 justai-3.3.1/justai/agent/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:05:20.000000 justai-3.3.1/justai/agent/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5992 2024-03-31 21:07:33.000000 justai-3.3.1/justai/agent/agent.py
+-rw-r--r--   0 hp         (501) staff       (20)      997 2024-03-05 16:49:21.000000 justai-3.3.1/justai/agent/message.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.120430 justai-3.3.1/justai/interactive/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:06:50.000000 justai-3.3.1/justai/interactive/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     5452 2024-02-07 19:49:01.000000 justai-3.3.1/justai/interactive/commands.py
+-rw-r--r--   0 hp         (501) staff       (20)     1320 2024-03-05 16:26:44.000000 justai-3.3.1/justai/interactive/repl.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.122134 justai-3.3.1/justai/models/
+-rw-r--r--   0 hp         (501) staff       (20)     2987 2024-04-30 15:37:24.000000 justai-3.3.1/justai/models/anthropic_models.py
+-rw-r--r--   0 hp         (501) staff       (20)     2465 2024-05-02 08:28:02.000000 justai-3.3.1/justai/models/gguf_models.py
+-rw-r--r--   0 hp         (501) staff       (20)      920 2024-04-30 15:42:29.000000 justai-3.3.1/justai/models/model.py
+-rw-r--r--   0 hp         (501) staff       (20)      709 2024-03-06 13:20:05.000000 justai-3.3.1/justai/models/modelfactory.py
+-rw-r--r--   0 hp         (501) staff       (20)     5907 2024-04-04 20:33:40.000000 justai-3.3.1/justai/models/openai_models.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.123830 justai-3.3.1/justai/tools/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:08:21.000000 justai-3.3.1/justai/tools/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     3815 2024-04-02 09:00:24.000000 justai-3.3.1/justai/tools/cache.py
+-rw-r--r--   0 hp         (501) staff       (20)      563 2023-08-26 19:32:55.000000 justai-3.3.1/justai/tools/display.py
+-rw-r--r--   0 hp         (501) staff       (20)     3479 2024-04-29 12:34:52.000000 justai-3.3.1/justai/tools/log.py
+-rw-r--r--   0 hp         (501) staff       (20)      615 2024-02-09 15:06:31.000000 justai-3.3.1/justai/tools/prompts.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.126026 justai-3.3.1/justai/translator/
+-rw-------   0 hp         (501) staff       (20)        0 2024-02-07 16:11:10.000000 justai-3.3.1/justai/translator/__init__.py
+-rw-r--r--   0 hp         (501) staff       (20)     4052 2024-02-13 10:39:31.000000 justai-3.3.1/justai/translator/languages.py
+-rw-r--r--   0 hp         (501) staff       (20)     1759 2024-04-05 09:44:01.000000 justai-3.3.1/justai/translator/prompts.toml
+-rw-r--r--   0 hp         (501) staff       (20)    16620 2024-04-29 12:34:32.000000 justai-3.3.1/justai/translator/translator.py
+-rw-r--r--   0 hp         (501) staff       (20)     5243 2024-02-16 15:51:36.000000 justai-3.3.1/justai/translator/xliff.py
+drwxr-xr-x   0 hp         (501) staff       (20)        0 2024-05-02 08:29:32.126625 justai-3.3.1/justai.egg-info/
+-rw-r--r--   0 hp         (501) staff       (20)     6448 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/PKG-INFO
+-rw-r--r--   0 hp         (501) staff       (20)      785 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/SOURCES.txt
+-rw-r--r--   0 hp         (501) staff       (20)        1 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/dependency_links.txt
+-rw-r--r--   0 hp         (501) staff       (20)      146 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/requires.txt
+-rw-r--r--   0 hp         (501) staff       (20)        7 2024-05-02 08:29:32.000000 justai-3.3.1/justai.egg-info/top_level.txt
+-rw-r--r--   0 hp         (501) staff       (20)      894 2024-05-02 08:29:29.000000 justai-3.3.1/pyproject.toml
+-rw-r--r--   0 hp         (501) staff       (20)       38 2024-05-02 08:29:32.127961 justai-3.3.1/setup.cfg
```

### Comparing `justai-3.2.9/LICENSE` & `justai-3.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/PKG-INFO` & `justai-3.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.9
+Version: 3.3.1
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -39,29 +39,30 @@
 Requires-Dist: tenacity
 Requires-Dist: python-dateutil
 Requires-Dist: python-dotenv
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: tiktoken
 Requires-Dist: lxml
-Requires-Dist: llama-cpp-python
 Requires-Dist: anthropic
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: nox; extra == "dev"
+Provides-Extra: llama
+Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.9
+Current version: 3.3.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.9/README.md` & `justai-3.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.9
+Current version: 3.3.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.9/justai/__init__.py` & `justai-3.3.1/justai/__init__.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/agent/agent.py` & `justai-3.3.1/justai/agent/agent.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/agent/message.py` & `justai-3.3.1/justai/agent/message.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/interactive/commands.py` & `justai-3.3.1/justai/interactive/commands.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/interactive/repl.py` & `justai-3.3.1/justai/interactive/repl.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/models/anthropic_models.py` & `justai-3.3.1/justai/models/anthropic_models.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 
 import anthropic
 from dotenv import load_dotenv
 
-from justai.models.model import Model
+from justai.models.model import Model, OverloadedException
 from justai.tools.display import ERROR_COLOR, color_print
 
 
 # Claude 3 Opus	    claude-3-opus-20240229
 # Claude 3 Sonnet	claude-3-sonnet-20240229
 # Claude 3 Haiku	Coming soon
 
@@ -49,21 +49,24 @@
                                } for m in messages if m['role'] != 'system']
         if return_json:
             anthropic_messages += [{"role": 'assistant',
                                     "content": [{"type": "text",
                                                  "text": "sure here's your json: {"}]
                                     }]
 
-        message = self.client.messages.create(
-            model=self.model_name,
-            max_tokens=self.model_params['max_tokens'],
-            temperature=self.model_params['temperature'],
-            system=self.system_message,
-            messages=anthropic_messages
-        )
+        try:
+            message = self.client.messages.create(
+                model=self.model_name,
+                max_tokens=self.model_params['max_tokens'],
+                temperature=self.model_params['temperature'],
+                system=self.system_message,
+                messages=anthropic_messages
+            )
+        except anthropic.InternalServerError as e:
+            raise OverloadedException(e)
 
         response = message.content[0].text
         if return_json:
             response = json.loads('{' + response)
         input_tokens = message.usage.input_tokens
         output_tokens = message.usage.output_tokens
         return response, input_tokens, output_tokens
```

### Comparing `justai-3.2.9/justai/models/gguf_models.py` & `justai-3.3.1/justai/models/gguf_models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,12 @@
-from llama_cpp import Llama
+try:
+    from llama_cpp import Llama
+except ImportError:
+    raise ImportError("If you want to use Llama models with justai run `pip install justai[llama]`")
+
 
 from justai.models.model import Model
 
 
 class GuffModel(Model):
 
     def __init__(self, model_name: str, params: dict):
```

### Comparing `justai-3.2.9/justai/models/model.py` & `justai-3.3.1/justai/models/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 from abc import ABC, abstractmethod
 
 
+class OverloadedException(Exception):
+    pass
+
+
 class Model(ABC):
 
     @abstractmethod
     def __init__(self, model_name: str, params: dict, system_message: str):
         """ Model implemention should create attributes for all supported parameters """
         self.model_name = model_name
         self.model_params = params # Specific parameters for specific models like temperature
```

### Comparing `justai-3.2.9/justai/models/modelfactory.py` & `justai-3.3.1/justai/models/modelfactory.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/models/openai_models.py` & `justai-3.3.1/justai/models/openai_models.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/tools/cache.py` & `justai-3.3.1/justai/tools/cache.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/tools/display.py` & `justai-3.3.1/justai/tools/display.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/tools/log.py` & `justai-3.3.1/justai/tools/log.py`

 * *Files 17% similar despite different names*

```diff
@@ -40,25 +40,34 @@
         self.conn = sqlite3.connect(self.log_path, check_same_thread=False)
         self.cursor = self.conn.cursor()
         self.cursor.execute('''CREATE TABLE IF NOT EXISTS log (
                                     timestamp DATETIME DEFAULT CURRENT_TIMESTAMP,
                                     title TEXT,
                                     value TEXT,
                                     logtype VARCHAR(10))''')
-        self.cursor.execute("DELETE FROM log WHERE timestamp < datetime('now', ? || ' hours')", (-log_retention_hours,))
-        self.conn.commit()
+        try:
+            self.cursor.execute("DELETE FROM log WHERE timestamp < datetime('now', ? || ' hours')", (-log_retention_hours,))
+        except sqlite3.OperationalError:
+            pass
+        try:
+            self.conn.commit()
+        except:
+            pass # Ignore errors when the log is closed
 
     def write(self, title, text, logtype='default'):
         if not isinstance(text, str):
             try:
                 text = json.dumps(text, indent=4)
             except Exception:
                 text = str(text)
         self.conn.execute('INSERT INTO log (title, value, logtype) VALUES (?, ?, ?)', (title, text, logtype))
-        self.conn.commit()
+        try:
+            self.conn.commit()
+        except:
+            pass # Ignore errors when the log is closed
         print('\n' + title)
         color_print(text, COLORS[logtype])
 
     def error(self, title, text):
         self.write(title, text, 'error')
 
     def info(self, title, text):
```

### Comparing `justai-3.2.9/justai/tools/prompts.py` & `justai-3.3.1/justai/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/translator/languages.py` & `justai-3.3.1/justai/translator/languages.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/translator/prompts.toml` & `justai-3.3.1/justai/translator/prompts.toml`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai/translator/translator.py` & `justai-3.3.1/justai/translator/translator.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,30 @@
 import os
 import hashlib
 import pickle
 import re
 from pathlib import Path
 from lxml import etree
+from enum import Enum
 
 from justai.agent.agent import Agent
 from justai.tools.log import Log
 from justai.tools.prompts import get_prompt, set_prompt_file
 from justai.translator.languages import LANGUAGES
 
 
+# Translation options
+class Opt(Enum):
+    REPLACE_VARIABLES = 'replace_variables'  # Vervang %variabelen% voor vertaling en zet ze daarna terug
+    LOG = 'log'
+    STRING_CACHED = 'string_cached'
+    CONCATENATED = 'concatenated'  # Of strings zijn samengevoegd met || om ze samen te vertalen
+    PROMPT = 'prompt'  # Om een eigen prompt mee te geven.
+
+
 class Translator(Agent):
 
     def __init__(self, model=None, **kwargs):
         if not model:
             model = os.environ.get('MODEL', 'claude-3-opus-20240229')
         super().__init__(model, temperature=0, max_tokens=4096, **kwargs)
         set_prompt_file(Path(__file__).parent / 'prompts.toml')
@@ -68,125 +78,158 @@
             translatable_from_source_element = [text for text in texts_from_source_element if is_translatable(text)]
             if translatable_from_source_element:
                 translatable.append("||".join(translatable_from_source_element))
         log.info('translate - all_texts', all_texts)
         log.info('translate - translatable_texts', translatable)
 
         # Vertaal de lijst van met || samengevoegde strings
-        flattened_all_texts = self.do_translate(translatable, language, string_cached=string_cached)
+        options = {Opt.STRING_CACHED: string_cached, Opt.LOG: True, Opt.CONCATENATED: True, Opt.REPLACE_VARIABLES: True}
+        translated = self.do_translate(translatable, language, options)
 
         # Zet nu de vertaalde delen terug in all_texts
-        index_in_translated_texts = 0
+        index_in_translated = 0
         for texts_from_source_element in all_texts:
             translatable_from_source_element = [text for text in texts_from_source_element if is_translatable(text)]
             if translatable_from_source_element:
-                translated_version = flattened_all_texts[index_in_translated_texts].split("||")
+                translated_version = translated[index_in_translated].split("||")
 
                 # Check
                 sc = len(translatable_from_source_element)
                 tc = len(translated_version)
                 if sc != tc:
                     log.error('translate - mismatch',
                               f'Source texts ({sc}) does not match number of translated texts ({tc})')
                     log.info('translate - translatable_from_source_element:', translatable_from_source_element)
                     log.info('translate - translated_version:', translated_version)
-                assert sc==tc, 'Mismatch see log'
+                assert sc == tc, 'Mismatch see log'
 
                 for index, text in enumerate(texts_from_source_element):
                     if is_translatable(text):
                         texts_from_source_element[index] = translated_version.pop(0)
-                index_in_translated_texts += 1
+                index_in_translated += 1
         flattened_all_texts = [item for sublist in all_texts for item in sublist]  # And flatten
 
         # Plaats vertaalde teksten in nieuwe <target> elementen met behoud van structuur
         counter = [0]
         for segment in root.xpath(f'.//ns:{segment_name}', namespaces=namespaces):
             source = segment.xpath('.//ns:source', namespaces=namespaces)[0]
             target = etree.SubElement(segment, f'{{urn:oasis:names:tc:xliff:document:{self.version}}}target')
             copy_structure_with_texts(source, target, flattened_all_texts, counter)
 
         updated_xml = etree.tostring(root, pretty_print=True, xml_declaration=True, encoding='UTF-8').decode('utf-8')
         return updated_xml
 
-    def do_translate(self, texts, language: str, string_cached=False):
-        log = self.logger
-
-        assert all(is_translatable(text) for text in texts), "Not all translatable"  # !! Tijdelijk
-        source_list = list(set(texts))
-        cache = StringCache(language) if string_cached else {}
-        source_list = [text for text in source_list if text not in cache]
+    def do_translate(self, texts, language: str, options: dict = {}):
+        # Options can be:
+        # REPLACE_VARIABLES: True | False
+        # LOG: True | False
+        # STRING_CACHED: True | False
+        # CONCATENATED: True | False
+
+        # assert all(is_translatable(text) for text in texts), "Not all translatable"  # !! Tijdelijk
+        cache = StringCache(language) if options.get(Opt.STRING_CACHED) else {}
+        source_list = [text for text in texts if text not in cache]
 
         if source_list:
             variables = []
             source_str_no_vars = ''
             for index, text in enumerate(source_list):
-                text_no_vars, v = replace_variables_with_hash(text)
-                variables.extend(v)
+                if options.get(Opt.REPLACE_VARIABLES):
+                    text_no_vars, v = replace_variables_with_hash(text)
+                    variables.extend(v)
+                else:
+                    text_no_vars = text
                 source_str_no_vars += f'{index + 1} [[{text_no_vars}]]\n'
-            prompt = get_prompt('TRANSLATE_MULTIPLE', language=language, translate_str=source_str_no_vars,
-                                count=len(source_list))
-            log.prompt('prompt', prompt)
-            target_str_no_vars = self.chat(prompt, return_json=False)
-            log.response('target_str_no_vars', target_str_no_vars)
-            target_str = replace_hash_with_variables(target_str_no_vars, variables)
-            log.info('do_translate - target_str', target_str)
+            given_prompt = options.get(Opt.PROMPT)
+            if given_prompt:
+                prompt = given_prompt.format(language=language, translate_str=source_str_no_vars,
+                                             count=len(source_list))
+            else:
+                prompt = get_prompt('TRANSLATE_MULTIPLE', language=language, translate_str=source_str_no_vars,
+                                    count=len(source_list))
+            target_str_no_vars = self.chat(prompt, return_json=False, cached=False)
+            if options.get(Opt.REPLACE_VARIABLES):
+                target_str = replace_hash_with_variables(target_str_no_vars, variables)
+            else:
+                target_str = target_str_no_vars
+            if options.get(Opt.LOG):
+                log = self.logger
+                log.response('target_str_no_vars', target_str_no_vars)
+                log.prompt('prompt', prompt)
+                log.info('do_translate - target_str', target_str)
 
             target_list = [t.split(']]')[0] for t in target_str.split('[[')[1:]]
-            translation_dict = dict(zip(source_list, target_list))
-            log.info('do_translate - translation_dict', translation_dict)
 
             count = 1
-            for source, translation in translation_dict.items():
+            for source, translation in zip(source_list, target_list):
 
-                source_parts = source.split('||')
-                translation_parts = translation.split('||')
-                log.info('do_translate - source_parts', source_parts)
-
-                # Check op het aantal onderdelen tussen ||. Dit moet gelijk zijn in de bron en de vertaling
-                sc = len(source_parts)
-                tc = len(translation_parts)
-                if tc != sc:
-                    log.warning('do_translate',
-                                f'Number of translated texts ({tc}) does not match number of source texts ({sc}). Correcting.')
-                    if tc < sc:
-                        translation_parts += [' '] * (sc - tc)
-                    else:
-                        # Dit is een hack! Het model geeft kennelijk meer ||'s terug in dan in het origineel.
-                        # Dat breekt de code verderop. Daarom voegen we de laatste onderdelen samen.
-                        # Maar dat levert wel een onjuiste vertaling op.
-                        translation_parts = translation_parts[:sc - 1] + [' '.join(translation_parts[sc - 1:])]
+                if options.get(Opt.CONCATENATED):
+                    source_parts = source.split('||')
+                    translation_parts = translation.split('||')
+                    # Check op het aantal onderdelen tussen ||. Dit moet gelijk zijn in de bron en de vertaling
                     sc = len(source_parts)
                     tc = len(translation_parts)
                     if tc != sc:
-                        log.error('do_translate',
-                                  f'Number of translated texts ({tc}) still does not match number of source texts ({sc}). Correcting.')
-                    assert (tc == sc), 'Mismatch in number of parts, see log for info'
+                        log.warning('do_translate',
+                                    f'Number of translated texts ({tc}) does not match number of source texts ({sc}). Correcting.')
+                        # Model krijgt het niet voor elkaar om een zin met evenveel delen terug te geven
+                        # We vertalen de stukjes los van elkaar.
+                        translation_parts = self.do_translate(source_parts, language, options)
+                        # if tc < sc:
+                        #     translation_parts += [' '] * (sc - tc)
+                        # else:
+                        #     # Dit is een hack! Het model geeft kennelijk meer ||'s terug in dan in het origineel.
+                        #     # Dat breekt de code verderop. Daarom voegen we de laatste onderdelen samen.
+                        #     # Maar dat levert wel een onjuiste vertaling op.
+                        #     translation_parts = translation_parts[:sc - 1] + [' '.join(translation_parts[sc - 1:])]
+                        sc = len(source_parts)
+                        tc = len(translation_parts)
+                        if tc != sc:
+                            log.error('do_translate',
+                                      f'Number of translated texts ({tc}) still does not match number of source texts ({sc}). Correcting.')
+                        assert (tc == sc), 'Mismatch in number of parts, see log for info'
+                else:
+                    source_parts = [source]
+                    translation_parts = [translation]
 
                 # Zorg dat de vertaling dezelfde whitespace aan het begin en eind heeft als de bron
                 for i, (source_part, translation_part) in enumerate(zip(source_parts, translation_parts)):
                     if source_part.strip() and (source_part[0] == ' ' or source_part[-1] == ' '):
                         start_spaces = (len(source_part) - len(source_part.lstrip(' '))) * ' '
                         end_spaces = (len(source_part) - len(source_part.rstrip(' '))) * ' '
                         translation_parts[i] = start_spaces + translation_part.strip() + end_spaces
-                log.info('do_translate - translation_parts', translation_parts)
-                translation = '||'.join(translation_parts)
+
+                target_list[count - 1] = '||'.join(translation_parts)
 
                 count += 1
-                ratio = len(source) / len(translation)
-                if ratio >= 1.5 or ratio <= 0.7:
-                    log.warning('', f'Vertaling van {source} naar {translation} is onverwacht lang of kort')
 
+                if options.get(Opt.LOG):
+                    ratio = len(source) / len(translation)
+                    if ratio >= 1.5 or ratio <= 0.7:
+                        log.warning('', f'Vertaling van {source} naar {translation} is onverwacht lang of kort')
+
+            translation_dict = dict(zip(source_list, target_list))
             cache.update(translation_dict)
-            if string_cached:
+            if options.get(Opt.STRING_CACHED):
                 cache.save()
 
         translations = [cache.get(text, text) for text in texts]
 
+        if options.get(Opt.CONCATENATED):
+            for s, t in zip(translations, texts):
+                sparts, tparts = s.split('||'), t.split('||')
+                if len(sparts) != len(tparts):
+                    assert False, f'Number of parts in source ({len(sparts)}) does not match number of parts in translation ({len(tparts)})'
+
         return translations
 
+    def translate_dict(self, text_dict, language: str, options):
+        return {k: v for k, v in zip(text_dict.keys(),
+                                     self.do_translate(list(text_dict.values()), language, options))}
+
 
 def replace_variables_with_hash(text):
     # Vindt alle variabelen in de tekst
     variables = re.findall(r'%[^%]+%', text)
     # Vervang alle variabelen in de tekst met ###
     # Het model heeft moeite met newlines. Daarom vervangen we ze door @@ en na vertaling weer terug.
     modified_text = re.sub(r'%[^%]+%', '###', text).replace('\n', '@@')
```

### Comparing `justai-3.2.9/justai/translator/xliff.py` & `justai-3.3.1/justai/translator/xliff.py`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/justai.egg-info/PKG-INFO` & `justai-3.3.1/justai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: justai
-Version: 3.2.9
+Version: 3.3.1
 Summary: Makes working with OpenAI's GPT API and other LLM's super easy
 Author-email: HP Harmsen <hp@harmsen.nl>
 License: This is free and unencumbered software released into the public domain.
         
         Anyone is free to copy, modify, publish, use, compile, sell, or
         distribute this software, either in source code form or as a compiled
         binary, for any purpose, commercial or non-commercial, and by any
@@ -39,29 +39,30 @@
 Requires-Dist: tenacity
 Requires-Dist: python-dateutil
 Requires-Dist: python-dotenv
 Requires-Dist: rich
 Requires-Dist: requests
 Requires-Dist: tiktoken
 Requires-Dist: lxml
-Requires-Dist: llama-cpp-python
 Requires-Dist: anthropic
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: build; extra == "dev"
 Requires-Dist: twine; extra == "dev"
 Requires-Dist: nox; extra == "dev"
+Provides-Extra: llama
+Requires-Dist: llama-cpp-python; extra == "llama"
 
 # JustAI
 
 Package to make working with Large Language models in Python super easy.
 
 Author: Hans-Peter Harmsen (hp@harmsen.nl) \
-Current version: 3.2.9
+Current version: 3.3.1
 
 ## Installation
 1. Install the package:
 ~~~~bash
 python -m pip install justai
 ~~~~
 2. Create an OpenAI acccount (for GPT3.5 / 4) [here](https://platform.openai.com/) or an Anthropic account [here](https://console.anthropic.com/)
```

### Comparing `justai-3.2.9/justai.egg-info/SOURCES.txt` & `justai-3.3.1/justai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `justai-3.2.9/pyproject.toml` & `justai-3.3.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [build-system]
 requires      = ["setuptools>=69", "wheel>=0.42"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "justai"
-version = "3.2.9"
+version = "3.3.1"
 description = "Makes working with OpenAI's GPT API and other LLM's super easy"
 readme = "README.md"
 authors = [{ name = "HP Harmsen", email = "hp@harmsen.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = ["ChatGPT", "GPT4", "GPT3.5", "api", "Claude", "Anthropic", "Lllama"]
+requires-python = ">=3.10"
+
+
 dependencies = [
     "openai",
     "tenacity",
     "python-dateutil",
     "python-dotenv",
     "rich",
     "requests",
     "tiktoken",
     "lxml",
-    "llama-cpp-python",
     "anthropic"
 ]
-requires-python = ">=3.10"
 
 [project.optional-dependencies]
 dev = ["black", "pytest", "build", "twine", "nox"]
+llama = ["llama-cpp-python"]
 
 [project.urls]
 Homepage = "https://github.com/hpharmsen/justai"
```

