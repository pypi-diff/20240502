# Comparing `tmp/hellologger-0.2.2.tar.gz` & `tmp/hellologger-0.2.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hellologger-0.2.2.tar", max compression
+gzip compressed data, was "hellologger-0.2.2.post1.tar", max compression
```

## Comparing `hellologger-0.2.2.tar` & `hellologger-0.2.2.post1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1086 2024-03-22 13:18:42.471202 hellologger-0.2.2/LICENSE
--rw-r--r--   0        0        0      596 2024-05-02 16:57:50.292853 hellologger-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     4354 2024-03-31 15:04:10.183295 hellologger-0.2.2/README.md
--rw-r--r--   0        0        0     4860 2024-05-02 16:56:56.465688 hellologger-0.2.2/src/hellologger/__init__.py
--rw-r--r--   0        0        0      308 2024-03-23 15:31:02.983633 hellologger-0.2.2/src/hellologger/const.py
--rw-r--r--   0        0        0     4986 1970-01-01 00:00:00.000000 hellologger-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-03-22 13:18:42.471202 hellologger-0.2.2.post1/LICENSE
+-rw-r--r--   0        0        0      601 2024-05-02 17:35:00.702011 hellologger-0.2.2.post1/pyproject.toml
+-rw-r--r--   0        0        0     4354 2024-03-31 15:04:10.183295 hellologger-0.2.2.post1/README.md
+-rw-r--r--   0        0        0     6078 2024-05-02 17:33:31.290933 hellologger-0.2.2.post1/src/hellologger/__init__.py
+-rw-r--r--   0        0        0      345 2024-05-02 17:32:48.532251 hellologger-0.2.2.post1/src/hellologger/const.py
+-rw-r--r--   0        0        0     4842 1970-01-01 00:00:00.000000 hellologger-0.2.2.post1/PKG-INFO
```

### Comparing `hellologger-0.2.2/LICENSE` & `hellologger-0.2.2.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `hellologger-0.2.2/pyproject.toml` & `hellologger-0.2.2.post1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "hellologger"
-version = "0.2.2"
+version = "0.2.2.post1"
 description = ""
 authors = ["快乐的老鼠宝宝 <laoshubaby@protonmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/OSMChina/Yuheng"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 packages = [{ include = "hellologger", from = "src" }]
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.11"
 loguru = "^0.7.2"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `hellologger-0.2.2/README.md` & `hellologger-0.2.2.post1/README.md`

 * *Files identical despite different names*

### Comparing `hellologger-0.2.2/PKG-INFO` & `hellologger-0.2.2.post1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: hellologger
-Version: 0.2.2
+Version: 0.2.2.post1
 Summary: 
 Home-page: https://github.com/OSMChina/Yuheng
 License: MIT
 Author: 快乐的老鼠宝宝
 Author-email: laoshubaby@protonmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Project-URL: Repository, https://github.com/OSMChina/Yuheng
 Description-Content-Type: text/markdown
 
 # HelloLogger
```

