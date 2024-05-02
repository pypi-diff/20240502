# Comparing `tmp/python-define-1.3.0.tar.gz` & `tmp/python_define-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-define-1.3.0.tar", last modified: Sun Sep  3 02:20:02 2023, max compression
+gzip compressed data, was "python_define-1.3.1.tar", last modified: Thu May  2 08:52:31 2024, max compression
```

## Comparing `python-define-1.3.0.tar` & `python_define-1.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-09-03 02:20:02.842222 python-define-1.3.0/
--rw-r--r--   0 grant     (1000) grant     (1000)    16725 2023-08-27 04:17:01.000000 python-define-1.3.0/LICENSE
--rw-r--r--   0 grant     (1000) grant     (1000)    24788 2023-09-03 02:20:02.842222 python-define-1.3.0/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python-define-1.3.0/README.md
--rwxr-xr-x   0 grant     (1000) grant     (1000)     5374 2023-09-03 02:17:57.000000 python-define-1.3.0/define.py
--rw-r--r--   0 grant     (1000) grant     (1000)      775 2023-09-03 02:18:59.000000 python-define-1.3.0/pyproject.toml
-drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2023-09-03 02:20:02.842222 python-define-1.3.0/python_define.egg-info/
--rw-r--r--   0 grant     (1000) grant     (1000)    24788 2023-09-03 02:20:02.000000 python-define-1.3.0/python_define.egg-info/PKG-INFO
--rw-r--r--   0 grant     (1000) grant     (1000)      266 2023-09-03 02:20:02.000000 python-define-1.3.0/python_define.egg-info/SOURCES.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        1 2023-09-03 02:20:02.000000 python-define-1.3.0/python_define.egg-info/dependency_links.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-09-03 02:20:02.000000 python-define-1.3.0/python_define.egg-info/entry_points.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       13 2023-09-03 02:20:02.000000 python-define-1.3.0/python_define.egg-info/requires.txt
--rw-r--r--   0 grant     (1000) grant     (1000)        7 2023-09-03 02:20:02.000000 python-define-1.3.0/python_define.egg-info/top_level.txt
--rw-r--r--   0 grant     (1000) grant     (1000)       38 2023-09-03 02:20:02.842222 python-define-1.3.0/setup.cfg
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2024-05-02 08:52:31.566506 python_define-1.3.1/
+-rw-r--r--   0 grant     (1000) grant     (1000)    16725 2023-08-27 04:17:01.000000 python_define-1.3.1/LICENSE
+-rw-r--r--   0 grant     (1000) grant     (1000)    24846 2024-05-02 08:52:31.566506 python_define-1.3.1/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)     4411 2023-08-07 01:18:14.000000 python_define-1.3.1/README.md
+-rwxr-xr-x   0 grant     (1000) grant     (1000)     5268 2024-05-02 08:37:28.000000 python_define-1.3.1/define.py
+-rw-r--r--   0 grant     (1000) grant     (1000)      790 2024-05-02 08:51:33.000000 python_define-1.3.1/pyproject.toml
+drwxr-xr-x   0 grant     (1000) grant     (1000)        0 2024-05-02 08:52:31.566506 python_define-1.3.1/python_define.egg-info/
+-rw-r--r--   0 grant     (1000) grant     (1000)    24846 2024-05-02 08:52:31.000000 python_define-1.3.1/python_define.egg-info/PKG-INFO
+-rw-r--r--   0 grant     (1000) grant     (1000)      266 2024-05-02 08:52:31.000000 python_define-1.3.1/python_define.egg-info/SOURCES.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        1 2024-05-02 08:52:31.000000 python_define-1.3.1/python_define.egg-info/dependency_links.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2024-05-02 08:52:31.000000 python_define-1.3.1/python_define.egg-info/entry_points.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       28 2024-05-02 08:52:31.000000 python_define-1.3.1/python_define.egg-info/requires.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)        8 2024-05-02 08:52:31.000000 python_define-1.3.1/python_define.egg-info/top_level.txt
+-rw-r--r--   0 grant     (1000) grant     (1000)       38 2024-05-02 08:52:31.566506 python_define-1.3.1/setup.cfg
```

### Comparing `python-define-1.3.0/LICENSE` & `python_define-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-define-1.3.0/PKG-INFO` & `python_define-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.3.0
+Version: 1.3.1
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
@@ -382,14 +382,16 @@
 Project-URL: Documentation, https://github.com/grantcarthew/python-define
 Project-URL: Repository, https://github.com/grantcarthew/python-define.git
 Project-URL: Changelog, https://github.com/grantcarthew/python-define/commits/main
 Keywords: define,openai,llm,english,linguistics,cli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Click~=8.1.7
