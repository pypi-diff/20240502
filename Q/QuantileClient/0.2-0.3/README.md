# Comparing `tmp/QuantileClient-0.2.tar.gz` & `tmp/QuantileClient-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QuantileClient-0.2.tar", last modified: Sat Mar 30 17:43:21 2024, max compression
+gzip compressed data, was "QuantileClient-0.3.tar", last modified: Thu May  2 14:20:06 2024, max compression
```

## Comparing `QuantileClient-0.2.tar` & `QuantileClient-0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-03-30 17:43:21.646248 QuantileClient-0.2/
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     2050 2024-03-30 17:43:21.645649 QuantileClient-0.2/PKG-INFO
-drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-03-30 17:43:21.640952 QuantileClient-0.2/QuantileClient/
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       32 2024-03-24 20:48:45.000000 QuantileClient-0.2/QuantileClient/__init__.py
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     5066 2024-03-30 16:22:40.000000 QuantileClient-0.2/QuantileClient/main.py
-drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-03-30 17:43:21.644842 QuantileClient-0.2/QuantileClient.egg-info/
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     2050 2024-03-30 17:43:21.000000 QuantileClient-0.2/QuantileClient.egg-info/PKG-INFO
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      257 2024-03-30 17:43:21.000000 QuantileClient-0.2/QuantileClient.egg-info/SOURCES.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)        1 2024-03-30 17:43:21.000000 QuantileClient-0.2/QuantileClient.egg-info/dependency_links.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       23 2024-03-30 17:43:21.000000 QuantileClient-0.2/QuantileClient.egg-info/requires.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       15 2024-03-30 17:43:21.000000 QuantileClient-0.2/QuantileClient.egg-info/top_level.txt
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     1711 2024-03-24 19:53:25.000000 QuantileClient-0.2/README.md
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       38 2024-03-30 17:43:21.646396 QuantileClient-0.2/setup.cfg
--rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      519 2024-03-30 17:33:59.000000 QuantileClient-0.2/setup.py
+drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-02 14:20:06.742400 QuantileClient-0.3/
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4447 2024-05-02 14:20:06.740938 QuantileClient-0.3/PKG-INFO
+drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-02 14:20:06.730940 QuantileClient-0.3/QuantileClient/
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       32 2024-03-24 20:48:45.000000 QuantileClient-0.3/QuantileClient/__init__.py
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     6912 2024-05-02 13:30:35.000000 QuantileClient-0.3/QuantileClient/main.py
+drwxr-xr-x   0 aryanrajpurohit   (501) staff       (20)        0 2024-05-02 14:20:06.739765 QuantileClient-0.3/QuantileClient.egg-info/
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4447 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/PKG-INFO
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      257 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/SOURCES.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)        1 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/dependency_links.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       23 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/requires.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       15 2024-05-02 14:20:06.000000 QuantileClient-0.3/QuantileClient.egg-info/top_level.txt
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)     4108 2024-05-02 14:17:20.000000 QuantileClient-0.3/README.md
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)       38 2024-05-02 14:20:06.742680 QuantileClient-0.3/setup.cfg
+-rw-r--r--   0 aryanrajpurohit   (501) staff       (20)      519 2024-05-02 14:19:00.000000 QuantileClient-0.3/setup.py
```

### Comparing `QuantileClient-0.2/QuantileClient/main.py` & `QuantileClient-0.3/QuantileClient/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         return os.getenv("API_KEY")
 
     def save_api_key_to_env(self, api_key):
         with open(".env", "w") as f:
             f.write(f"API_KEY={api_key}")
 
     def generate_openai_response(self, model, messages, tools=None, tool_choice=None, max_tokens=None,
-                                 temperature=None, top_p=None, frequency_penalty=None, presence_penalty=None):
+                                 temperature=None, top_p=None, frequency_penalty=None, presence_penalty=None,parsed_output=False):
         messages_json = json.dumps(messages)
         url = f"{self.base_url}/generate_openai_response"
         headers = {
             "accept": "application/json",
             "quant-api-key": self.api_key
         }
         payload = {
@@ -31,49 +31,52 @@
             "messages": messages_json,
             "tools": tools,
             "tool_choice": tool_choice,
             "max_tokens": max_tokens,
             "temperature": temperature,
             "top_p": top_p,
             "frequency_penalty": frequency_penalty,
-            "presence_penalty": presence_penalty
+            "presence_penalty": presence_penalty,
+            "parese_output": parsed_output
         }
         response = requests.get(url, headers=headers, params=payload)
         return response.json()
 
