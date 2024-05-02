# Comparing `tmp/cria-1.6.2.tar.gz` & `tmp/cria-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cria-1.6.2.tar", max compression
+gzip compressed data, was "cria-1.6.5.tar", max compression
```

## Comparing `cria-1.6.2.tar` & `cria-1.6.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2024-04-29 15:24:13.797190 cria-1.6.2/LICENSE.md
--rw-r--r--   0        0        0     8790 2024-04-29 15:24:13.797190 cria-1.6.2/README.md
--rw-r--r--   0        0        0      824 2024-04-29 15:24:13.797190 cria-1.6.2/pyproject.toml
--rw-r--r--   0        0        0     9555 2024-04-29 15:24:13.797190 cria-1.6.2/src/cria.py
--rw-r--r--   0        0        0     9429 1970-01-01 00:00:00.000000 cria-1.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-02 16:14:04.015252 cria-1.6.5/LICENSE.md
+-rw-r--r--   0        0        0    10426 2024-05-02 16:14:04.015252 cria-1.6.5/README.md
+-rw-r--r--   0        0        0      824 2024-05-02 16:14:04.015252 cria-1.6.5/pyproject.toml
+-rw-r--r--   0        0        0    10530 2024-05-02 16:14:04.015252 cria-1.6.5/src/cria.py
+-rw-r--r--   0        0        0    11065 1970-01-01 00:00:00.000000 cria-1.6.5/PKG-INFO
```

### Comparing `cria-1.6.2/LICENSE.md` & `cria-1.6.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cria-1.6.2/README.md` & `cria-1.6.5/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -28,14 +28,17 @@
   - [Custom Models](#custom-models)
   - [Streams](#streams)
   - [Closing](#closing)
   - [Message History](#message-history)
     - [Follow-Up](#follow-up)
     - [Clear Message History](#clear-message-history)
     - [Passing In Custom Context](#passing-in-custom-context)
+  - [Interrupting](#interrupting)
+    - [With Message History](#with-message-history)
+    - [Without Message History](#without-message-history)
   - [Multiple Models and Parallel Conversations](#multiple-models-and-parallel-conversations)
     - [Models](#models)
     - [With](#with-model)
     - [Standalone](#standalone-model)
   - [Running Standalone](#running-standalone)
 - [Contributing](#contributing)
 - [License](#license)
@@ -49,27 +52,30 @@
 
 ai = cria.Cria()
 
 prompt = "Who is the CEO of OpenAI?"
 for chunk in ai.chat(prompt):
     print(chunk, end="")
 ```
+
 ```
 >>> The CEO of OpenAI is Sam Altman!
 ```
+
 or, you can run this more configurable example.
 
 ```python
 import cria
 
 with cria.Model() as ai:
   prompt = "Who is the CEO of OpenAI?"
   response = ai.chat(prompt, stream=False)
   print(response)
 ```
+
 ```
 >>> The CEO of OpenAI is Sam Altman!
 ```
 
 If no model is configured, Cria runs the default model: `llama3:8b`. If the default model is not installed on your machine, Cria will install it automatically.
 
 **Important**: `llama3:8b` is about **4.7GB**, and will likely take a while to download.
@@ -190,14 +196,72 @@
 
 - `user` - Pass prompts as the user.
 - `system` - Give instructions as the system.
 - `assistant` - Act as the AI assistant yourself, and give the LLM lines.
 
 The prompt parameter will always be appended to messages under the `user` role, to override this, you can choose to pass in nothing for `prompt`.
 
+### Interrupting
+
+#### With Message History
+
+If you are streaming messages with Cria, you can interrupt the prompt mid way.
+
+```python
+response = ""
+max_token_length = 5
+
+prompt = "Who is the CEO of OpenAI?"
+for i, chunk in enumerate(ai.chat(prompt)):
+
+  if i >= max_token_length:
+    ai.stop()
+
+  print(chunk, end="") # The CEO of OpenAI is
+```
+
+```python
+response = ""
+max_token_length = 5
+
+prompt = "Who is the CEO of OpenAI?"
+for i, chunk in enumerate(ai.generate(prompt)):
+
+  if i >= max_token_length:
+    ai.stop()
+
+  print(chunk, end="") # The CEO of OpenAI is
+```
+
+In the examples, after the AI generates five tokens (units of text that are usually a couple of characters long), text generation is stopped via the `stop` method. After `stop` is called, you can safely `break` out of the `for` loop.
+
+#### Without Message History
+
+By default, Cria automatically saves responses in message history, even if the stream is interrupted. To prevent this behaviour though, you can pass in the `allow_interruption` boolean.
+
+```python
+ai = cria.Cria(allow_interruption=False)
+
+response = ""
+max_token_length = 5
+
+prompt = "Who is the CEO of OpenAI?"
+for i, chunk in enumerate(ai.chat(prompt)):
+
+  if i >= max_token_length:
+    ai.stop()
+    break
+
+  print(chunk, end="") # The CEO of OpenAI is
+
+prompt = "Tell me more about him."
+for chunk in ai.chat(prompt):
+  print(chunk, end="") # I apologize, but I don't have any information about "him" because the conversation just started...
+```
+
 ### Multiple Models and Parallel Conversations
 
 #### Models
 
 If you are running multiple models or parallel conversations, the `Model` class is also available. This is recommended for most use cases.
 
 ```python
```

#### html2text {}

```diff
@@ -7,17 +7,19 @@
 less code to save time and avoid duplication. - **Efficient**: Use advanced
 features with your own `ollama` instance, or a subprocess. ## Guide - [Quick
 Start](#quickstart) - [Installation](#installation) - [Windows](#windows) -
 [Mac](#mac) - [Linux](#linux) - [Advanced Usage](#advanced-usage) - [Custom
 Models](#custom-models) - [Streams](#streams) - [Closing](#closing) - [Message
 History](#message-history) - [Follow-Up](#follow-up) - [Clear Message History]
 (#clear-message-history) - [Passing In Custom Context](#passing-in-custom-
-context) - [Multiple Models and Parallel Conversations](#multiple-models-and-
-parallel-conversations) - [Models](#models) - [With](#with-model) -
-[Standalone](#standalone-model) - [Running Standalone](#running-standalone) -
+context) - [Interrupting](#interrupting) - [With Message History](#with-
+message-history) - [Without Message History](#without-message-history) -
+[Multiple Models and Parallel Conversations](#multiple-models-and-parallel-
+conversations) - [Models](#models) - [With](#with-model) - [Standalone]
+(#standalone-model) - [Running Standalone](#running-standalone) -
 [Contributing](#contributing) - [License](#license) ## Quickstart Running Cria
 is easy. After installation, you need just five lines of code â no
 configurations, no manual downloads, and no servers to worry about. ```python
 import cria ai = cria.Cria() prompt = "Who is the CEO of OpenAI?" for chunk in
 ai.chat(prompt): print(chunk, end="") ``` ``` >>> The CEO of OpenAI is Sam
 Altman! ``` or, you can run this more configurable example. ```python import
 cria with cria.Model() as ai: prompt = "Who is the CEO of OpenAI?" response =
@@ -65,15 +67,34 @@
 the example, instructions are given to the LLM as the `system`. Then, extra
 context is given as the `user`. Finally, the prompt is entered (as a `user`).
 You can use any mixture of roles to specify the LLM to your liking. The
 available roles for messages are: - `user` - Pass prompts as the user. -
 `system` - Give instructions as the system. - `assistant` - Act as the AI
 assistant yourself, and give the LLM lines. The prompt parameter will always be
 appended to messages under the `user` role, to override this, you can choose to
-pass in nothing for `prompt`. ### Multiple Models and Parallel Conversations
+pass in nothing for `prompt`. ### Interrupting #### With Message History If you
+are streaming messages with Cria, you can interrupt the prompt mid way.
+```python response = "" max_token_length = 5 prompt = "Who is the CEO of
+OpenAI?" for i, chunk in enumerate(ai.chat(prompt)): if i >= max_token_length:
+ai.stop() print(chunk, end="") # The CEO of OpenAI is ``` ```python response =
+"" max_token_length = 5 prompt = "Who is the CEO of OpenAI?" for i, chunk in
+enumerate(ai.generate(prompt)): if i >= max_token_length: ai.stop() print
+(chunk, end="") # The CEO of OpenAI is ``` In the examples, after the AI
+generates five tokens (units of text that are usually a couple of characters
+long), text generation is stopped via the `stop` method. After `stop` is
+called, you can safely `break` out of the `for` loop. #### Without Message
+History By default, Cria automatically saves responses in message history, even
+if the stream is interrupted. To prevent this behaviour though, you can pass in
+the `allow_interruption` boolean. ```python ai = cria.Cria
+(allow_interruption=False) response = "" max_token_length = 5 prompt = "Who is
+the CEO of OpenAI?" for i, chunk in enumerate(ai.chat(prompt)): if i >=
+max_token_length: ai.stop() break print(chunk, end="") # The CEO of OpenAI is
+prompt = "Tell me more about him." for chunk in ai.chat(prompt): print(chunk,
+end="") # I apologize, but I don't have any information about "him" because the
+conversation just started... ``` ### Multiple Models and Parallel Conversations
 #### Models If you are running multiple models or parallel conversations, the
 `Model` class is also available. This is recommended for most use cases.
 ```python import cria ai = cria.Model() prompt = "Who is the CEO of OpenAI?"
 response = ai.chat(prompt, stream=False) print(response) # The CEO of OpenAI is
 Sam Altman. ``` _All methods that apply to the `Cria` class also apply to
 `Model`._ #### With Model Multiple models can be run through a `with`
 statement. This automatically closes them after use. ```python import cria
```

### Comparing `cria-1.6.2/pyproject.toml` & `cria-1.6.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "cria"
-version = "1.6.2"
+version = "1.6.5"
 authors = [{ name = "leftmove", email = "100anonyo@gmail.com" }]
 description = "Run AI locally with as little friction as possible"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
@@ -13,15 +13,15 @@
 
 [project.urls]
 Homepage = "https://github.com/leftmove/cria"
 Issues = "https://github.com/leftmove/cria/issues"
 
 [tool.poetry]
 name = "cria"
-version = "1.6.2"
+version = "1.6.5"
 description = "Run AI locally with as little friction as possible."
 authors = ["leftmove"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `cria-1.6.2/src/cria.py` & `cria-1.6.5/src/cria.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,23 +19,39 @@
 
 class Client(OllamaClient):
     def chat_stream(self, messages, **kwargs):
         model = self.model
         ai = ollama
 
         response = ""
+        self.running = True
 
         for chunk in ai.chat(model=model, messages=messages, stream=True, **kwargs):
+            if self.stop_stream:
+                if self.allow_interruption:
+                    messages.append({"role": "assistant", "content": response})
+                self.running = False
+                return
             content = chunk["message"]["content"]
             response += content
             yield content
 
+        self.running = False
+
         messages.append({"role": "assistant", "content": response})
         self.messages = messages
 
+    stop_stream = False
+
+    def stop(self):
+        if self.running:
+            self.stop_stream = True
+        else:
+            raise ValueError("No active chat stream to stop.")
+
     def chat(
         self,
         prompt: Optional[str] = None,
         messages: Optional[list] = DEFAULT_MESSAGE_HISTORY,
         stream: Optional[bool] = True,
         **kwargs,
     ) -> str:
@@ -66,18 +82,27 @@
 
         return response
 
     def generate_stream(self, prompt, **kwargs):
         model = self.model
         ai = ollama
 
+        response = ""
+        self.running = True
+
         for chunk in ai.generate(model=model, prompt=prompt, stream=True, **kwargs):
+            if self.stop_stream:
+                self.running = False
+                return
             content = chunk["response"]
+            response += content
             yield content
 
+        self.running = False
+
     def generate(self, prompt: str, stream: Optional[bool] = True, **kwargs) -> str:
         model = self.model
         ai = ollama
 
         if stream:
             return self.generate_stream(prompt)
 
@@ -152,21 +177,23 @@
 class Cria(Client):
     def __init__(
         self,
         model: Optional[str] = DEFAULT_MODEL,
         standalone: Optional[bool] = False,
         run_subprocess: Optional[bool] = False,
         capture_output: Optional[bool] = False,
+        allow_interruption: Optional[bool] = True,
         silence_output: Optional[bool] = False,
         close_on_exit: Optional[bool] = True,
     ) -> None:
         self.run_subprocess = run_subprocess
         self.capture_output = capture_output
         self.silence_output = silence_output
         self.close_on_exit = close_on_exit
+        self.allow_interruption = allow_interruption
 
         ollama_process = find_process(["ollama", "serve"])
         self.ollama_process = ollama_process
 
         if ollama_process and run_subprocess:
             self.ollama_process.kill()
 
@@ -198,28 +225,33 @@
             self.ollama_subrprocess = None
 
         self.model = check_models(model, silence_output)
 
         if not standalone:
             self.llm = find_process(["ollama", "run", self.model])
 
-            if self.llm and run_subprocess:
+            if run_subprocess and self.llm:
                 self.llm.kill()
+                self.llm = None
+
+            if not self.llm:
                 self.llm = subprocess.Popen(
                     ["ollama", "run", self.model],
                     stdout=subprocess.DEVNULL,
                     stderr=subprocess.DEVNULL,
                 )
 
         if close_on_exit and self.ollama_subrprocess:
             atexit.register(lambda: self.ollama_subrprocess.kill())
 
         if close_on_exit and not standalone:
             atexit.register(lambda: self.llm.kill())
 
+    messages = DEFAULT_MESSAGE_HISTORY
+
     def output(self):
         ollama_subprocess = self.ollama_subrprocess
         if not ollama_subprocess:
             raise ValueError(
                 "Ollama is not running as a subprocess, you must pass run_subprocess as True to capture output."
             )
         if not self.capture_output:
@@ -236,27 +268,29 @@
 
 class Model(Cria, ContextDecorator):
     def __init__(
         self,
         model: Optional[str] = DEFAULT_MODEL,
         run_attached: Optional[bool] = False,
         run_subprocess: Optional[bool] = False,
+        allow_interruption: Optional[bool] = True,
         capture_output: Optional[bool] = False,
         silence_output: Optional[bool] = False,
         close_on_exit: Optional[bool] = True,
     ) -> None:
         super().__init__(
             model=model,
             capture_output=capture_output,
             run_subprocess=False,
             standalone=True,
             close_on_exit=close_on_exit,
         )
 
         self.capture_output = capture_output
+        self.allow_interruption = allow_interruption
         self.silence_output = silence_output
         self.close_on_exit = close_on_exit
 
         self.model = check_models(model, silence_output)
 
         if run_attached and run_subprocess:
             raise ValueError(
```

### Comparing `cria-1.6.2/PKG-INFO` & `cria-1.6.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cria
-Version: 1.6.2
+Version: 1.6.5
 Summary: Run AI locally with as little friction as possible.
 License: MIT
 Author: leftmove
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -46,14 +46,17 @@
   - [Custom Models](#custom-models)
   - [Streams](#streams)
   - [Closing](#closing)
   - [Message History](#message-history)
     - [Follow-Up](#follow-up)
     - [Clear Message History](#clear-message-history)
     - [Passing In Custom Context](#passing-in-custom-context)
+  - [Interrupting](#interrupting)
+    - [With Message History](#with-message-history)
+    - [Without Message History](#without-message-history)
   - [Multiple Models and Parallel Conversations](#multiple-models-and-parallel-conversations)
     - [Models](#models)
     - [With](#with-model)
     - [Standalone](#standalone-model)
   - [Running Standalone](#running-standalone)
 - [Contributing](#contributing)
 - [License](#license)
@@ -67,27 +70,30 @@
 
 ai = cria.Cria()
 
 prompt = "Who is the CEO of OpenAI?"
 for chunk in ai.chat(prompt):
     print(chunk, end="")
 ```
+
 ```
 >>> The CEO of OpenAI is Sam Altman!
 ```
+
 or, you can run this more configurable example.
 
 ```python
 import cria
 
 with cria.Model() as ai:
   prompt = "Who is the CEO of OpenAI?"
   response = ai.chat(prompt, stream=False)
   print(response)
 ```
+
 ```
 >>> The CEO of OpenAI is Sam Altman!
 ```
 
 If no model is configured, Cria runs the default model: `llama3:8b`. If the default model is not installed on your machine, Cria will install it automatically.
 
 **Important**: `llama3:8b` is about **4.7GB**, and will likely take a while to download.
@@ -208,14 +214,72 @@
 
 - `user` - Pass prompts as the user.
 - `system` - Give instructions as the system.
 - `assistant` - Act as the AI assistant yourself, and give the LLM lines.
 
 The prompt parameter will always be appended to messages under the `user` role, to override this, you can choose to pass in nothing for `prompt`.
 
+### Interrupting
+
+#### With Message History
+
+If you are streaming messages with Cria, you can interrupt the prompt mid way.
+
+```python
+response = ""
+max_token_length = 5
+
+prompt = "Who is the CEO of OpenAI?"
+for i, chunk in enumerate(ai.chat(prompt)):
+
+  if i >= max_token_length:
+    ai.stop()
+
+  print(chunk, end="") # The CEO of OpenAI is
+```
+
+```python
+response = ""
+max_token_length = 5
+
+prompt = "Who is the CEO of OpenAI?"
+for i, chunk in enumerate(ai.generate(prompt)):
+
+  if i >= max_token_length:
+    ai.stop()
+
+  print(chunk, end="") # The CEO of OpenAI is
+```
+
+In the examples, after the AI generates five tokens (units of text that are usually a couple of characters long), text generation is stopped via the `stop` method. After `stop` is called, you can safely `break` out of the `for` loop.
+
+#### Without Message History
+
+By default, Cria automatically saves responses in message history, even if the stream is interrupted. To prevent this behaviour though, you can pass in the `allow_interruption` boolean.
+
+```python
+ai = cria.Cria(allow_interruption=False)
+
+response = ""
+max_token_length = 5
+
+prompt = "Who is the CEO of OpenAI?"
+for i, chunk in enumerate(ai.chat(prompt)):
+
+  if i >= max_token_length:
+    ai.stop()
+    break
+
+  print(chunk, end="") # The CEO of OpenAI is
+
+prompt = "Tell me more about him."
+for chunk in ai.chat(prompt):
+  print(chunk, end="") # I apologize, but I don't have any information about "him" because the conversation just started...
+```
+
 ### Multiple Models and Parallel Conversations
 
 #### Models
 
 If you are running multiple models or parallel conversations, the `Model` class is also available. This is recommended for most use cases.
 
 ```python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cria Version: 1.6.2 Summary: Run AI locally with as
+Metadata-Version: 2.1 Name: cria Version: 1.6.5 Summary: Run AI locally with as
 little friction as possible. License: MIT Author: leftmove Requires-Python:
 >=3.8,<4.0 Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Requires-
 Dist: ollama (>=0.1.8,<0.2.0) Requires-Dist: psutil (>=5.9.8,<6.0.0)
@@ -16,17 +16,19 @@
 less code to save time and avoid duplication. - **Efficient**: Use advanced
 features with your own `ollama` instance, or a subprocess. ## Guide - [Quick
 Start](#quickstart) - [Installation](#installation) - [Windows](#windows) -
 [Mac](#mac) - [Linux](#linux) - [Advanced Usage](#advanced-usage) - [Custom
 Models](#custom-models) - [Streams](#streams) - [Closing](#closing) - [Message
 History](#message-history) - [Follow-Up](#follow-up) - [Clear Message History]
 (#clear-message-history) - [Passing In Custom Context](#passing-in-custom-
-context) - [Multiple Models and Parallel Conversations](#multiple-models-and-
-parallel-conversations) - [Models](#models) - [With](#with-model) -
-[Standalone](#standalone-model) - [Running Standalone](#running-standalone) -
+context) - [Interrupting](#interrupting) - [With Message History](#with-
+message-history) - [Without Message History](#without-message-history) -
+[Multiple Models and Parallel Conversations](#multiple-models-and-parallel-
+conversations) - [Models](#models) - [With](#with-model) - [Standalone]
+(#standalone-model) - [Running Standalone](#running-standalone) -
 [Contributing](#contributing) - [License](#license) ## Quickstart Running Cria
 is easy. After installation, you need just five lines of code â no
 configurations, no manual downloads, and no servers to worry about. ```python
 import cria ai = cria.Cria() prompt = "Who is the CEO of OpenAI?" for chunk in
 ai.chat(prompt): print(chunk, end="") ``` ``` >>> The CEO of OpenAI is Sam
 Altman! ``` or, you can run this more configurable example. ```python import
 cria with cria.Model() as ai: prompt = "Who is the CEO of OpenAI?" response =
@@ -74,15 +76,34 @@
 the example, instructions are given to the LLM as the `system`. Then, extra
 context is given as the `user`. Finally, the prompt is entered (as a `user`).
 You can use any mixture of roles to specify the LLM to your liking. The
 available roles for messages are: - `user` - Pass prompts as the user. -
 `system` - Give instructions as the system. - `assistant` - Act as the AI
 assistant yourself, and give the LLM lines. The prompt parameter will always be
 appended to messages under the `user` role, to override this, you can choose to
-pass in nothing for `prompt`. ### Multiple Models and Parallel Conversations
+pass in nothing for `prompt`. ### Interrupting #### With Message History If you
+are streaming messages with Cria, you can interrupt the prompt mid way.
+```python response = "" max_token_length = 5 prompt = "Who is the CEO of
+OpenAI?" for i, chunk in enumerate(ai.chat(prompt)): if i >= max_token_length:
+ai.stop() print(chunk, end="") # The CEO of OpenAI is ``` ```python response =
+"" max_token_length = 5 prompt = "Who is the CEO of OpenAI?" for i, chunk in
+enumerate(ai.generate(prompt)): if i >= max_token_length: ai.stop() print
+(chunk, end="") # The CEO of OpenAI is ``` In the examples, after the AI
+generates five tokens (units of text that are usually a couple of characters
+long), text generation is stopped via the `stop` method. After `stop` is
+called, you can safely `break` out of the `for` loop. #### Without Message
+History By default, Cria automatically saves responses in message history, even
+if the stream is interrupted. To prevent this behaviour though, you can pass in
+the `allow_interruption` boolean. ```python ai = cria.Cria
+(allow_interruption=False) response = "" max_token_length = 5 prompt = "Who is
+the CEO of OpenAI?" for i, chunk in enumerate(ai.chat(prompt)): if i >=
+max_token_length: ai.stop() break print(chunk, end="") # The CEO of OpenAI is
+prompt = "Tell me more about him." for chunk in ai.chat(prompt): print(chunk,
+end="") # I apologize, but I don't have any information about "him" because the
+conversation just started... ``` ### Multiple Models and Parallel Conversations
 #### Models If you are running multiple models or parallel conversations, the
 `Model` class is also available. This is recommended for most use cases.
 ```python import cria ai = cria.Model() prompt = "Who is the CEO of OpenAI?"
 response = ai.chat(prompt, stream=False) print(response) # The CEO of OpenAI is
 Sam Altman. ``` _All methods that apply to the `Cria` class also apply to
 `Model`._ #### With Model Multiple models can be run through a `with`
 statement. This automatically closes them after use. ```python import cria
```