+Requires-Dist: openai~=1.25.0
 
 # define
 
 An OpenAI-powered command-line linguistics assistant.
 
 If you're like me, you often feel unsure about the spelling of words, and sometimes even the definition of a word. Perhaps you're a programmer trying to come up with a name for that variable, function, data, or whatever else.
```

### Comparing `python-define-1.3.0/README.md` & `python_define-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `python-define-1.3.0/define.py` & `python_define-1.3.1/define.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,37 @@
 #!/usr/bin/env python
 
 from importlib.metadata import version
+from openai import OpenAI
 from typing import List, Dict
 import click
 import locale
-import openai
 import os
 import sys
 
+client = OpenAI(api_key=os.getenv('OPENAI_API_KEY'))
 
 def call_gpt_async(model: str, messages: List[Dict[str, str]], parameters: Dict[str, float]) -> Dict[str, str]:
     """Call the GPT model asynchronously and return the response."""
 
-    response = openai.ChatCompletion.create(
-        model=model,
-        messages=messages,
-        temperature=parameters['temperature'],
-        frequency_penalty=parameters['frequency_penalty'],
-        presence_penalty=parameters['presence_penalty'],
-        stream=True
-    )
+    stream = client.chat.completions.create(model=model,
+    messages=messages,
+    temperature=parameters['temperature'],
+    frequency_penalty=parameters['frequency_penalty'],
+    presence_penalty=parameters['presence_penalty'],
+    stream=True)
 
     try:
-        for chunk in response:
-            if 'content' in chunk['choices'][0]['delta']:
-                chunk_content = chunk['choices'][0]['delta']['content']
-                click.secho(chunk_content, fg='cyan', nl=False)
+        for chunk in stream:
+            click.secho(chunk.choices[0].delta.content or "", fg='cyan', nl=False)
         print()
     except KeyboardInterrupt:
         print()
     except Exception as err:
-        click.echo(f'[red]Error:[/] {err}')
+        click.echo(click.style(f'Error: {err}', fg='red'), err=True)
 
 
 def get_messages(user_content: str) -> List[Dict[str, str]]:
     """Prepare the list of messages for the GPT model."""
 
     locale_info = '_'.join(locale.getlocale())
 
@@ -179,16 +176,15 @@
 
 @click.command()
 @click.version_option(version('python-define'))
 @click.argument('query')
 def cli(query: str) -> None:
     """An OpenAI-powered command-line linguistics assistant."""
 
-    openai.api_key = os.getenv('OPENAI_API_KEY')
-    if not openai.api_key:
+    if not client.api_key:
         click.echo('Please set the OPENAI_API_KEY environment variable')
         sys.exit(1)
 
     model = 'gpt-3.5-turbo'
     parameters = {
         'temperature': 0,
         'frequency_penalty': 0,
```

### Comparing `python-define-1.3.0/pyproject.toml` & `python_define-1.3.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "python-define"
-version = "1.3.0"
+version = "1.3.1"
 description = "An OpenAI powered command-line linguistics assistant"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
 maintainers = [
   {name = "Grant Carthew", email = "grant@carthew.net"},
 ]
 keywords = ["define", "openai", "llm", "english", "linguistics", "cli"]
 dependencies = [
-  "Click",
-  "openai",
+  "Click~=8.1.7",
+  "openai~=1.25.0",
 ]
 
 [project.urls]
 Homepage = "https://github.com/grantcarthew/python-define"
 Documentation = "https://github.com/grantcarthew/python-define"
 Repository = "https://github.com/grantcarthew/python-define.git"
 Changelog = "https://github.com/grantcarthew/python-define/commits/main"
```

### Comparing `python-define-1.3.0/python_define.egg-info/PKG-INFO` & `python_define-1.3.1/python_define.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-define
-Version: 1.3.0
+Version: 1.3.1
 Summary: An OpenAI powered command-line linguistics assistant
 Author-email: Grant Carthew <grant@carthew.net>
 Maintainer-email: Grant Carthew <grant@carthew.net>
 License: Mozilla Public License Version 2.0
         ==================================
         
         1. Definitions
@@ -382,14 +382,16 @@
 Project-URL: Documentation, https://github.com/grantcarthew/python-define
 Project-URL: Repository, https://github.com/grantcarthew/python-define.git
 Project-URL: Changelog, https://github.com/grantcarthew/python-define/commits/main
 Keywords: define,openai,llm,english,linguistics,cli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: Click~=8.1.7
+Requires-Dist: openai~=1.25.0
 
 # define
 
 An OpenAI-powered command-line linguistics assistant.
 
 If you're like me, you often feel unsure about the spelling of words, and sometimes even the definition of a word. Perhaps you're a programmer trying to come up with a name for that variable, function, data, or whatever else.
```

