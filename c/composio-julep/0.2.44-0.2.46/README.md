# Comparing `tmp/composio_julep-0.2.44.tar.gz` & `tmp/composio_julep-0.2.46.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.2.44.tar", last modified: Wed May  1 14:47:33 2024, max compression
+gzip compressed data, was "composio_julep-0.2.46.tar", last modified: Wed May  1 20:28:55 2024, max compression
```

## Comparing `composio_julep-0.2.44.tar` & `composio_julep-0.2.46.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 14:47:33.815760 composio_julep-0.2.44/
--rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-01 14:47:33.815493 composio_julep-0.2.44/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     3933 2024-05-01 14:24:08.000000 composio_julep-0.2.44/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 14:47:33.814417 composio_julep-0.2.44/composio_julep/
--rw-r--r--   0 sawradip   (501) staff       (20)      157 2024-05-01 14:23:13.000000 composio_julep-0.2.44/composio_julep/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     1624 2024-05-01 14:23:13.000000 composio_julep-0.2.44/composio_julep/julep_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 14:47:33.815247 composio_julep-0.2.44/composio_julep.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-01 14:47:33.000000 composio_julep-0.2.44/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      267 2024-05-01 14:47:33.000000 composio_julep-0.2.44/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-01 14:47:33.000000 composio_julep-0.2.44/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-01 14:47:33.000000 composio_julep-0.2.44/composio_julep.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       15 2024-05-01 14:47:33.000000 composio_julep-0.2.44/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-01 14:47:33.815812 composio_julep-0.2.44/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      842 2024-05-01 14:47:09.000000 composio_julep-0.2.44/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 20:28:55.346595 composio_julep-0.2.46/
+-rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-01 20:28:55.346379 composio_julep-0.2.46/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     3933 2024-05-01 14:24:08.000000 composio_julep-0.2.46/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 20:28:55.345477 composio_julep-0.2.46/composio_julep/
+-rw-r--r--   0 sawradip   (501) staff       (20)      157 2024-05-01 14:23:13.000000 composio_julep-0.2.46/composio_julep/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     1619 2024-05-01 20:17:45.000000 composio_julep-0.2.46/composio_julep/julep_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-01 20:28:55.346181 composio_julep-0.2.46/composio_julep.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     4463 2024-05-01 20:28:55.000000 composio_julep-0.2.46/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      267 2024-05-01 20:28:55.000000 composio_julep-0.2.46/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-01 20:28:55.000000 composio_julep-0.2.46/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-01 20:28:55.000000 composio_julep-0.2.46/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       15 2024-05-01 20:28:55.000000 composio_julep-0.2.46/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-01 20:28:55.346635 composio_julep-0.2.46/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      842 2024-05-01 20:28:48.000000 composio_julep-0.2.46/setup.py
```

### Comparing `composio_julep-0.2.44/PKG-INFO` & `composio_julep-0.2.46/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.44
+Version: 0.2.46
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.44
+Requires-Dist: composio_openai===0.2.46
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.44/README.md` & `composio_julep-0.2.46/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.2.44/composio_julep/julep_toolspec.py` & `composio_julep-0.2.46/composio_julep/julep_toolspec.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
                 try:
                     function = json.loads(response.content)
                     action_name_to_execute = function["name"]
                     action = self.client.sdk.get_action_enum_without_tool(
                         action_name=action_name_to_execute
                     )
                     arguments = json.loads(function["arguments"])
-                    account = self.client.get_connection(app_name=action.service)
+                    account = entity.get_connection(app_name=action.service)
                     output = account.execute_action(action, arguments)
                     
                 except json.JSONDecodeError:
                     output = response.content
                     
                 outputs.append(output)
```

### Comparing `composio_julep-0.2.44/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.2.46/composio_julep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.2.44
+Version: 0.2.46
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.44
+Requires-Dist: composio_openai===0.2.46
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.2.44/setup.py` & `composio_julep-0.2.46/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.2.44",
+    version="0.2.46",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
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
-        "composio_openai===0.2.44",
+        "composio_openai===0.2.46",
         "julep>=0.3.2"
     ],
     include_package_data=True,
 )
```

