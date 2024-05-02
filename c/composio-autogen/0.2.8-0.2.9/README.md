# Comparing `tmp/composio_autogen-0.2.8.tar.gz` & `tmp/composio_autogen-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.2.8.tar", last modified: Thu Apr 18 18:07:51 2024, max compression
+gzip compressed data, was "composio_autogen-0.2.9.tar", last modified: Thu Apr 18 18:49:59 2024, max compression
```

## Comparing `composio_autogen-0.2.8.tar` & `composio_autogen-0.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:51.060133 composio_autogen-0.2.8/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-18 18:07:51.059956 composio_autogen-0.2.8/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-15 07:39:40.000000 composio_autogen-0.2.8/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:51.058835 composio_autogen-0.2.8/composio_autogen/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      100 2024-04-15 07:39:40.000000 composio_autogen-0.2.8/composio_autogen/__init__.py
--rw-r--r--   0 karanvaidya   (501) staff       (20)     8535 2024-04-16 16:08:42.000000 composio_autogen-0.2.8/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:07:51.059775 composio_autogen-0.2.8/composio_autogen.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-18 18:07:51.000000 composio_autogen-0.2.8/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-18 18:07:51.000000 composio_autogen-0.2.8/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:07:51.000000 composio_autogen-0.2.8/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       40 2024-04-18 18:07:51.000000 composio_autogen-0.2.8/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-18 18:07:51.000000 composio_autogen-0.2.8/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      297 2024-04-18 18:07:01.000000 composio_autogen-0.2.8/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:07:51.060173 composio_autogen-0.2.8/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      840 2024-04-18 18:07:01.000000 composio_autogen-0.2.8/setup.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:59.117014 composio_autogen-0.2.9/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-18 18:49:59.116839 composio_autogen-0.2.9/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     2776 2024-04-15 07:39:40.000000 composio_autogen-0.2.9/README.md
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:59.115550 composio_autogen-0.2.9/composio_autogen/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      100 2024-04-15 07:39:40.000000 composio_autogen-0.2.9/composio_autogen/__init__.py
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     8535 2024-04-16 16:08:42.000000 composio_autogen-0.2.9/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-18 18:49:59.116643 composio_autogen-0.2.9/composio_autogen.egg-info/
+-rw-r--r--   0 karanvaidya   (501) staff       (20)     3306 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      298 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       40 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       17 2024-04-18 18:49:59.000000 composio_autogen-0.2.9/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      296 2024-04-18 18:47:29.000000 composio_autogen-0.2.9/pyproject.toml
+-rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-18 18:49:59.117136 composio_autogen-0.2.9/setup.cfg
+-rw-r--r--   0 karanvaidya   (501) staff       (20)      840 2024-04-18 18:44:03.000000 composio_autogen-0.2.9/setup.py
```

### Comparing `composio_autogen-0.2.8/PKG-INFO` & `composio_autogen-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.8
+Requires-Dist: composio_core===0.2.9
 Requires-Dist: pyautogen>=0.2.29
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.2.8/README.md` & `composio_autogen-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.2.8/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.2.9/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.2.8/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.2.9/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.2.8
+Version: 0.2.9
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.8
+Requires-Dist: composio_core===0.2.9
 Requires-Dist: pyautogen>=0.2.29
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.2.8/setup.py` & `composio_autogen-0.2.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.2.8",
+    version="0.2.9",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

