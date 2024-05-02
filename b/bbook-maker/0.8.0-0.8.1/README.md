# Comparing `tmp/bbook_maker-0.8.0.tar.gz` & `tmp/bbook_maker-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bbook_maker-0.8.0.tar", last modified: Thu Apr  4 13:03:26 2024, max compression
+gzip compressed data, was "bbook_maker-0.8.1.tar", last modified: Thu Apr  4 13:37:07 2024, max compression
```

## Comparing `bbook_maker-0.8.0.tar` & `bbook_maker-0.8.1.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.480922 bbook_maker-0.8.0/
--rw-r--r--   0 hyi        (502) staff       (20)     1063 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/LICENSE
--rw-r--r--   0 hyi        (502) staff       (20)      825 2024-04-04 13:03:26.480493 bbook_maker-0.8.0/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)    13423 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/README.md
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.479889 bbook_maker-0.8.0/bbook_maker.egg-info/
--rw-r--r--   0 hyi        (502) staff       (20)      825 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/PKG-INFO
--rw-r--r--   0 hyi        (502) staff       (20)     1083 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/SOURCES.txt
--rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/dependency_links.txt
--rw-r--r--   0 hyi        (502) staff       (20)       52 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/entry_points.txt
--rw-r--r--   0 hyi        (502) staff       (20)      111 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/requires.txt
--rw-r--r--   0 hyi        (502) staff       (20)       11 2024-04-04 13:03:26.000000 bbook_maker-0.8.0/bbook_maker.egg-info/top_level.txt
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.454918 bbook_maker-0.8.0/book_maker/
--rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/book_maker/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)       60 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/book_maker/__main__.py
--rw-r--r--   0 hyi        (502) staff       (20)    15333 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/book_maker/cli.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.463526 bbook_maker-0.8.0/book_maker/loader/
--rw-r--r--   0 hyi        (502) staff       (20)      296 2023-12-26 08:27:25.000000 bbook_maker-0.8.0/book_maker/loader/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      491 2023-03-30 08:48:21.000000 bbook_maker-0.8.0/book_maker/loader/base_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)    20061 2024-01-27 14:28:19.000000 bbook_maker-0.8.0/book_maker/loader/epub_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     3641 2024-02-29 03:05:11.000000 bbook_maker-0.8.0/book_maker/loader/helper.py
--rw-r--r--   0 hyi        (502) staff       (20)    10383 2024-01-27 14:28:19.000000 bbook_maker-0.8.0/book_maker/loader/srt_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)     4558 2023-07-30 13:14:07.000000 bbook_maker-0.8.0/book_maker/loader/txt_loader.py
--rw-r--r--   0 hyi        (502) staff       (20)    30290 2023-03-30 11:26:33.000000 bbook_maker-0.8.0/book_maker/obok.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.478262 bbook_maker-0.8.0/book_maker/translator/
--rw-r--r--   0 hyi        (502) staff       (20)      895 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/book_maker/translator/__init__.py
--rw-r--r--   0 hyi        (502) staff       (20)      391 2023-04-03 11:56:33.000000 bbook_maker-0.8.0/book_maker/translator/base_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2115 2023-05-28 12:22:19.000000 bbook_maker-0.8.0/book_maker/translator/caiyun_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)    10874 2024-04-04 13:03:01.000000 bbook_maker-0.8.0/book_maker/translator/chatgptapi_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     1649 2023-05-21 11:18:16.000000 bbook_maker-0.8.0/book_maker/translator/claude_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)      846 2024-01-05 14:10:29.000000 bbook_maker-0.8.0/book_maker/translator/custom_api_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     1525 2023-05-15 00:32:18.000000 bbook_maker-0.8.0/book_maker/translator/deepl_free_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2227 2024-01-31 02:15:04.000000 bbook_maker-0.8.0/book_maker/translator/deepl_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2810 2024-01-27 14:17:37.000000 bbook_maker-0.8.0/book_maker/translator/gemini_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     1843 2023-05-24 01:29:57.000000 bbook_maker-0.8.0/book_maker/translator/google_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2472 2023-11-26 14:01:12.000000 bbook_maker-0.8.0/book_maker/translator/litellm_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     2839 2024-02-29 03:05:11.000000 bbook_maker-0.8.0/book_maker/translator/tencent_transmart_translator.py
--rw-r--r--   0 hyi        (502) staff       (20)     4246 2023-03-30 08:35:07.000000 bbook_maker-0.8.0/book_maker/utils.py
--rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-04 13:03:26.480992 bbook_maker-0.8.0/setup.cfg
--rw-r--r--   0 hyi        (502) staff       (20)     1000 2024-04-04 13:03:18.000000 bbook_maker-0.8.0/setup.py
-drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:03:26.478969 bbook_maker-0.8.0/tests/
--rw-r--r--   0 hyi        (502) staff       (20)     9507 2023-08-23 02:01:55.000000 bbook_maker-0.8.0/tests/test_integration.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:37:07.912221 bbook_maker-0.8.1/
+-rw-r--r--   0 hyi        (502) staff       (20)     1063 2023-03-30 08:35:07.000000 bbook_maker-0.8.1/LICENSE
+-rw-r--r--   0 hyi        (502) staff       (20)      850 2024-04-04 13:37:07.911857 bbook_maker-0.8.1/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)    13660 2024-04-04 13:11:44.000000 bbook_maker-0.8.1/README.md
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:37:07.911269 bbook_maker-0.8.1/bbook_maker.egg-info/
+-rw-r--r--   0 hyi        (502) staff       (20)      850 2024-04-04 13:37:07.000000 bbook_maker-0.8.1/bbook_maker.egg-info/PKG-INFO
+-rw-r--r--   0 hyi        (502) staff       (20)     1083 2024-04-04 13:37:07.000000 bbook_maker-0.8.1/bbook_maker.egg-info/SOURCES.txt
+-rw-r--r--   0 hyi        (502) staff       (20)        1 2024-04-04 13:37:07.000000 bbook_maker-0.8.1/bbook_maker.egg-info/dependency_links.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       52 2024-04-04 13:37:07.000000 bbook_maker-0.8.1/bbook_maker.egg-info/entry_points.txt
+-rw-r--r--   0 hyi        (502) staff       (20)      121 2024-04-04 13:37:07.000000 bbook_maker-0.8.1/bbook_maker.egg-info/requires.txt
+-rw-r--r--   0 hyi        (502) staff       (20)       11 2024-04-04 13:37:07.000000 bbook_maker-0.8.1/bbook_maker.egg-info/top_level.txt
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:37:07.885695 bbook_maker-0.8.1/book_maker/
+-rw-r--r--   0 hyi        (502) staff       (20)        0 2023-03-30 08:35:07.000000 bbook_maker-0.8.1/book_maker/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)       60 2023-03-30 08:35:07.000000 bbook_maker-0.8.1/book_maker/__main__.py
+-rw-r--r--   0 hyi        (502) staff       (20)    15333 2024-04-04 13:03:01.000000 bbook_maker-0.8.1/book_maker/cli.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:37:07.894744 bbook_maker-0.8.1/book_maker/loader/
+-rw-r--r--   0 hyi        (502) staff       (20)      296 2023-12-26 08:27:25.000000 bbook_maker-0.8.1/book_maker/loader/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      491 2023-03-30 08:48:21.000000 bbook_maker-0.8.1/book_maker/loader/base_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)    20061 2024-01-27 14:28:19.000000 bbook_maker-0.8.1/book_maker/loader/epub_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     3641 2024-02-29 03:05:11.000000 bbook_maker-0.8.1/book_maker/loader/helper.py
+-rw-r--r--   0 hyi        (502) staff       (20)    10383 2024-01-27 14:28:19.000000 bbook_maker-0.8.1/book_maker/loader/srt_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4558 2023-07-30 13:14:07.000000 bbook_maker-0.8.1/book_maker/loader/txt_loader.py
+-rw-r--r--   0 hyi        (502) staff       (20)    30290 2023-03-30 11:26:33.000000 bbook_maker-0.8.1/book_maker/obok.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:37:07.910265 bbook_maker-0.8.1/book_maker/translator/
+-rw-r--r--   0 hyi        (502) staff       (20)      895 2024-04-04 13:03:01.000000 bbook_maker-0.8.1/book_maker/translator/__init__.py
+-rw-r--r--   0 hyi        (502) staff       (20)      391 2023-04-03 11:56:33.000000 bbook_maker-0.8.1/book_maker/translator/base_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2115 2023-05-28 12:22:19.000000 bbook_maker-0.8.1/book_maker/translator/caiyun_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)    10874 2024-04-04 13:03:01.000000 bbook_maker-0.8.1/book_maker/translator/chatgptapi_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1445 2024-04-04 13:36:48.000000 bbook_maker-0.8.1/book_maker/translator/claude_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)      846 2024-01-05 14:10:29.000000 bbook_maker-0.8.1/book_maker/translator/custom_api_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1525 2023-05-15 00:32:18.000000 bbook_maker-0.8.1/book_maker/translator/deepl_free_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2227 2024-01-31 02:15:04.000000 bbook_maker-0.8.1/book_maker/translator/deepl_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2810 2024-01-27 14:17:37.000000 bbook_maker-0.8.1/book_maker/translator/gemini_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     1843 2023-05-24 01:29:57.000000 bbook_maker-0.8.1/book_maker/translator/google_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2472 2023-11-26 14:01:12.000000 bbook_maker-0.8.1/book_maker/translator/litellm_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     2839 2024-02-29 03:05:11.000000 bbook_maker-0.8.1/book_maker/translator/tencent_transmart_translator.py
+-rw-r--r--   0 hyi        (502) staff       (20)     4246 2023-03-30 08:35:07.000000 bbook_maker-0.8.1/book_maker/utils.py
+-rw-r--r--   0 hyi        (502) staff       (20)       38 2024-04-04 13:37:07.912272 bbook_maker-0.8.1/setup.cfg
+-rw-r--r--   0 hyi        (502) staff       (20)     1017 2024-04-04 13:37:01.000000 bbook_maker-0.8.1/setup.py
+drwxr-xr-x   0 hyi        (502) staff       (20)        0 2024-04-04 13:37:07.910637 bbook_maker-0.8.1/tests/
+-rw-r--r--   0 hyi        (502) staff       (20)     9507 2023-08-23 02:01:55.000000 bbook_maker-0.8.1/tests/test_integration.py
```

### Comparing `bbook_maker-0.8.0/LICENSE` & `bbook_maker-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/PKG-INFO` & `bbook_maker-0.8.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbook_maker
-Version: 0.8.0
+Version: 0.8.1
 Summary: The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.
 Home-page: https://github.com/yihong0618/bilingual_book_maker
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,7 +19,8 @@
 Requires-Dist: rich
 Requires-Dist: tqdm
 Requires-Dist: tiktoken
 Requires-Dist: PyDeepLX
 Requires-Dist: google-generativeai
 Requires-Dist: langdetect
 Requires-Dist: backoff
