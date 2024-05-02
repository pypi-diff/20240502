# Comparing `tmp/programlib-9.0.2.tar.gz` & `tmp/programlib-9.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "programlib-9.0.2.tar", max compression
+gzip compressed data, was "programlib-9.0.3.tar", max compression
```

## Comparing `programlib-9.0.2.tar` & `programlib-9.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1082 2023-11-23 17:11:57.863197 programlib-9.0.2/LICENSE
--rw-r--r--   0        0        0     4011 2023-11-23 17:11:57.863197 programlib-9.0.2/README.md
--rw-r--r--   0        0        0      137 2023-11-23 17:11:57.863197 programlib-9.0.2/programlib/__init__.py
--rw-r--r--   0        0        0     2539 2023-11-23 17:11:57.867197 programlib-9.0.2/programlib/agent.py
--rw-r--r--   0        0        0     5142 2023-11-23 17:11:57.867197 programlib-9.0.2/programlib/language.py
--rw-r--r--   0        0        0     5604 2023-11-23 17:11:57.867197 programlib-9.0.2/programlib/program.py
--rw-r--r--   0        0        0        0 2023-11-23 17:11:57.867197 programlib-9.0.2/programlib/programs/.gitkeep
--rw-r--r--   0        0        0      461 2023-11-23 17:11:57.867197 programlib-9.0.2/programlib/terminal.py
--rw-r--r--   0        0        0      577 2023-11-23 17:11:57.867197 programlib-9.0.2/pyproject.toml
--rw-r--r--   0        0        0     4958 1970-01-01 00:00:00.000000 programlib-9.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1082 2023-01-20 01:12:50.224813 programlib-9.0.3/LICENSE
+-rw-r--r--   0        0        0     4011 2023-10-18 12:44:38.135224 programlib-9.0.3/README.md
+-rw-r--r--   0        0        0      137 2023-10-03 13:37:44.676824 programlib-9.0.3/programlib/__init__.py
+-rw-r--r--   0        0        0     2552 2023-11-24 23:59:01.231226 programlib-9.0.3/programlib/agent.py
+-rw-r--r--   0        0        0     5142 2023-11-23 17:10:07.539173 programlib-9.0.3/programlib/language.py
+-rw-r--r--   0        0        0     5604 2023-11-22 15:01:54.906522 programlib-9.0.3/programlib/program.py
+-rw-r--r--   0        0        0        0 2023-01-20 01:12:50.225301 programlib-9.0.3/programlib/programs/.gitkeep
+-rw-r--r--   0        0        0      461 2023-10-03 18:14:14.792524 programlib-9.0.3/programlib/terminal.py
+-rw-r--r--   0        0        0      577 2023-11-25 00:16:49.359784 programlib-9.0.3/pyproject.toml
+-rw-r--r--   0        0        0     4894 1970-01-01 00:00:00.000000 programlib-9.0.3/PKG-INFO
```

### Comparing `programlib-9.0.2/LICENSE` & `programlib-9.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `programlib-9.0.2/README.md` & `programlib-9.0.3/README.md`

 * *Files identical despite different names*

### Comparing `programlib-9.0.2/programlib/agent.py` & `programlib-9.0.3/programlib/agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import gym
+import gymnasium as gym
 import numpy as np
 
 def decode_action(action_space, action):
     try:
         a = eval(action)
 
         if not isinstance(action_space, gym.spaces.Discrete):
```

### Comparing `programlib-9.0.2/programlib/language.py` & `programlib-9.0.3/programlib/language.py`

 * *Files identical despite different names*

### Comparing `programlib-9.0.2/programlib/program.py` & `programlib-9.0.3/programlib/program.py`

 * *Files identical despite different names*

### Comparing `programlib-9.0.2/pyproject.toml` & `programlib-9.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "programlib"
-version = "9.0.2"
+version = "9.0.3"
 description = "Programs as Objects"
 authors = ["Vadim Liventsev <dev@vadim.me>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Topic :: Software Development :: Compilers"
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pexpect = "^4.8.0"
-gym = "^0.26.2"
+gymnasium = "*"
 numpy = "^1.24.2"
 pyte = "^0.8.0"
 contextlib-chdir = {version = "^1.0.2", python = "<3.11"}
 
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `programlib-9.0.2/PKG-INFO` & `programlib-9.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 Metadata-Version: 2.1
 Name: programlib
-Version: 9.0.2
+Version: 9.0.3
 Summary: Programs as Objects
 License: MIT
 Author: Vadim Liventsev
 Author-email: dev@vadim.me
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Compilers
 Requires-Dist: contextlib-chdir (>=1.0.2,<2.0.0) ; python_version < "3.11"
-Requires-Dist: gym (>=0.26.2,<0.27.0)
+Requires-Dist: gymnasium
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pexpect (>=4.8.0,<5.0.0)
 Requires-Dist: pyte (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
 
 # Programlib: programs as objects
```

