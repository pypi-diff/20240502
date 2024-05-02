# Comparing `tmp/quaero-1.1.4.tar.gz` & `tmp/quaero-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quaero-1.1.4.tar", last modified: Mon Apr  1 01:44:16 2024, max compression
+gzip compressed data, was "quaero-1.1.5.tar", last modified: Thu May  2 04:37:01 2024, max compression
```

## Comparing `quaero-1.1.4.tar` & `quaero-1.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gillian    (501) staff       (20)        0 2024-04-01 01:44:16.013071 quaero-1.1.4/
--rw-r--r--   0 gillian    (501) staff       (20)      950 2024-04-01 01:44:16.012873 quaero-1.1.4/PKG-INFO
--rw-r--r--   0 gillian    (501) staff       (20)      602 2024-04-01 01:43:56.000000 quaero-1.1.4/README.md
-drwxr-xr-x   0 gillian    (501) staff       (20)        0 2024-04-01 01:44:16.011688 quaero-1.1.4/quaero/
--rw-r--r--   0 gillian    (501) staff       (20)        0 2024-04-01 00:41:55.000000 quaero-1.1.4/quaero/__init__.py
--rw-r--r--   0 gillian    (501) staff       (20)      137 2024-04-01 00:41:55.000000 quaero-1.1.4/quaero/consts.py
--rwxr-xr-x   0 gillian    (501) staff       (20)     3129 2024-04-01 01:21:20.000000 quaero-1.1.4/quaero/index.py
--rw-r--r--   0 gillian    (501) staff       (20)     2418 2024-04-01 01:34:17.000000 quaero-1.1.4/quaero/openai.py
--rw-r--r--   0 gillian    (501) staff       (20)     1641 2024-04-01 01:17:46.000000 quaero-1.1.4/quaero/utils.py
-drwxr-xr-x   0 gillian    (501) staff       (20)        0 2024-04-01 01:44:16.012583 quaero-1.1.4/quaero.egg-info/
--rw-r--r--   0 gillian    (501) staff       (20)      950 2024-04-01 01:44:15.000000 quaero-1.1.4/quaero.egg-info/PKG-INFO
--rw-r--r--   0 gillian    (501) staff       (20)      285 2024-04-01 01:44:15.000000 quaero-1.1.4/quaero.egg-info/SOURCES.txt
--rw-r--r--   0 gillian    (501) staff       (20)        1 2024-04-01 01:44:15.000000 quaero-1.1.4/quaero.egg-info/dependency_links.txt
--rw-r--r--   0 gillian    (501) staff       (20)       45 2024-04-01 01:44:15.000000 quaero-1.1.4/quaero.egg-info/entry_points.txt
--rw-r--r--   0 gillian    (501) staff       (20)       31 2024-04-01 01:44:15.000000 quaero-1.1.4/quaero.egg-info/requires.txt
--rw-r--r--   0 gillian    (501) staff       (20)        7 2024-04-01 01:44:15.000000 quaero-1.1.4/quaero.egg-info/top_level.txt
--rw-r--r--   0 gillian    (501) staff       (20)       38 2024-04-01 01:44:16.013112 quaero-1.1.4/setup.cfg
--rw-r--r--   0 gillian    (501) staff       (20)      712 2024-04-01 01:44:08.000000 quaero-1.1.4/setup.py
+drwxr-xr-x   0 gillian    (501) staff       (20)        0 2024-05-02 04:37:01.614369 quaero-1.1.5/
+-rw-r--r--   0 gillian    (501) staff       (20)      950 2024-05-02 04:37:01.614160 quaero-1.1.5/PKG-INFO
+-rw-r--r--   0 gillian    (501) staff       (20)      602 2024-04-01 01:43:56.000000 quaero-1.1.5/README.md
+drwxr-xr-x   0 gillian    (501) staff       (20)        0 2024-05-02 04:37:01.613172 quaero-1.1.5/quaero/
+-rw-r--r--   0 gillian    (501) staff       (20)        0 2024-04-01 00:41:55.000000 quaero-1.1.5/quaero/__init__.py
+-rw-r--r--   0 gillian    (501) staff       (20)      137 2024-04-01 00:41:55.000000 quaero-1.1.5/quaero/consts.py
+-rwxr-xr-x   0 gillian    (501) staff       (20)     3732 2024-05-02 04:19:59.000000 quaero-1.1.5/quaero/index.py
+-rw-r--r--   0 gillian    (501) staff       (20)     2415 2024-05-02 04:15:22.000000 quaero-1.1.5/quaero/openai.py
+-rw-r--r--   0 gillian    (501) staff       (20)     1641 2024-04-01 01:17:46.000000 quaero-1.1.5/quaero/utils.py
+drwxr-xr-x   0 gillian    (501) staff       (20)        0 2024-05-02 04:37:01.613872 quaero-1.1.5/quaero.egg-info/
+-rw-r--r--   0 gillian    (501) staff       (20)      950 2024-05-02 04:37:01.000000 quaero-1.1.5/quaero.egg-info/PKG-INFO
+-rw-r--r--   0 gillian    (501) staff       (20)      285 2024-05-02 04:37:01.000000 quaero-1.1.5/quaero.egg-info/SOURCES.txt
+-rw-r--r--   0 gillian    (501) staff       (20)        1 2024-05-02 04:37:01.000000 quaero-1.1.5/quaero.egg-info/dependency_links.txt
+-rw-r--r--   0 gillian    (501) staff       (20)       45 2024-05-02 04:37:01.000000 quaero-1.1.5/quaero.egg-info/entry_points.txt
+-rw-r--r--   0 gillian    (501) staff       (20)       31 2024-05-02 04:37:01.000000 quaero-1.1.5/quaero.egg-info/requires.txt
+-rw-r--r--   0 gillian    (501) staff       (20)        7 2024-05-02 04:37:01.000000 quaero-1.1.5/quaero.egg-info/top_level.txt
+-rw-r--r--   0 gillian    (501) staff       (20)       38 2024-05-02 04:37:01.614410 quaero-1.1.5/setup.cfg
+-rw-r--r--   0 gillian    (501) staff       (20)      712 2024-05-02 04:20:37.000000 quaero-1.1.5/setup.py
```

### Comparing `quaero-1.1.4/PKG-INFO` & `quaero-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quaero
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simple CLI tool for asking ChatGPT questions in the CLI
 Home-page: https://github.com/yeo-yeo/chatgpt-cli-python
 Author: Gillian Yeomans
 Author-email: hello@gillian.codes
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: colorama
```

### Comparing `quaero-1.1.4/README.md` & `quaero-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `quaero-1.1.4/quaero/index.py` & `quaero-1.1.5/quaero/index.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,16 @@
 
 from quaero.openai import fetch_data
 from quaero.utils import print_waiting, save_to_file, check_for_config
 from quaero.consts import app_directory, api_key_key, config_path
 
 async def main_impl():
     conversation = {}
+    model = 'gpt-3.5-turbo'
+
     
     # Handler for ?? (ctrl + c)
     def quit_handler(sig, frame):
         print("\nExiting script...")
         id = save_to_file(conversation)
         if id:
             print("Conversation ID: ", id)
@@ -29,14 +31,17 @@
     parser = argparse.ArgumentParser(description="🤖 ChatGPT CLI")
     parser.add_argument(
         "command", choices=["init"], help="Set up your OpenAI credentials", nargs="?"
     )
     parser.add_argument(
         "-c", "--conversation", help="Use with the ID printed at the end of a previous conversation to resume that same conversation.  Will not work if the conversation has been deleted.", nargs=1
     )
+    parser.add_argument(
+        "-m", "--model", help="Specify which model to use. Options are -m 3: gpt-3.5-turbo and -m 4: gpt-4-turbo-preview.  Will default to gpt-3.5-turbo unless -m 4 is passed.", nargs=1
+    )
     args = parser.parse_args()
 
     # Handle init setup
     if args.command == "init":
         print(
             Fore.YELLOW + "Welcome to quaero! To get started you will need to generate an OpenAI API key and paste it here to save it to your quaero config.\n\nVisit " + Fore.WHITE + "https://platform.openai.com/api-keys." + Fore.YELLOW + "\n\nThe key should be like sk-{20chars}\n" + Style.RESET_ALL
         )
@@ -60,27 +65,37 @@
         conversation_path = os.path.join(app_directory, d, t)
         if not os.path.isfile(conversation_path):
             print(Fore.RED + "That conversation ID was not found" + Style.RESET_ALL)
             sys.exit(1)
         with open(conversation_path) as file:
             conversation = json.load(file)
 
+    if args.model:
+        model_arg = args.model[0]
+        if model_arg == '4':
+            model = 'gpt-4-turbo-preview'
+        elif model_arg == '3':
+            # already set as the default
+            pass
+        else:
+            raise Exception('Unrecognised model input.  Options are 3 for 3.5-turbo (default) or 4 for 4-turbo-preview.')
+
     while True:
         fetched_data_flag = asyncio.Event()
 
         # Prompt user for their question
         user_input = input("> ")
 
         # Store their question in the conversation dictionary
         conversation[time.time()] = {'content': user_input, 'role': 'user'}
 
         # Simultaneous kick off the API request and printing the waiting message
         # The fetch_data function also writes the response to the conversation dictionary
         await asyncio.gather(
-            fetch_data(conversation, fetched_data_flag), print_waiting(fetched_data_flag)
+            fetch_data(conversation, model, fetched_data_flag), print_waiting(fetched_data_flag)
         )
 
         print("\n")
 
 
 def main():
     # Asyncio lib needed so the data request and wait message can happen simultaneously (requests lib is blocking)
```