+Requires-Dist: anthropic
```

### Comparing `bbook_maker-0.8.0/README.md` & `bbook_maker-0.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -83,14 +83,17 @@
 
 # Use the GPT-4 model with context to Japanese
 python3 make_book.py --book_name test_books/animal_farm.epub --model gpt4 --use_context --language ja
 
 # Use a specific OpenAI model alias
 python3 make_book.py --book_name test_books/animal_farm.epub --model openai --model_list gpt-4-1106-preview --openai_key ${openai_key}
 
+**Note** you can use other `openai like` model in this way
+python3 make_book.py --book_name test_books/animal_farm.epub --model openai --model_list yi-34b-chat-0205 --openai_key ${openai_key} --api_base "https://api.lingyiwanwu.com/v1"
+
 # Use a specific list of OpenAI model aliases
 python3 make_book.py --book_name test_books/animal_farm.epub --model openai --model_list gpt-4-1106-preview,gpt-4-0125-preview,gpt-3.5-turbo-0125 --openai_key ${openai_key}
 
 # Use the DeepL model with Japanese
 python3 make_book.py --book_name test_books/animal_farm.epub --model deepl --deepl_key ${deepl_key} --language ja
 
 # Use the Claude model with Japanese
```

### Comparing `bbook_maker-0.8.0/bbook_maker.egg-info/PKG-INFO` & `bbook_maker-0.8.1/bbook_maker.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bbook_maker
-Version: 0.8.0
+Version: 0.8.1
 Summary: The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.
 Home-page: https://github.com/yihong0618/bilingual_book_maker
 Author: yihong0618
 Author-email: zouzou0208@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -19,7 +19,8 @@
 Requires-Dist: rich
 Requires-Dist: tqdm
 Requires-Dist: tiktoken
 Requires-Dist: PyDeepLX
 Requires-Dist: google-generativeai
 Requires-Dist: langdetect
 Requires-Dist: backoff
