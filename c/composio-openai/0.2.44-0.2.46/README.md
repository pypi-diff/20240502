# Comparing `tmp/composio_openai-0.2.44.tar.gz` & `tmp/composio_openai-0.2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.2.44.tar", last modified: Wed May  1 14:47:44 2024, max compression
+gzip compressed data, was "composio_openai-0.2.46.tar", last modified: Wed May  1 20:29:01 2024, max compression
```

## Comparing `composio_openai-0.2.44.tar` & `composio_openai-0.2.46.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 14:47:44.674059 composio_openai-0.2.44/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-01 14:47:44.673871 composio_openai-0.2.44/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     2107 2024-05-01 14:24:08.000000 composio_openai-0.2.44/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 14:47:44.673030 composio_openai-0.2.44/composio_openai/
--rw-r--r--   0 sawradip   (501) staff       (20)      182 2024-05-01 14:23:13.000000 composio_openai-0.2.44/composio_openai/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     2874 2024-05-01 14:24:08.000000 composio_openai-0.2.44/composio_openai/openai_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 14:47:44.673694 composio_openai-0.2.44/composio_openai.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-01 14:47:44.000000 composio_openai-0.2.44/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      275 2024-05-01 14:47:44.000000 composio_openai-0.2.44/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-01 14:47:44.000000 composio_openai-0.2.44/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       23 2024-05-01 14:47:44.000000 composio_openai-0.2.44/composio_openai.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-01 14:47:44.000000 composio_openai-0.2.44/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-01 14:47:44.674094 composio_openai-0.2.44/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      826 2024-05-01 14:47:09.000000 composio_openai-0.2.44/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 20:29:01.749766 composio_openai-0.2.46/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-01 20:29:01.749549 composio_openai-0.2.46/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     2107 2024-05-01 14:24:08.000000 composio_openai-0.2.46/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 20:29:01.748688 composio_openai-0.2.46/composio_openai/
+-rw-r--r--   0 sawradip   (501) staff       (20)      182 2024-05-01 14:23:13.000000 composio_openai-0.2.46/composio_openai/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     2869 2024-05-01 19:58:35.000000 composio_openai-0.2.46/composio_openai/openai_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 20:29:01.749351 composio_openai-0.2.46/composio_openai.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-01 20:29:01.000000 composio_openai-0.2.46/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      275 2024-05-01 20:29:01.000000 composio_openai-0.2.46/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-01 20:29:01.000000 composio_openai-0.2.46/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       23 2024-05-01 20:29:01.000000 composio_openai-0.2.46/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-01 20:29:01.000000 composio_openai-0.2.46/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-01 20:29:01.749803 composio_openai-0.2.46/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      826 2024-05-01 20:28:48.000000 composio_openai-0.2.46/setup.py
```

### Comparing `composio_openai-0.2.44/PKG-INFO` & `composio_openai-0.2.46/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.44
+Version: 0.2.46
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.44
+Requires-Dist: composio_core===0.2.46
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.44/README.md` & `composio_openai-0.2.46/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.44/composio_openai/openai_toolspec.py` & `composio_openai-0.2.46/composio_openai/openai_toolspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     if choice.message.tool_calls:
                         for tool_call in choice.message.tool_calls:
                             action_name_to_execute = tool_call.function.name
                             action = self.client.sdk.get_action_enum_without_tool(
                                 action_name=action_name_to_execute
                             )
                             arguments = json.loads(tool_call.function.arguments)
-                            account = self.client.get_connection(app_name=action.service)
+                            account = entity.get_connection(app_name=action.service)
                             output.append(account.execute_action(action, arguments))
 
         except Exception as e:
             raise e from e
 
         return output
```

### Comparing `composio_openai-0.2.44/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.2.46/composio_openai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.44
+Version: 0.2.46
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.44
+Requires-Dist: composio_core===0.2.46
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.44/setup.py` & `composio_openai-0.2.46/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,25 +5,25 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_openai",
-    version="0.2.44",
+    version="0.2.46",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your OpenAI Function Call.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
-        "composio_core===0.2.44",
+        "composio_core===0.2.46",
     ],
     include_package_data=True,
 )
```