### Comparing `quaero-1.1.4/quaero/openai.py` & `quaero-1.1.5/quaero/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import json
 import aiohttp
 from quaero.utils import get_api_key
 from colorama import Style
 import time
 
 # Fn to call the bot and print its response as it streams in
-async def fetch_data(conversation, fetched_data_flag):
+async def fetch_data(conversation, model, fetched_data_flag):
     api_key = get_api_key()
     headers = {"Authorization": f"Bearer {api_key}", "content-type": "application/json"}
     url = f"https://api.openai.com/v1/chat/completions"
     payload = {
-        "model": "gpt-3.5-turbo",
+        "model": model,
         "messages": [value for value in conversation.values()],
         "temperature": 0.7,
         "stream": True,
     }
 
     try:
         async with aiohttp.ClientSession() as session:
```

### Comparing `quaero-1.1.4/quaero/utils.py` & `quaero-1.1.5/quaero/utils.py`

 * *Files identical despite different names*

### Comparing `quaero-1.1.4/quaero.egg-info/PKG-INFO` & `quaero-1.1.5/quaero.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quaero
-Version: 1.1.4
+Version: 1.1.5
 Summary: Simple CLI tool for asking ChatGPT questions in the CLI
 Home-page: https://github.com/yeo-yeo/chatgpt-cli-python
 Author: Gillian Yeomans
 Author-email: hello@gillian.codes
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: colorama
```

### Comparing `quaero-1.1.4/setup.py` & `quaero-1.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="quaero",
-    version="1.1.4",
+    version="1.1.5",
     description="Simple CLI tool for asking ChatGPT questions in the CLI",
     long_description=long_description,
     long_description_content_type='text/markdown',
     author="Gillian Yeomans",
     author_email="hello@gillian.codes",
     url="https://github.com/yeo-yeo/chatgpt-cli-python",
     packages=find_packages(),
```