+Requires-Dist: anthropic
```

### Comparing `bbook_maker-0.8.0/bbook_maker.egg-info/SOURCES.txt` & `bbook_maker-0.8.1/bbook_maker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/cli.py` & `bbook_maker-0.8.1/book_maker/cli.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/loader/epub_loader.py` & `bbook_maker-0.8.1/book_maker/loader/epub_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/loader/helper.py` & `bbook_maker-0.8.1/book_maker/loader/helper.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/loader/srt_loader.py` & `bbook_maker-0.8.1/book_maker/loader/srt_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/loader/txt_loader.py` & `bbook_maker-0.8.1/book_maker/loader/txt_loader.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/obok.py` & `bbook_maker-0.8.1/book_maker/obok.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/__init__.py` & `bbook_maker-0.8.1/book_maker/translator/__init__.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/caiyun_translator.py` & `bbook_maker-0.8.1/book_maker/translator/caiyun_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/chatgptapi_translator.py` & `bbook_maker-0.8.1/book_maker/translator/chatgptapi_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/claude_translator.py` & `bbook_maker-0.8.1/book_maker/translator/claude_translator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import re
-import requests
+import time
 from rich import print
+from anthropic import Anthropic
 
 from .base_translator import Base
 
 
 class Claude(Base):
     def __init__(
         self,
@@ -12,47 +13,38 @@
         language,
         api_base=None,
         prompt_template=None,
         temperature=1.0,
         **kwargs,
     ) -> None:
         super().__init__(key, language)