-    def generate_anthropic_response(self, messages, model=None, max_tokens=None, temperature=None):
+    def generate_anthropic_response(self, messages, model=None, max_tokens=None, temperature=None,parsed_output=False):
         url = f"{self.base_url}/generate_anthropic_response"
         messages_json = json.dumps(messages)
 
         headers = {
             "accept": "application/json",
             "quant-api-key": self.api_key
         }
         payload = {
             "messages": messages_json,
             "model": model,
             "max_tokens": max_tokens,
-            "temperature": temperature
+            "temperature": temperature,
+            "parese_output": parsed_output
         }
         response = requests.get(url, headers=headers, params=payload)
         return response.json()
 
-    def generate_deepinfra_response(self, messages, model=None, max_tokens=None, temperature=None):
+    def generate_deepinfra_response(self, messages, model=None, max_tokens=None, temperature=None,parsed_output=False):
         url = f"{self.base_url}/generate_deepinfra_response"
         messages_json = json.dumps(messages)
 
         headers = {
             "accept": "application/json",
             "quant-api-key": self.api_key
         }
         payload = {
             "messages":messages_json,
             "model": model,
             "max_tokens": max_tokens,
-            "temperature": temperature
+            "temperature": temperature,
+            "parese_output":parsed_output
         }
         response = requests.get(url, headers=headers, params=payload)
         return response.json()
 
     def generate_perplexity_response(self, messages, model=None, max_tokens=None, temperature=None):
         url = f"{self.base_url}/generate_perplexity_response"
         messages_json = json.dumps(messages)
@@ -110,25 +113,26 @@
             "temperature": temperature,
             "max_tokens": max_tokens,
             "connectors": connectors
         }
         response = requests.get(url, headers=headers, params=payload)
         return response.json()
     
-    def call_cascading(self,prompt, max_tokens=None,temperature=None):
+    def call_cascading(self,prompt, max_tokens=None,temperature=None,parsed_output=False):
         
         url = f"{self.base_url}/call_cascading"
         headers = {
             "accept": "application/json",
             "quant-api-key": self.api_key
         }
         params = {
             "prompt": prompt,
             "max_tokens": max_tokens,
-            "temperature":temperature
+            "temperature":temperature,
+            "parese_output":parsed_output
         }
         response = requests.get(url, headers=headers, params=params)
         return response.json()
     
     def image_gen(self,prompt,model,width,height,num_images,quality):
         url = f"{self.base_url}/image_generation"
         headers = {
@@ -142,8 +146,55 @@
             "height": height,
             "num_images": num_images,
             "quality": quality
         
         }
         response = requests.get(url, headers=headers, params=params)
         return response.json()
+    def rag_data_upload(self, db_name, pdf_file, chunk_size=100, chunk_overlap=10, embedding_model="text-embedding-3-small"):
+        url = f"{self.base_url}/rag_data_upload"
+        
+        headers = {
+            "accept": "application/json",
+            "quant-api-key": self.api_key
+        }
+        
+        params = {
+            "db_name": db_name,
+            "pdf_file": pdf_file,
+            "chunk_size": chunk_size,
+            "chunk_overlap": chunk_overlap,
+            "embedding_model": embedding_model
+        }
+        if not os.path.exists(pdf_file):
+            return {"error": "File not found"}
+        
+        with open(pdf_file, 'rb') as file:
+            files = {'pdf_file': (os.path.basename(pdf_file), file)}
+            response = requests.post(url, headers=headers, params=params, files=files)
+        
+        return response.json()
+    def rag_chat(self,db_name,description,question,embedding_model="text-embedding-3-small",inference_model="gpt-3.5-turbo-0125",temperature=0):
+        url = f"{self.base_url}/rag_assistant"
+        
+        headers = {
+            "accept": "application/json",
+            "quant-api-key": self.api_key
+        }
+        params = {
+            "db_name": db_name,
+            "description": description,
+            "question": question,
+            "embedding_model": embedding_model,
+            "inference_model": inference_model,
+            "temperature": temperature
+        }
+        
+        response = requests.get(url, headers=headers, params=params)
+        return response.json()
+
+        
+ 
+        
+
+
```

### Comparing `QuantileClient-0.2/setup.py` & `QuantileClient-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='QuantileClient',
-    version='0.2',
+    version='0.3',
     packages=find_packages(),
     install_requires=[
         'python-dotenv',
         'requests',
     ],
     author='QuantileaiDev',
     author_email='quantileai@gmail.com',
```

