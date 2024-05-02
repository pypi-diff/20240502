# Comparing `tmp/composio_crewai-0.2.8.tar.gz` & `tmp/composio_crewai-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.2.8.tar", last modified: Thu Apr 18 18:07:45 2024, max compression
+gzip compressed data, was "composio_crewai-0.2.9.tar", last modified: Thu Apr 18 18:49:52 2024, max compression
```

## Comparing `composio_crewai-0.2.8.tar` & `composio_crewai-0.2.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:45.095535 composio_crewai-0.2.8/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-18 18:07:45.095353 composio_crewai-0.2.8/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-15 07:39:40.000000 composio_crewai-0.2.8/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:45.094133 composio_crewai-0.2.8/composio_crewai/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      110 2024-04-15 07:39:40.000000 composio_crewai-0.2.8/composio_crewai/__init__.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:45.095141 composio_crewai-0.2.8/composio_crewai.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-18 18:07:45.000000 composio_crewai-0.2.8/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-18 18:07:45.000000 composio_crewai-0.2.8/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:07:45.000000 composio_crewai-0.2.8/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       27 2024-04-18 18:07:45.000000 composio_crewai-0.2.8/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-18 18:07:45.000000 composio_crewai-0.2.8/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      275 2024-04-18 18:07:01.000000 composio_crewai-0.2.8/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:07:45.095570 composio_crewai-0.2.8/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-18 18:07:01.000000 composio_crewai-0.2.8/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:52.938040 composio_crewai-0.2.9/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-18 18:49:52.937870 composio_crewai-0.2.9/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-15 07:39:40.000000 composio_crewai-0.2.9/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:52.936754 composio_crewai-0.2.9/composio_crewai/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      110 2024-04-15 07:39:40.000000 composio_crewai-0.2.9/composio_crewai/__init__.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:52.937686 composio_crewai-0.2.9/composio_crewai.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       27 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-18 18:49:52.000000 composio_crewai-0.2.9/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      275 2024-04-18 18:44:03.000000 composio_crewai-0.2.9/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:52.938080 composio_crewai-0.2.9/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-18 18:44:03.000000 composio_crewai-0.2.9/setup.py
```

### Comparing `composio_crewai-0.2.8/PKG-INFO` & `composio_crewai-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.2.8
+Requires-Dist: composio_langchain===0.2.9
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.2.8/README.md` & `composio_crewai-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.2.8/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.2.9/composio_crewai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.2.8
+Requires-Dist: composio_langchain===0.2.9
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.2.8/setup.py` & `composio_crewai-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.2.8",
+    version="0.2.9",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