-        self.api_url = (
-            f"{api_base}v1/complete"
-            if api_base
-            else "https://api.anthropic.com/v1/complete"
-        )
-        self.headers = {
-            "Content-Type": "application/json",
-            "x-api-key": key,
-        }
-        self.data = {
-            "prompt": "",
-            "model": "claude-v1.3",
-            "max_tokens_to_sample": 1024,
-            "temperature": temperature,
-            "stop_sequences": ["\n\nHuman:"],
-        }
-        self.session = requests.session()
+        self.api_url = f"{api_base}" if api_base else "https://api.anthropic.com"
+        self.client = Anthropic(base_url=api_base, api_key=key, timeout=20)
+
         self.language = language
         self.prompt_template = (
             prompt_template
             or "\n\nHuman: Help me translate the text within triple backticks into {language} and provide only the translated result.\n```{text}```\n\nAssistant: "
         )
 
     def rotate_key(self):
         pass
 
     def translate(self, text):
         print(text)
         self.rotate_key()
-        self.data["prompt"] = self.prompt_template.format(
+        prompt = self.prompt_template.format(
             text=text,
             language=self.language,
         )
-        r = self.session.post(self.api_url, headers=self.headers, json=self.data)
-        if not r.ok:
-            return text
-        t_text = r.json().get("completion").strip()
+        message = [{"role": "user", "content": prompt}]
+        r = self.client.messages.create(
+            max_tokens=4096,
+            messages=message,
+            model="claude-3-haiku-20240307",  # default it for now
+        )
+        t_text = r.content[0].text
+        # api limit rate and spider rule
+        time.sleep(1)
 
         print("[bold green]" + re.sub("\n{3,}", "\n\n", t_text) + "[/bold green]")
         return t_text
```

### Comparing `bbook_maker-0.8.0/book_maker/translator/custom_api_translator.py` & `bbook_maker-0.8.1/book_maker/translator/custom_api_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/deepl_free_translator.py` & `bbook_maker-0.8.1/book_maker/translator/deepl_free_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/deepl_translator.py` & `bbook_maker-0.8.1/book_maker/translator/deepl_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/gemini_translator.py` & `bbook_maker-0.8.1/book_maker/translator/gemini_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/google_translator.py` & `bbook_maker-0.8.1/book_maker/translator/google_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/litellm_translator.py` & `bbook_maker-0.8.1/book_maker/translator/litellm_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/translator/tencent_transmart_translator.py` & `bbook_maker-0.8.1/book_maker/translator/tencent_transmart_translator.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/book_maker/utils.py` & `bbook_maker-0.8.1/book_maker/utils.py`

 * *Files identical despite different names*

### Comparing `bbook_maker-0.8.0/setup.py` & `bbook_maker-0.8.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,21 +10,22 @@
     "rich",
     "tqdm",
     "tiktoken",
     "PyDeepLX",
     "google-generativeai",
     "langdetect",
     "backoff",
+    "anthropic",
 ]
 
 
 setup(
     name="bbook_maker",
     description="The bilingual_book_maker is an AI translation tool that uses ChatGPT to assist users in creating multi-language versions of epub/txt files and books.",
-    version="0.8.0",
+    version="0.8.1",
     license="MIT",
     author="yihong0618",
     author_email="zouzou0208@gmail.com",
     packages=find_packages(),
     url="https://github.com/yihong0618/bilingual_book_maker",
     python_requires=">=3.8",
     install_requires=packages,
```

### Comparing `bbook_maker-0.8.0/tests/test_integration.py` & `bbook_maker-0.8.1/tests/test_integration.py`

 * *Files identical despite different names*

